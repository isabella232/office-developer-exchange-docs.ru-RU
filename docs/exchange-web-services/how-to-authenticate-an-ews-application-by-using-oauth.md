---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.
ms.openlocfilehash: 8b6a3fd72e42a36e31f261205292de28ef341270
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353583"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Проверка подлинности приложения EWS с помощью OAuth

Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.
  
Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, для интеграции приложений управляемых API EWS с той же моделью проверки подлинности, что и для REST API Office 365. Чтобы использовать OAuth с вашим приложением, необходимо выполнить следующие действия:
  
1. [Зарегистрируйте свое приложение](#bk_register) с помощью Azure Active Directory. 
    
2. [Добавьте код, чтобы получить маркер проверки](#bk_getToken) подлинности для получения маркера проверки подлинности с сервера маркеров. 
    
3. [Добавьте маркер проверки подлинности в](#bk_useToken) отправляемые вами запросы EWS. 
    
> [!NOTE]
> Проверка подлинности OAuth для EWS доступна только в Exchange в составе Office 365. Приложениям EWS требуется разрешение "полный доступ к почтовому ящику пользователя". 
  
Чтобы использовать код, описанный в этой статье, вам потребуется доступ к следующим программам:
  
- [Учетная запись разработчика Office 365](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program). Для тестирования приложения можно использовать пробную учетную запись.
    
- [Библиотека проверки подлинности Azure AD для .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).
    
- [Управляемый API EWS](https://github.com/officedev/ews-managed-api.aspx).

<a name="bk_register"> </a>

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно иметь идентификатор клиента и URI приложения, который идентифицирует приложение. Если вы еще не зарегистрировали приложение с помощью служб Azure Active Directory, вам потребуется вручную добавить свое приложение, выполнив действия, описанные в статье [Регистрация приложения](https://apps.dev.microsoft.com/#/appList).

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>Добавление кода для получения маркера проверки подлинности

Библиотека проверки подлинности Azure AD для .NET упрощает извлечение маркера проверки подлинности из Azure Active Directory, чтобы можно было использовать маркер в приложении. Для получения маркера необходимо предоставить четыре фрагмента данных:
  
1. Универсальный код ресурса (URI) сервера маркеров. Сервер маркеров — это **центр** , проверяющий подлинность пользователя и возвращающий маркер, который приложение может использовать для доступа к EWS. 
    
2. Идентификатор клиента приложения, созданный при регистрации приложения с помощью Azure Active Directory.
    
3. URI клиента приложения, созданный при регистрации приложения в Azure Active Directory.
    
4. Универсальный код ресурса (URI) сервера EWS и URI конечной точки EWS. Для Exchange в составе Office 365 это будет быть `https://<server name>/ews/exchange.asmx`.
    
В приведенном ниже коде показано, как использовать библиотеку проверки подлинности Azure AD для получения маркера проверки подлинности. Предполагается, что сведения, необходимые для выполнения запроса на проверку подлинности, хранятся в файле App. config приложения. В этом примере не включается проверка ошибок, приведен [пример кода](#bk_codeSample) для полного кода. 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<a name="bk_useToken"> </a>

## <a name="add-an-authentication-token-to-ews-requests"></a>Добавление маркера проверки подлинности в запросы EWS

После получения объекта **аусентикатионресулт** можно использовать свойство **AccessToken** для получения маркера, выданного службой маркеров. 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<a name="bk_codeSample"> </a>

## <a name="code-sample"></a>Пример кода

Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth.
  
```cs
using System;
using System.Collections.Generic;
using System.Configuration;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;
using System.Web.Script.Serialization;
using Microsoft.Exchange.WebServices.Autodiscover;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.IdentityModel.Clients.ActiveDirectory;
namespace TestV1App
{
    class Program
    {
        static void Main(string[] args)
        {
            var t = new Thread(Run);
            t.SetApartmentState(ApartmentState.STA);
            t.Start();
            t.Join();
        }
        static void Run()
        {
           string authority = ConfigurationManager.AppSettings["authority"];
           string clientID = ConfigurationManager.AppSettings["clientID"];
           Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
           string serverName = ConfigurationManager.AppSettings["serverName"];
            AuthenticationResult authenticationResult = null;
            AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
            
            string errorMessage = null;
            try
            {
                Console.WriteLine("Trying to acquire token");
                authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);
            }
                catch (AdalException ex)
            {
                errorMessage = ex.Message;
                if (ex.InnerException != null)
                {
                    errorMessage += "\nInnerException : " + ex.InnerException.Message;
                }
            }
            catch (ArgumentException ex)
            {
                errorMessage = ex.Message;
            }
            if (!string.IsNullOrEmpty(errorMessage))
            {
                Console.WriteLine("Failed: {0}" + errorMessage);
                return;
            }
            Console.WriteLine("\nMaking the protocol call\n");
            ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
            exchangeService.Url = new Uri(resource + "ews/exchange.asmx");
            exchangeService.TraceEnabled = true;
            exchangeService.TraceFlags = TraceFlags.All;
            exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken);
            exchangeService.FindFolders(WellKnownFolderName.Root, new FolderView(10));
        }
    }
}

```

Для примера кода требуется файл App. config со следующими записями:
  
```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.5" />
  </startup>
  <appSettings>
    <add key="authority" value="http://login.windows.net/<devAccountName>.onmicrosoft.com" />
    <add key="clientId" value="<ID generated by Azure Active Directory"/>
    <add key="clientAppUri" value="<URI registered with Azure Active Directory"/>
    <add key="serverName" value="outlook.office365.com" />
  </appSettings>
</configuration>
```

## <a name="see-also"></a>См. также

- [Проверка подлинности и EWS в Exchange](authentication-and-ews-in-exchange.md)    

    

