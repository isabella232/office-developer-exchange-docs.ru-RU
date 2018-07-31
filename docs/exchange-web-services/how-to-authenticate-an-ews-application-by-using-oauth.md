---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth с приложениями управляемый API веб-служб Exchange.
ms.openlocfilehash: 8b6a3fd72e42a36e31f261205292de28ef341270
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353583"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="223c8-103">Проверка подлинности приложения EWS с помощью OAuth</span><span class="sxs-lookup"><span data-stu-id="223c8-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="223c8-104">Узнайте, как использовать проверку подлинности OAuth с приложениями управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="223c8-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="223c8-105">Служба проверки подлинности OAuth, предоставляемая Azure Active Directory можно использовать для интеграции приложений управляемый API веб-служб Exchange с помощью той же модели проверки подлинности, используемых API-интерфейсы REST Office 365.</span><span class="sxs-lookup"><span data-stu-id="223c8-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications with the same authentication model used by the Office 365 REST APIs.</span></span> <span data-ttu-id="223c8-106">Для использования OAuth с приложением, необходимую для:</span><span class="sxs-lookup"><span data-stu-id="223c8-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="223c8-107">[Регистрация приложения](#bk_register) с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="223c8-107">[Register your application](#bk_register) with Azure Active Directory.</span></span> 
    
2. <span data-ttu-id="223c8-108">[Добавьте код для получения маркера проверки подлинности](#bk_getToken) для получения маркера проверки подлинности с сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="223c8-108">[Add code to get an authentication token](#bk_getToken) to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="223c8-109">[Добавить маркера проверки подлинности для запросов веб-служб Exchange](#bk_useToken) , можно отправить.</span><span class="sxs-lookup"><span data-stu-id="223c8-109">[Add an authentication token to EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="223c8-110">Проверка подлинности OAuth для веб-служб Exchange доступна только в составе Office 365 Exchange.</span><span class="sxs-lookup"><span data-stu-id="223c8-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="223c8-111">Приложения веб-служб Exchange требуется разрешение «Полный доступ к почтовому ящику пользователя».</span><span class="sxs-lookup"><span data-stu-id="223c8-111">EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="223c8-112">Чтобы использовать код в этой статье, необходимо иметь доступ к таким компонентам:</span><span class="sxs-lookup"><span data-stu-id="223c8-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="223c8-113">[Учетная запись разработчика Office 365](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span><span class="sxs-lookup"><span data-stu-id="223c8-113">An [Office 365 developer account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span></span> <span data-ttu-id="223c8-114">Пробной учетной записи можно использовать для тестирования приложения.</span><span class="sxs-lookup"><span data-stu-id="223c8-114">You can use a trial account to test your application.</span></span>
    
- <span data-ttu-id="223c8-115">[Библиотека проверки подлинности Azure AD для платформы .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="223c8-115">The [Azure AD Authentication Library for .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>
    
- <span data-ttu-id="223c8-116">[Управляемый API веб-служб Exchange](https://github.com/officedev/ews-managed-api.aspx).</span><span class="sxs-lookup"><span data-stu-id="223c8-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx).</span></span>

<span data-ttu-id="223c8-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="223c8-117"></span></span>

## <a name="register-your-application"></a><span data-ttu-id="223c8-118">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="223c8-118">Register your application</span></span>

<span data-ttu-id="223c8-119">Чтобы использовать OAuth, приложение должно иметь идентификатор клиента и URI, определяющая приложение, приложения.</span><span class="sxs-lookup"><span data-stu-id="223c8-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="223c8-120">Если вы еще не зарегистрирован приложения с помощью служб Azure Active Directory, то необходимо вручную добавить приложение, выполнив действия по [регистрации приложения](https://apps.dev.microsoft.com/#/appList).</span><span class="sxs-lookup"><span data-stu-id="223c8-120">If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps at [Register your app](https://apps.dev.microsoft.com/#/appList).</span></span>

<span data-ttu-id="223c8-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="223c8-121"></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="223c8-122">Добавление кода для получения маркера проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="223c8-122">Add code to get an authentication token</span></span>

<span data-ttu-id="223c8-123">Библиотеке проверка подлинности Azure AD для платформы .NET упрощает получение маркера проверки подлинности с Azure Active Directory, можно использовать маркер в приложении.</span><span class="sxs-lookup"><span data-stu-id="223c8-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.</span></span> <span data-ttu-id="223c8-124">Необходимо указать четыре фрагмента данных для получения маркера:</span><span class="sxs-lookup"><span data-stu-id="223c8-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="223c8-125">URI сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="223c8-125">The URI of the token server.</span></span> <span data-ttu-id="223c8-126">Сервер — это **центра сертификации** , который выполняет проверку подлинности пользователя и возвращает маркер, приложение может использовать для доступа к веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="223c8-126">The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="223c8-127">Идентификатор клиента приложения, созданные при регистрации приложения в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="223c8-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="223c8-128">URI, созданному при регистрации приложения с помощью Azure Active Directory клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="223c8-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="223c8-129">URI сервера веб-служб Exchange и URI конечной точки веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="223c8-129">The URI of the EWS server and the URI of the EWS endpoint.</span></span> <span data-ttu-id="223c8-130">Для Exchange в составе Office 365, это будет `https://<server name>/ews/exchange.asmx`.</span><span class="sxs-lookup"><span data-stu-id="223c8-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="223c8-131">Приведенный ниже код показано, как использовать библиотеку проверка подлинности Azure AD для получения маркера проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="223c8-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="223c8-132">Предполагается, что сведения, необходимые для выполнения запроса проверки подлинности хранится в файле App.config приложения.</span><span class="sxs-lookup"><span data-stu-id="223c8-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="223c8-133">В этом примере не включают проверки ошибок, просмотрите [образец кода](#bk_codeSample) для выполнения кода.</span><span class="sxs-lookup"><span data-stu-id="223c8-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="223c8-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="223c8-134"></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="223c8-135">Добавление маркера проверки подлинности для запросов веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="223c8-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="223c8-136">После получения объекта **AuthenticationResult** можно использовать свойство **AccessToken** для получения маркера, выдаваемого службой маркеров.</span><span class="sxs-lookup"><span data-stu-id="223c8-136">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="223c8-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="223c8-137"></span></span>

## <a name="code-sample"></a><span data-ttu-id="223c8-138">Пример кода</span><span class="sxs-lookup"><span data-stu-id="223c8-138">Code sample</span></span>

<span data-ttu-id="223c8-139">Ниже приведен полный пример кода, в котором показывается делает запрос на проверку подлинности OAuth веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="223c8-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
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

<span data-ttu-id="223c8-140">Пример кода требует файле App.config с помощью следующие записи:</span><span class="sxs-lookup"><span data-stu-id="223c8-140">The sample code requires an App.config file with the following entries:</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="223c8-141">См. также</span><span class="sxs-lookup"><span data-stu-id="223c8-141">See also</span></span>

- [<span data-ttu-id="223c8-142">Проверка подлинности и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="223c8-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    

    

