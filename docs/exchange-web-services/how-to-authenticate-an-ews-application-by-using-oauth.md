---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth для приложений на основе API, управляемого EWS.
localization_priority: Priority
ms.openlocfilehash: 795cbcc3dd1c895850086ebf0e23da905c1c99b7
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254967"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Проверка подлинности приложения EWS с помощью OAuth
<!-- markdownlint-enable MD025 -->

Узнайте, как использовать проверку подлинности OAuth для приложений на основе API, управляемого EWS.

Службу проверки подлинности OAuth, предоставляемую Azure Active Directory, можно использовать для обеспечения доступа к Exchange Online в Office 365 приложениям на основе API, управляемого EWS. Чтобы использовать OAuth с приложением, необходимо выполнить следующие действия.

1. [Регистрация приложения](#register-your-application) в Azure Active Directory.

2. [Добавление кода для получения токена проверки подлинности](#add-code-to-get-an-authentication-token) от сервера токенов.

3. [Добавление токена проверки подлинности в запросы EWS](#add-an-authentication-token-to-ews-requests), которые вы отправляете.

> [!NOTE]
> Проверка подлинности OAuth для EWS доступна в Exchange только в составе Office 365. Приложения EWS, использующие OAuth, необходимо зарегистрировать в Azure Active Directory.

Чтобы использовать код, приведенный в этой статье, необходимо иметь доступ к следующему:

- учетной записи Office 365 с почтовым ящиком Exchange Online. Если у вас нет учетной записи Office 365, вы можете получить бесплатную подписку на Office 365, [зарегистрировавшись в программе для разработчиков Office 365](https://developer.microsoft.com/office/dev-program);

- [библиотеке проверки подлинности Майкрософт для .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet);

- [API, управляемому EWS](https://github.com/officedev/ews-managed-api).


Существует два типа разрешений OAuth, которые можно использовать для доступа к API, управляемому EWS, в Exchange Online. Перед тем как приступить к выполнению описанных в руководстве действий, нужно выбрать конкретный тип разрешения.

* **Делегированные разрешения** используются в приложениях, предусматривающих вход пользователя. Для таких приложений пользователь или администратор соглашается предоставить разрешения, запрашиваемые приложением. Приложение при вызове API может действовать от имени выполнившего вход пользователя. 
* **Разрешения приложений** используются приложениями, не требующими от пользователя выполнения входа (например, фоновыми службами и управляющими программами, которые имеют доступ к нескольким почтовым ящикам).

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно иметь ИД приложения, выпущенный Azure Active Directory. В этом руководстве предполагается, что приложение является консольным, поэтому необходимо зарегистрировать приложение в качестве общедоступного клиента с помощью Azure Active Directory.

1. Откройте браузер и перейдите в [Центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите с помощью **личной учетной записи** (т.е. учетной записи Майкрософт) или **рабочей или учебной учетной записи**.

1. Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление**.

1. Выберите **Новая регистрация**. На странице **Регистрация приложения** задайте необходимые значения следующим образом.

    - Задайте понятное **Название** для своего приложения.
    - Настройте **Поддерживаемые типы учетных записей**, чтобы выбрать подходящий вариант.
    - В раскрывающемся списке **URI перенаправления** выберите **Общедоступный клиент (мобильный и классический)** и задайте для него значение `urn:ietf:wg:oauth:2.0:oob`.

1. Нажмите кнопку **Зарегистрировать**. На следующей странице скопируйте значение **ИД приложения (клиента)** и сохраните его, оно понадобится вам в дальнейшем.

1. Нажмите **Разрешения API** в области навигации слева в разделе **Управление**. 

1. Выберите **Добавить разрешение**. На странице **Запрос разрешений API** выберите **Exchange** в разделе **Поддерживаемые устаревшие API**. 

1. Чтобы использовать делегированные разрешения, выберите **Делегированные разрешения** а затем нажмите **EWS.AccessAsUser.All** в разделе **EWS**. Щелкните **Добавление разрешений** 

Чтобы использовать разрешения приложения, выполните следующие действия.

1. Нажмите **Разрешения приложения** а затем выберите **full_access_as_app**. Щелкните **Добавление разрешений**

1. Выберите **Предоставить согласие администратора для организации** и согласитесь с условиями. 

1. Нажмите **Сертификаты и секреты** в области навигации слева в разделе **Управление**. 

1. Выберите **Новый секрет клиента**, введите краткое описание и нажмите **Добавить**.

1. Скопируйте **Значение** добавленного секрета клиента и сохраните его. оно потребуется позже. 

## <a name="add-code-to-get-an-authentication-token"></a>Добавьте код для получения токена проверки подлинности

В следующих фрагментах кода показано, как с помощью библиотеки проверки подлинности Майкрософт можно получить токены проверки подлинности для делегированных разрешений и разрешений приложений. В этих фрагментах предполагается, что информация, необходимая для выполнения запроса на проверку подлинности, хранится в файле **App.config** приложения. В этих примерах не включена проверка ошибок. Полный код содержится в разделе [Примеры кода](#code-samples).

### <a name="delegated-permissions"></a>Делегированные разрешения

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

### <a name="application-permissions"></a>Разрешения приложений

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

### <a name="delegated-permissions"></a>Делегированные разрешения

Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании делегированных разрешений.

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

### <a name="application-permissions"></a>Разрешения приложений

Ниже приведен пример полного кода, в котором показано создание запроса EWS с проверкой подлинности OAuth при использовании разрешений приложения.

> [!NOTE]
> При использовании олицетворения необходимо всегда использовать заголовок запроса X-AnchorMailbox, который должен быть установлен в протоколе SMTP олицетворенного почтового ящика.

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

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "test@demotenant.onmicrosoft.com");

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
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>См. также

- [Проверка подлинности и EWS в Exchange](authentication-and-ews-in-exchange.md)
