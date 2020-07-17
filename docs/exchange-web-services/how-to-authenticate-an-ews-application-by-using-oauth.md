---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.
localization_priority: Priority
ms.openlocfilehash: 0375095faac918859354da026118ea4ccfd6792b
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012568"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="aa289-103">Проверка подлинности приложения EWS с помощью OAuth</span><span class="sxs-lookup"><span data-stu-id="aa289-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="aa289-104">Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="aa289-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="aa289-105">Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, чтобы разрешить приложениям управляемых API EWS получать доступ к Exchange Online в Office 365.</span><span class="sxs-lookup"><span data-stu-id="aa289-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="aa289-106">Чтобы использовать OAuth с вашим приложением, необходимо выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="aa289-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="aa289-107">[Зарегистрируйте свое приложение](#register-your-application) с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa289-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>

2. <span data-ttu-id="aa289-108">[Добавьте код, чтобы получить маркер проверки](#add-code-to-get-an-authentication-token) подлинности для получения маркера проверки подлинности с сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="aa289-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>

3. <span data-ttu-id="aa289-109">[Добавьте маркер проверки подлинности в](#add-an-authentication-token-to-ews-requests) отправляемые вами запросы EWS.</span><span class="sxs-lookup"><span data-stu-id="aa289-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="aa289-110">Проверка подлинности OAuth для EWS доступна только в Exchange в составе Office 365.</span><span class="sxs-lookup"><span data-stu-id="aa289-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="aa289-111">Приложения EWS, использующие OAuth, должны быть зарегистрированы в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa289-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="aa289-112">Чтобы использовать код, описанный в этой статье, вам потребуется доступ к следующим программам:</span><span class="sxs-lookup"><span data-stu-id="aa289-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="aa289-113">Учетная запись Office 365 с почтовым ящиком Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="aa289-113">An Office 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="aa289-114">Если у вас нет учетной записи Office 365, вы можете [зарегистрироваться в программе для разработчиков office 365](https://developer.microsoft.com/office/dev-program) , чтобы получить бесплатную подписку на Office 365.</span><span class="sxs-lookup"><span data-stu-id="aa289-114">If you do not have an Office 365 account, you can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

- <span data-ttu-id="aa289-115">[Библиотека проверки подлинности (Майкрософт) для .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span><span class="sxs-lookup"><span data-stu-id="aa289-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span></span>

- <span data-ttu-id="aa289-116">[Управляемый API EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="aa289-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>


<span data-ttu-id="aa289-117">Существует два типа разрешений OAuth, которые можно использовать для доступа к API EWS в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="aa289-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="aa289-118">Прежде чем приступать к работе с учебником, необходимо выбрать определенный тип разрешений.</span><span class="sxs-lookup"><span data-stu-id="aa289-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

* <span data-ttu-id="aa289-119">**Делегированные разрешения** используются в приложениях, предусматривающих вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa289-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="aa289-120">Для этих приложений либо пользователь, либо администратор отправляет разрешения, которые приложение запрашивает и приложение может выполнять в качестве вошедшего пользователя при совершении вызовов API.</span><span class="sxs-lookup"><span data-stu-id="aa289-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span> 
* <span data-ttu-id="aa289-121">**Разрешения приложений** используются приложениями, которые запускаются без вошедшего пользователя; Например, приложения, которые запускаются как фоновые службы или управляющие программы и могут получать доступ к нескольким почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="aa289-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="aa289-122">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="aa289-122">Register your application</span></span>

<span data-ttu-id="aa289-123">Чтобы использовать OAuth, приложение должно иметь идентификатор приложения, выданный Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa289-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="aa289-124">В этом руководстве предполагается, что приложение является консольным приложением, поэтому необходимо зарегистрировать приложение в качестве общедоступного клиента с Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa289-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span>

1. <span data-ttu-id="aa289-125">Откройте браузер и перейдите в [Центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите с помощью **личной учетной записи** (т.е. учетной записи Майкрософт) или **рабочей или учебной учетной записи**.</span><span class="sxs-lookup"><span data-stu-id="aa289-125">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="aa289-126">Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="aa289-126">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="aa289-127">Выберите **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="aa289-127">Select **New registration**.</span></span> <span data-ttu-id="aa289-128">На странице**Зарегистрировать приложение** задайте необходимые значения следующим образом.</span><span class="sxs-lookup"><span data-stu-id="aa289-128">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="aa289-129">Задайте в качестве **имени** понятное имя для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="aa289-129">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="aa289-130">Установите для **поддерживаемых типов учетных записей** вариант, который имеет смысл для вашего сценария.</span><span class="sxs-lookup"><span data-stu-id="aa289-130">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="aa289-131">Для **URI перенаправления**измените раскрывающийся список на **общедоступный клиент (мобильный & Настольный)** и присвойте ему значение `urn:ietf:wg:oauth:2.0:oob` .</span><span class="sxs-lookup"><span data-stu-id="aa289-131">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="aa289-132">Нажмите кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="aa289-132">Choose **Register**.</span></span> <span data-ttu-id="aa289-133">На следующей странице скопируйте значение **идентификатора Application (Client)** и сохраните его, он понадобится позже.</span><span class="sxs-lookup"><span data-stu-id="aa289-133">On the next page, copy the value of the **Application (client) ID** and save it, you will need it later.</span></span>

1. <span data-ttu-id="aa289-134">Выберите **разрешения API** в левой панели навигации в разделе **Manage (Управление**).</span><span class="sxs-lookup"><span data-stu-id="aa289-134">Select **API permissions** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="aa289-135">Нажмите кнопку **Добавить разрешение**.</span><span class="sxs-lookup"><span data-stu-id="aa289-135">Select **Add a permission**.</span></span> <span data-ttu-id="aa289-136">На странице **разрешения API запроса** выберите **Exchange** в разделе **Поддерживаемые устаревшие API**.</span><span class="sxs-lookup"><span data-stu-id="aa289-136">On the **Request API permissions** page, select **Exchange** under **Supported legacy APIs**.</span></span> 

1. <span data-ttu-id="aa289-137">Чтобы использовать делегированные разрешения, выберите **делегированные разрешения** , а затем выберите **EWS. AccessAsUser. ALL** в **EWS**.</span><span class="sxs-lookup"><span data-stu-id="aa289-137">To use Delegated permissions, select **Delegated permissions** and then select **EWS.AccessAsUser.All** under **EWS**.</span></span> <span data-ttu-id="aa289-138">Нажмите кнопку **Добавить разрешения**.</span><span class="sxs-lookup"><span data-stu-id="aa289-138">Click on **Add permissions**.</span></span> 

<span data-ttu-id="aa289-139">Чтобы использовать разрешения приложения, выполните следующие дополнительные действия.</span><span class="sxs-lookup"><span data-stu-id="aa289-139">To use Application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="aa289-140">Выберите **разрешения приложения** , а затем выберите **full_access_as_app**.</span><span class="sxs-lookup"><span data-stu-id="aa289-140">Select **Application permissions** and then select **full_access_as_app**.</span></span> <span data-ttu-id="aa289-141">Нажмите кнопку **Добавить разрешения**.</span><span class="sxs-lookup"><span data-stu-id="aa289-141">Click on **Add permissions**.</span></span>

1. <span data-ttu-id="aa289-142">Выберите **предоставить согласие администратора для Организации** и примите диалоговое окно согласия.</span><span class="sxs-lookup"><span data-stu-id="aa289-142">Select **Grant admin consent for org** and accept the consent dialog.</span></span> 

1. <span data-ttu-id="aa289-143">Выберите **сертификаты & секреты** в левой панели навигации в разделе **Manage (Управление**).</span><span class="sxs-lookup"><span data-stu-id="aa289-143">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="aa289-144">Выберите **новый секрет клиента**, введите краткое описание и нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="aa289-144">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="aa289-145">Скопируйте **значение** только что добавленного секрета клиента и сохраните его, он понадобится позже.</span><span class="sxs-lookup"><span data-stu-id="aa289-145">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span> 

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="aa289-146">Добавление кода для получения маркера проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="aa289-146">Add code to get an authentication token</span></span>

<span data-ttu-id="aa289-147">В следующих фрагментах кода показано, как использовать библиотеку проверки подлинности (Майкрософт) для получения маркеров проверки подлинности для делегированных разрешений и разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="aa289-147">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="aa289-148">В этих фрагментах предполагается, что сведения, необходимые для выполнения запроса проверки подлинности, хранятся в файле **App.config** приложения.</span><span class="sxs-lookup"><span data-stu-id="aa289-148">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="aa289-149">В этих примерах не включается проверка ошибок, приведенные в [примерах кода](#code-samples) для полного кода.</span><span class="sxs-lookup"><span data-stu-id="aa289-149">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="aa289-150">Делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="aa289-150">Delegated permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="application-permissions"></a><span data-ttu-id="aa289-151">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="aa289-151">Application permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var app = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"]).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/.default" };

//Make the token request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="aa289-152">Добавление маркера проверки подлинности в запросы EWS</span><span class="sxs-lookup"><span data-stu-id="aa289-152">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="aa289-153">После получения объекта **аусентикатионресулт** можно использовать свойство **AccessToken** для получения маркера, выданного службой маркеров.</span><span class="sxs-lookup"><span data-stu-id="aa289-153">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="aa289-154">Чтобы использовать разрешения приложения, вам также потребуется експликтли олицетворение почтового ящика, к которому нужно получить доступ.</span><span class="sxs-lookup"><span data-stu-id="aa289-154">To use Application permissions, you will also need to explictly impersonate a mailbox that you would like to access.</span></span> 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="aa289-155">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="aa289-155">Code samples</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="aa289-156">Делегированные разрешения</span><span class="sxs-lookup"><span data-stu-id="aa289-156">Delegated permissions</span></span>

<span data-ttu-id="aa289-157">Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth с использованием делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="aa289-157">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Delegated permissions.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }

        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

            try
            {
                // Make the interactive token request
                var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

### <a name="application-permissions"></a><span data-ttu-id="aa289-158">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="aa289-158">Application permissions</span></span>

<span data-ttu-id="aa289-159">Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="aa289-159">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Application permissions.</span></span>

```cs
using System;
using System.Configuration;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;

namespace ews_oauth_samples
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
        
        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var ewsScopes = new string[] { "https://outlook.office.com/.default" };

            var app = ConfidentialClientApplicationBuilder.Create(ConfigurationManager.AppSettings["appId"])
                .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .Build();

            AuthenticationResult result = null;

            try
            {
                // Make the interactive token request
                result = await app.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(result.AccessToken);

                //Impersonate the mailbox you'd like to access.
                ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach (var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

<span data-ttu-id="aa289-160">В примере кода в обоих случаях требуется файл **App.config** со следующими записями:</span><span class="sxs-lookup"><span data-stu-id="aa289-160">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="aa289-161">См. также</span><span class="sxs-lookup"><span data-stu-id="aa289-161">See also</span></span>

- [<span data-ttu-id="aa289-162">Проверка подлинности и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="aa289-162">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
