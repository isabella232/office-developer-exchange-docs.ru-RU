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
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="91e37-103">Проверка подлинности приложения EWS с помощью OAuth</span><span class="sxs-lookup"><span data-stu-id="91e37-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="91e37-104">Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="91e37-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="91e37-105">Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, для интеграции приложений управляемых API EWS с той же моделью проверки подлинности, что и для REST API Office 365.</span><span class="sxs-lookup"><span data-stu-id="91e37-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications with the same authentication model used by the Office 365 REST APIs.</span></span> <span data-ttu-id="91e37-106">Чтобы использовать OAuth с вашим приложением, необходимо выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="91e37-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="91e37-107">[Зарегистрируйте свое приложение](#bk_register) с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="91e37-107">[Register your application](#bk_register) with Azure Active Directory.</span></span> 
    
2. <span data-ttu-id="91e37-108">[Добавьте код, чтобы получить маркер проверки](#bk_getToken) подлинности для получения маркера проверки подлинности с сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="91e37-108">[Add code to get an authentication token](#bk_getToken) to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="91e37-109">[Добавьте маркер проверки подлинности в](#bk_useToken) отправляемые вами запросы EWS.</span><span class="sxs-lookup"><span data-stu-id="91e37-109">[Add an authentication token to EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="91e37-110">Проверка подлинности OAuth для EWS доступна только в Exchange в составе Office 365.</span><span class="sxs-lookup"><span data-stu-id="91e37-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="91e37-111">Приложениям EWS требуется разрешение "полный доступ к почтовому ящику пользователя".</span><span class="sxs-lookup"><span data-stu-id="91e37-111">EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="91e37-112">Чтобы использовать код, описанный в этой статье, вам потребуется доступ к следующим программам:</span><span class="sxs-lookup"><span data-stu-id="91e37-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="91e37-113">[Учетная запись разработчика Office 365](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span><span class="sxs-lookup"><span data-stu-id="91e37-113">An [Office 365 developer account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span></span> <span data-ttu-id="91e37-114">Для тестирования приложения можно использовать пробную учетную запись.</span><span class="sxs-lookup"><span data-stu-id="91e37-114">You can use a trial account to test your application.</span></span>
    
- <span data-ttu-id="91e37-115">[Библиотека проверки подлинности Azure AD для .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="91e37-115">The [Azure AD Authentication Library for .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>
    
- <span data-ttu-id="91e37-116">[Управляемый API EWS](https://github.com/officedev/ews-managed-api.aspx).</span><span class="sxs-lookup"><span data-stu-id="91e37-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx).</span></span>

<span data-ttu-id="91e37-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="91e37-117"><a name="bk_register"> </a></span></span>

## <a name="register-your-application"></a><span data-ttu-id="91e37-118">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="91e37-118">Register your application</span></span>

<span data-ttu-id="91e37-119">Чтобы использовать OAuth, приложение должно иметь идентификатор клиента и URI приложения, который идентифицирует приложение.</span><span class="sxs-lookup"><span data-stu-id="91e37-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="91e37-120">Если вы еще не зарегистрировали приложение с помощью служб Azure Active Directory, вам потребуется вручную добавить свое приложение, выполнив действия, описанные в статье [Регистрация приложения](https://apps.dev.microsoft.com/#/appList).</span><span class="sxs-lookup"><span data-stu-id="91e37-120">If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps at [Register your app](https://apps.dev.microsoft.com/#/appList).</span></span>

<span data-ttu-id="91e37-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="91e37-121"><a name="bk_getToken"> </a></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="91e37-122">Добавление кода для получения маркера проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="91e37-122">Add code to get an authentication token</span></span>

<span data-ttu-id="91e37-123">Библиотека проверки подлинности Azure AD для .NET упрощает извлечение маркера проверки подлинности из Azure Active Directory, чтобы можно было использовать маркер в приложении.</span><span class="sxs-lookup"><span data-stu-id="91e37-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.</span></span> <span data-ttu-id="91e37-124">Для получения маркера необходимо предоставить четыре фрагмента данных:</span><span class="sxs-lookup"><span data-stu-id="91e37-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="91e37-125">Универсальный код ресурса (URI) сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="91e37-125">The URI of the token server.</span></span> <span data-ttu-id="91e37-126">Сервер маркеров — это **центр** , проверяющий подлинность пользователя и возвращающий маркер, который приложение может использовать для доступа к EWS.</span><span class="sxs-lookup"><span data-stu-id="91e37-126">The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="91e37-127">Идентификатор клиента приложения, созданный при регистрации приложения с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="91e37-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="91e37-128">URI клиента приложения, созданный при регистрации приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="91e37-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="91e37-129">Универсальный код ресурса (URI) сервера EWS и URI конечной точки EWS.</span><span class="sxs-lookup"><span data-stu-id="91e37-129">The URI of the EWS server and the URI of the EWS endpoint.</span></span> <span data-ttu-id="91e37-130">Для Exchange в составе Office 365 это будет быть `https://<server name>/ews/exchange.asmx`.</span><span class="sxs-lookup"><span data-stu-id="91e37-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="91e37-131">В приведенном ниже коде показано, как использовать библиотеку проверки подлинности Azure AD для получения маркера проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="91e37-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="91e37-132">Предполагается, что сведения, необходимые для выполнения запроса на проверку подлинности, хранятся в файле App. config приложения.</span><span class="sxs-lookup"><span data-stu-id="91e37-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="91e37-133">В этом примере не включается проверка ошибок, приведен [пример кода](#bk_codeSample) для полного кода.</span><span class="sxs-lookup"><span data-stu-id="91e37-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="91e37-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="91e37-134"><a name="bk_useToken"> </a></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="91e37-135">Добавление маркера проверки подлинности в запросы EWS</span><span class="sxs-lookup"><span data-stu-id="91e37-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="91e37-136">После получения объекта **аусентикатионресулт** можно использовать свойство **AccessToken** для получения маркера, выданного службой маркеров.</span><span class="sxs-lookup"><span data-stu-id="91e37-136">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="91e37-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="91e37-137"><a name="bk_codeSample"> </a></span></span>

## <a name="code-sample"></a><span data-ttu-id="91e37-138">Пример кода</span><span class="sxs-lookup"><span data-stu-id="91e37-138">Code sample</span></span>

<span data-ttu-id="91e37-139">Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth.</span><span class="sxs-lookup"><span data-stu-id="91e37-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
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

<span data-ttu-id="91e37-140">Для примера кода требуется файл App. config со следующими записями:</span><span class="sxs-lookup"><span data-stu-id="91e37-140">The sample code requires an App.config file with the following entries:</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="91e37-141">См. также</span><span class="sxs-lookup"><span data-stu-id="91e37-141">See also</span></span>

- [<span data-ttu-id="91e37-142">Проверка подлинности и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="91e37-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    

    

