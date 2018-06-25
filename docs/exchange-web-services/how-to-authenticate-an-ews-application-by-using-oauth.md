---
title: Проверка подлинности приложения веб-служб Exchange с помощью OAuth
manager: sethgros
ms.date: 1/15/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth с приложениями управляемый API веб-служб Exchange.
ms.openlocfilehash: 66bbc0525ecf78407e853da0c8dcdec92791ca56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760977"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Проверка подлинности приложения веб-служб Exchange с помощью OAuth

Узнайте, как использовать проверку подлинности OAuth с приложениями управляемый API веб-служб Exchange.
  
Служба проверки подлинности OAuth, предоставляемая Azure Active Directory можно использовать для интеграции приложений управляемый API веб-служб Exchange с помощью той же модели проверки подлинности, используемых API-интерфейсы REST Office 365. Для использования OAuth с приложением, необходимую для:
  
1. [Регистрация приложения](#bk_register) с помощью Azure Active Directory. 
    
2. [Добавьте код для получения маркера проверки подлинности](#bk_getToken) для получения маркера проверки подлинности с сервера маркеров. 
    
3. [Добавить маркера проверки подлинности для запросов веб-служб Exchange](#bk_useToken) , можно отправить. 
    
> [!NOTE]
> Проверка подлинности OAuth для веб-служб Exchange доступна только в составе Office 365 Exchange. Приложения веб-служб Exchange требуется разрешение «Полный доступ к почтовому ящику пользователя». 
  
Чтобы использовать код в этой статье, необходимо иметь доступ к таким компонентам:
  
- [Учетная запись разработчика Office 365](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx). Пробной учетной записи можно использовать для тестирования приложения
    
- [Библиотека проверки подлинности Azure AD для платформы .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).
    
- [Управляемый API веб-служб Exchange](https://github.com/officedev/ews-managed-api.aspx).

<a name="bk_register"> </a>

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно иметь идентификатор клиента и URI, определяющая приложение, приложения. Если вы еще не зарегистрирован приложения с помощью служб Azure Active Directory, то необходимо вручную добавить приложения с помощью шагов, описанных в разделе [Регистрация приложения вы](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>Добавление кода для получения маркера проверки подлинности

Библиотеке проверка подлинности Azure AD для платформы .NET упрощает получение маркера проверки подлинности с Azure Active Directory, можно использовать маркер в приложении. Необходимо указать четыре фрагмента данных для получения маркера:
  
1. URI сервера маркеров. Сервер — это **центра сертификации** , который выполняет проверку подлинности пользователя и возвращает маркер, приложение может использовать для доступа к веб-служб Exchange. 
    
2. Идентификатор клиента приложения, созданные при регистрации приложения в Azure Active Directory.
    
3. URI, созданному при регистрации приложения с помощью Azure Active Directory клиентского приложения.
    
4. URI сервера веб-служб Exchange и URI конечной точки веб-служб Exchange. Для Exchange в составе Office 365, это будет `https://<server name>/ews/exchange.asmx`.
    
Приведенный ниже код показано, как использовать библиотеку проверка подлинности Azure AD для получения маркера проверки подлинности. Предполагается, что сведения, необходимые для выполнения запроса проверки подлинности хранится в файле App.config приложения. В этом примере не включают проверки ошибок, просмотрите [образец кода](#bk_codeSample) для выполнения кода. 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<a name="bk_useToken"> </a>

## <a name="add-an-authentication-token-to-ews-requests"></a>Добавление маркера проверки подлинности для запросов веб-служб Exchange

После получения объекта **AuthenticationResult** можно использовать свойство **AccessToken** для получения маркера, выдаваемого службой маркеров. 
  
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

Ниже приведен полный пример кода, в котором показывается делает запрос на проверку подлинности OAuth веб-служб Exchange.
  
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

Пример кода требует файле App.config с помощью следующие записи:
  
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

- [Проверка подлинности и веб-службах Exchange](authentication-and-ews-in-exchange.md)    
- [Тестирование и развертывание приложений Office 365](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    

