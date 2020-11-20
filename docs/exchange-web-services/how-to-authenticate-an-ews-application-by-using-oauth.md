---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 11/19/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth для приложений на основе API, управляемого EWS.
localization_priority: Priority
ms.openlocfilehash: c52b254f14cadd287a709bb68f8464e7cfe1837a
ms.sourcegitcommit: 2d16ba247a8cb4b6c8ca9941cb079f75202aae1e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49356495"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="e4790-103">Проверка подлинности приложения EWS с помощью OAuth</span><span class="sxs-lookup"><span data-stu-id="e4790-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="e4790-104">Узнайте, как использовать проверку подлинности OAuth для приложений на основе API, управляемого EWS.</span><span class="sxs-lookup"><span data-stu-id="e4790-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="e4790-105">Службу проверки подлинности OAuth, предоставляемую Azure Active Directory, можно использовать для обеспечения доступа к Exchange Online в Office 365 приложениям на основе API, управляемого EWS.</span><span class="sxs-lookup"><span data-stu-id="e4790-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="e4790-106">Чтобы использовать OAuth с приложением, необходимо выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e4790-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="e4790-107">[Регистрация приложения](#register-your-application) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4790-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="e4790-108">[Добавление кода для получения токена проверки подлинности](#add-code-to-get-an-authentication-token) от сервера токенов.</span><span class="sxs-lookup"><span data-stu-id="e4790-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>
1. <span data-ttu-id="e4790-109">[Добавление токена проверки подлинности в запросы EWS](#add-an-authentication-token-to-ews-requests), которые вы отправляете.</span><span class="sxs-lookup"><span data-stu-id="e4790-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="e4790-110">Проверка подлинности OAuth для EWS доступна в Exchange Online только в составе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e4790-110">OAuth authentication for EWS is only available in Exchange Online as part of Microsoft 365.</span></span> <span data-ttu-id="e4790-111">Приложения EWS, использующие OAuth, необходимо зарегистрировать в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4790-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="e4790-112">Чтобы использовать код, приведенный в этой статье, необходимо иметь доступ к следующему:</span><span class="sxs-lookup"><span data-stu-id="e4790-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="e4790-113">Учетной записи Microsoft 365 с почтовым ящиком Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e4790-113">A Microsoft 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="e4790-114">Если у вас нет учетной записи Microsoft 365, [зарегистрируйтесь в программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program), чтобы получить бесплатную подписку на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e4790-114">If you do not have a Microsoft 365 account, you can [sign up for the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program) to get a free Microsoft 365 subscription.</span></span>
- <span data-ttu-id="e4790-115">[Библиотеке проверки подлинности Майкрософт для .NET](/dotnet/api/microsoft.identity.client).</span><span class="sxs-lookup"><span data-stu-id="e4790-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client).</span></span>
- <span data-ttu-id="e4790-116">[API, управляемому EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="e4790-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>

<span data-ttu-id="e4790-117">Существует два типа разрешений OAuth, которые можно использовать для доступа к API, управляемому EWS, в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e4790-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="e4790-118">Перед тем как приступить к выполнению описанных в руководстве действий, нужно выбрать конкретный тип разрешения.</span><span class="sxs-lookup"><span data-stu-id="e4790-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

- <span data-ttu-id="e4790-119">**Делегированные разрешения** используются в приложениях, предусматривающих вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4790-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="e4790-120">Для таких приложений пользователь или администратор соглашается предоставить разрешения, запрашиваемые приложением. Приложение при вызове API может действовать от имени выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4790-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span>
- <span data-ttu-id="e4790-121">**Разрешения приложений** используются приложениями, не требующими от пользователя выполнения входа (например, фоновыми службами и управляющими программами, которые имеют доступ к нескольким почтовым ящикам).</span><span class="sxs-lookup"><span data-stu-id="e4790-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="e4790-122">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e4790-122">Register your application</span></span>

<span data-ttu-id="e4790-123">Чтобы использовать OAuth, приложение должно иметь ИД приложения, выпущенный Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4790-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="e4790-124">В этом руководстве предполагается, что приложение является консольным, поэтому необходимо зарегистрировать приложение в качестве общедоступного клиента с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4790-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span> <span data-ttu-id="e4790-125">Зарегистрируйте приложение в центре администрирования Azure Active Directory или с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e4790-125">You can register an application in the Azure Active Directory admin center or by using Microsoft Graph.</span></span>

1. <span data-ttu-id="e4790-126">Откройте браузер и перейдите в [Центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите с помощью **личной учетной записи** (т.е. учетной записи Майкрософт) или **рабочей или учебной учетной записи**.</span><span class="sxs-lookup"><span data-stu-id="e4790-126">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="e4790-127">Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-127">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="e4790-128">Выберите **Новая регистрация**.</span><span class="sxs-lookup"><span data-stu-id="e4790-128">Select **New registration**.</span></span> <span data-ttu-id="e4790-129">На странице **Регистрация приложения** задайте необходимые значения следующим образом.</span><span class="sxs-lookup"><span data-stu-id="e4790-129">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="e4790-130">Задайте понятное **Название** для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="e4790-130">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="e4790-131">Настройте **Поддерживаемые типы учетных записей**, чтобы выбрать подходящий вариант.</span><span class="sxs-lookup"><span data-stu-id="e4790-131">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="e4790-132">В раскрывающемся списке **URI перенаправления** выберите **Общедоступный клиент (мобильный и классический)** и задайте для него значение `urn:ietf:wg:oauth:2.0:oob`.</span><span class="sxs-lookup"><span data-stu-id="e4790-132">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="e4790-133">Нажмите кнопку **Зарегистрировать**.</span><span class="sxs-lookup"><span data-stu-id="e4790-133">Choose **Register**.</span></span> <span data-ttu-id="e4790-134">На следующей странице скопируйте значение **ИД приложения (клиента)** и **ИД каталога (клиента)**, и сохраните, это понадобится в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="e4790-134">On the next page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them, you will need them later.</span></span>

### <a name="configure-for-delegated-authentication"></a><span data-ttu-id="e4790-135">Настройка делегированной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e4790-135">Configure for delegated authentication</span></span>

<span data-ttu-id="e4790-136">Если приложение использует делегированную проверку подлинности, дополнительные настройки не требуются.</span><span class="sxs-lookup"><span data-stu-id="e4790-136">If your application uses delegated authentication, no further configuration is required.</span></span> <span data-ttu-id="e4790-137">Служба [Платформа удостоверений Майкрософт для разработчиков] позволяет приложениям динамически запрашивать разрешения, поэтому вам не нужно предварительно настраивать разрешения на регистрацию приложений.</span><span class="sxs-lookup"><span data-stu-id="e4790-137">The [Microsoft identity platform] allows apps to request permissions dynamically, so you do not have to pre-configure permissions on the app registration.</span></span> <span data-ttu-id="e4790-138">Тем не менее в некоторых ситуациях (например, [в потоке "от имени"](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) требуются предварительно настроенные разрешения.</span><span class="sxs-lookup"><span data-stu-id="e4790-138">However, in some scenarios (like the [on-behalf-of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) pre-configuring permissions is required.</span></span> <span data-ttu-id="e4790-139">Чтобы предварительно настроить разрешения EWS, выполните действия ниже.</span><span class="sxs-lookup"><span data-stu-id="e4790-139">Use the following steps to pre-configure EWS permissions.</span></span>

1. <span data-ttu-id="e4790-140">Нажмите **Манифест** в области навигации слева в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-140">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="e4790-141">Найдите свойство `requiredResourceAccess` в манифесте и добавьте его в квадратные скобки (`[]`):</span><span class="sxs-lookup"><span data-stu-id="e4790-141">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "3b5f3d61-589b-4a3c-a359-5dd4b5ee5bd5",
                "type": "Scope"
            }
        ]
    }
    ```

1. <span data-ttu-id="e4790-142">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e4790-142">Select **Save**.</span></span>

1. <span data-ttu-id="e4790-143">Выберите **Разрешения API** в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-143">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="e4790-144">Убедитесь в том, что разрешение **EWS.AccessAsUser.All** в списке.</span><span class="sxs-lookup"><span data-stu-id="e4790-144">Confirm that the **EWS.AccessAsUser.All** permission is listed.</span></span>

### <a name="configure-for-app-only-authentication"></a><span data-ttu-id="e4790-145">Настройка проверки подлинности только для приложений</span><span class="sxs-lookup"><span data-stu-id="e4790-145">Configure for app-only authentication</span></span>

<span data-ttu-id="e4790-146">Чтобы использовать разрешения приложения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e4790-146">To use application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="e4790-147">Нажмите **Манифест** в области навигации слева в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-147">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="e4790-148">Найдите свойство `requiredResourceAccess` в манифесте и добавьте его в квадратные скобки (`[]`):</span><span class="sxs-lookup"><span data-stu-id="e4790-148">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "dc890d15-9560-4a4c-9b7f-a736ec74ec40",
                "type": "Role"
            }
        ]
    }
    ```

1. <span data-ttu-id="e4790-149">Нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="e4790-149">Select **Save**.</span></span>

1. <span data-ttu-id="e4790-150">Выберите **Разрешения API** в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-150">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="e4790-151">Убедитесь, что разрешение **full_access_as_app** в списке.</span><span class="sxs-lookup"><span data-stu-id="e4790-151">Confirm that the **full_access_as_app** permission is listed.</span></span>

1. <span data-ttu-id="e4790-152">Выберите **Предоставить согласие администратора для организации** и согласитесь с условиями.</span><span class="sxs-lookup"><span data-stu-id="e4790-152">Select **Grant admin consent for org** and accept the consent dialog.</span></span>

1. <span data-ttu-id="e4790-153">Нажмите **Сертификаты и секреты** в области навигации слева в разделе **Управление**.</span><span class="sxs-lookup"><span data-stu-id="e4790-153">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="e4790-154">Выберите **Новый секрет клиента**, введите краткое описание и нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="e4790-154">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="e4790-155">Скопируйте **Значение** добавленного секрета клиента и сохраните его. оно потребуется позже.</span><span class="sxs-lookup"><span data-stu-id="e4790-155">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="e4790-156">Добавьте код для получения токена проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e4790-156">Add code to get an authentication token</span></span>

<span data-ttu-id="e4790-157">В следующих фрагментах кода показано, как с помощью библиотеки проверки подлинности Майкрософт можно получить токены проверки подлинности для делегированных разрешений и разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="e4790-157">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="e4790-158">В этих фрагментах предполагается, что информация, необходимая для выполнения запроса на проверку подлинности, хранится в файле **App.config** приложения.</span><span class="sxs-lookup"><span data-stu-id="e4790-158">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="e4790-159">В этих примерах не включена проверка ошибок. Полный код содержится в разделе [Примеры кода](#code-samples).</span><span class="sxs-lookup"><span data-stu-id="e4790-159">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="get-a-token-with-delegated-auth"></a><span data-ttu-id="e4790-160">Получение токена с помощью делегированной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e4790-160">Get a token with delegated auth</span></span>

```cs
// Using Microsoft.Identity.Client 4.22.0
var pca = PublicClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a><span data-ttu-id="e4790-161">Получение токена с помощью проверки подлинности только для приложений</span><span class="sxs-lookup"><span data-stu-id="e4790-161">Get a token with app-only auth</span></span>

```cs
// Using Microsoft.Identity.Client 4.22.0
var cca = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
    .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

//Make the token request
var authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="e4790-162">Добавление токена проверки подлинности в запросы EWS</span><span class="sxs-lookup"><span data-stu-id="e4790-162">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="e4790-163">После получения объекта **AuthenticationResult** можно использовать свойство **AccessToken**, чтобы получить токен, выданный службой токенов.</span><span class="sxs-lookup"><span data-stu-id="e4790-163">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="e4790-164">Чтобы использовать разрешения приложения, вам также потребуется явно обозначить олицетворение того почтового ящика, к которому вы хотите получить доступ.</span><span class="sxs-lookup"><span data-stu-id="e4790-164">To use application permissions, you will also need to explicitly impersonate a mailbox that you would like to access.</span></span>

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="e4790-165">Примеры кода</span><span class="sxs-lookup"><span data-stu-id="e4790-165">Code samples</span></span>

### <a name="delegated-authentication"></a><span data-ttu-id="e4790-166">Делегированная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="e4790-166">Delegated authentication</span></span>

<span data-ttu-id="e4790-167">Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании делегированной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e4790-167">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using delegated authentication.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var pca = PublicClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .Build();

            var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

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
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

### <a name="app-only-authentication"></a><span data-ttu-id="e4790-168">Проверка подлинности только для приложений</span><span class="sxs-lookup"><span data-stu-id="e4790-168">App-only authentication</span></span>

<span data-ttu-id="e4790-169">Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании проверки подлинности только для приложений.</span><span class="sxs-lookup"><span data-stu-id="e4790-169">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using app-only authentication.</span></span>

> [!NOTE]
> <span data-ttu-id="e4790-170">При использовании олицетворения необходимо всегда использовать заголовок запроса X-AnchorMailbox, который должен быть установлен в протоколе SMTP-адреса олицетворенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e4790-170">When using impersonation you must always use the X-AnchorMailbox request header, which should be set to the SMTP address of the impersonated mailbox.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var cca = ConfidentialClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
                .Build();

            var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

            try
            {
                var authResult = await cca.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
                ewsClient.ImpersonatedUserId =
                    new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "meganb@contoso.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "meganb@contoso.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

<span data-ttu-id="e4790-171">В примере кода в обоих случаях требуется наличие файла **App.config** со следующими записями.</span><span class="sxs-lookup"><span data-stu-id="e4790-171">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- The tenant ID copied from your app registration -->
    <add key="tenantId" value="YOUR_TENANT_ID_HERE"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="e4790-172">См. также</span><span class="sxs-lookup"><span data-stu-id="e4790-172">See also</span></span>

- [<span data-ttu-id="e4790-173">Проверка подлинности и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e4790-173">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
