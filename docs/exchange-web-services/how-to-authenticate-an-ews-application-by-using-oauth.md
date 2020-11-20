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
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Проверка подлинности приложения EWS с помощью OAuth
<!-- markdownlint-enable MD025 -->

Узнайте, как использовать проверку подлинности OAuth для приложений на основе API, управляемого EWS.

Службу проверки подлинности OAuth, предоставляемую Azure Active Directory, можно использовать для обеспечения доступа к Exchange Online в Office 365 приложениям на основе API, управляемого EWS. Чтобы использовать OAuth с приложением, необходимо выполнить следующие действия.

1. [Регистрация приложения](#register-your-application) в Azure Active Directory.
1. [Добавление кода для получения токена проверки подлинности](#add-code-to-get-an-authentication-token) от сервера токенов.
1. [Добавление токена проверки подлинности в запросы EWS](#add-an-authentication-token-to-ews-requests), которые вы отправляете.

> [!NOTE]
> Проверка подлинности OAuth для EWS доступна в Exchange Online только в составе Microsoft 365. Приложения EWS, использующие OAuth, необходимо зарегистрировать в Azure Active Directory.

Чтобы использовать код, приведенный в этой статье, необходимо иметь доступ к следующему:

- Учетной записи Microsoft 365 с почтовым ящиком Exchange Online. Если у вас нет учетной записи Microsoft 365, [зарегистрируйтесь в программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program), чтобы получить бесплатную подписку на Microsoft 365.
- [Библиотеке проверки подлинности Майкрософт для .NET](/dotnet/api/microsoft.identity.client).
- [API, управляемому EWS](https://github.com/officedev/ews-managed-api).

Существует два типа разрешений OAuth, которые можно использовать для доступа к API, управляемому EWS, в Exchange Online. Перед тем как приступить к выполнению описанных в руководстве действий, нужно выбрать конкретный тип разрешения.

- **Делегированные разрешения** используются в приложениях, предусматривающих вход пользователя. Для таких приложений пользователь или администратор соглашается предоставить разрешения, запрашиваемые приложением. Приложение при вызове API может действовать от имени выполнившего вход пользователя.
- **Разрешения приложений** используются приложениями, не требующими от пользователя выполнения входа (например, фоновыми службами и управляющими программами, которые имеют доступ к нескольким почтовым ящикам).

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно иметь ИД приложения, выпущенный Azure Active Directory. В этом руководстве предполагается, что приложение является консольным, поэтому необходимо зарегистрировать приложение в качестве общедоступного клиента с помощью Azure Active Directory. Зарегистрируйте приложение в центре администрирования Azure Active Directory или с помощью Microsoft Graph.

1. Откройте браузер и перейдите в [Центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите с помощью **личной учетной записи** (т.е. учетной записи Майкрософт) или **рабочей или учебной учетной записи**.

1. Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление**.

1. Выберите **Новая регистрация**. На странице **Регистрация приложения** задайте необходимые значения следующим образом.

    - Задайте понятное **Название** для своего приложения.
    - Настройте **Поддерживаемые типы учетных записей**, чтобы выбрать подходящий вариант.
    - В раскрывающемся списке **URI перенаправления** выберите **Общедоступный клиент (мобильный и классический)** и задайте для него значение `urn:ietf:wg:oauth:2.0:oob`.

1. Нажмите кнопку **Зарегистрировать**. На следующей странице скопируйте значение **ИД приложения (клиента)** и **ИД каталога (клиента)**, и сохраните, это понадобится в дальнейшем.

### <a name="configure-for-delegated-authentication"></a>Настройка делегированной проверки подлинности

Если приложение использует делегированную проверку подлинности, дополнительные настройки не требуются. Служба [Платформа удостоверений Майкрософт для разработчиков] позволяет приложениям динамически запрашивать разрешения, поэтому вам не нужно предварительно настраивать разрешения на регистрацию приложений. Тем не менее в некоторых ситуациях (например, [в потоке "от имени"](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) требуются предварительно настроенные разрешения. Чтобы предварительно настроить разрешения EWS, выполните действия ниже.

1. Нажмите **Манифест** в области навигации слева в разделе **Управление**.

1. Найдите свойство `requiredResourceAccess` в манифесте и добавьте его в квадратные скобки (`[]`):

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

1. Нажмите **Сохранить**.

1. Выберите **Разрешения API** в разделе **Управление**. Убедитесь в том, что разрешение **EWS.AccessAsUser.All** в списке.

### <a name="configure-for-app-only-authentication"></a>Настройка проверки подлинности только для приложений

Чтобы использовать разрешения приложения, выполните следующие действия.

1. Нажмите **Манифест** в области навигации слева в разделе **Управление**.

1. Найдите свойство `requiredResourceAccess` в манифесте и добавьте его в квадратные скобки (`[]`):

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

1. Нажмите **Сохранить**.

1. Выберите **Разрешения API** в разделе **Управление**. Убедитесь, что разрешение **full_access_as_app** в списке.

1. Выберите **Предоставить согласие администратора для организации** и согласитесь с условиями.

1. Нажмите **Сертификаты и секреты** в области навигации слева в разделе **Управление**.

1. Выберите **Новый секрет клиента**, введите краткое описание и нажмите **Добавить**.

1. Скопируйте **Значение** добавленного секрета клиента и сохраните его. оно потребуется позже.

## <a name="add-code-to-get-an-authentication-token"></a>Добавьте код для получения токена проверки подлинности

В следующих фрагментах кода показано, как с помощью библиотеки проверки подлинности Майкрософт можно получить токены проверки подлинности для делегированных разрешений и разрешений приложений. В этих фрагментах предполагается, что информация, необходимая для выполнения запроса на проверку подлинности, хранится в файле **App.config** приложения. В этих примерах не включена проверка ошибок. Полный код содержится в разделе [Примеры кода](#code-samples).

### <a name="get-a-token-with-delegated-auth"></a>Получение токена с помощью делегированной проверки подлинности

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

### <a name="get-a-token-with-app-only-auth"></a>Получение токена с помощью проверки подлинности только для приложений

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

## <a name="add-an-authentication-token-to-ews-requests"></a>Добавление токена проверки подлинности в запросы EWS

После получения объекта **AuthenticationResult** можно использовать свойство **AccessToken**, чтобы получить токен, выданный службой токенов.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Чтобы использовать разрешения приложения, вам также потребуется явно обозначить олицетворение того почтового ящика, к которому вы хотите получить доступ.

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Примеры кода

### <a name="delegated-authentication"></a>Делегированная проверка подлинности

Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании делегированной проверки подлинности.

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

### <a name="app-only-authentication"></a>Проверка подлинности только для приложений

Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании проверки подлинности только для приложений.

> [!NOTE]
> При использовании олицетворения необходимо всегда использовать заголовок запроса X-AnchorMailbox, который должен быть установлен в протоколе SMTP-адреса олицетворенного почтового ящика.

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

В примере кода в обоих случаях требуется наличие файла **App.config** со следующими записями.

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

## <a name="see-also"></a>См. также

- [Проверка подлинности и EWS в Exchange](authentication-and-ews-in-exchange.md)
