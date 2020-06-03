---
title: Проверка подлинности приложения EWS с помощью OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.
localization_priority: Priority
ms.openlocfilehash: e2bcb339ddac51b888660b6f982a8377591b1a29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528253"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Проверка подлинности приложения EWS с помощью OAuth
<!-- markdownlint-enable MD025 -->

Узнайте, как использовать проверку подлинности OAuth с приложениями управляемого API EWS.

Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, чтобы разрешить приложениям управляемых API EWS получать доступ к Exchange Online в Office 365. Чтобы использовать OAuth с вашим приложением, необходимо выполнить следующие действия:

1. [Зарегистрируйте свое приложение](#register-your-application) с помощью Azure Active Directory.

2. [Добавьте код, чтобы получить маркер проверки](#add-code-to-get-an-authentication-token) подлинности для получения маркера проверки подлинности с сервера маркеров.

3. [Добавьте маркер проверки подлинности в](#add-an-authentication-token-to-ews-requests) отправляемые вами запросы EWS.

> [!NOTE]
> Проверка подлинности OAuth для EWS доступна только в Exchange в составе Office 365. Приложения EWS, использующие OAuth, должны быть зарегистрированы в Azure Active Directory.

Чтобы использовать код, описанный в этой статье, вам потребуется доступ к следующим программам:

- Учетная запись Office 365 с почтовым ящиком Exchange Online. Если у вас нет учетной записи Office 365, вы можете [зарегистрироваться в программе для разработчиков office 365](https://developer.microsoft.com/office/dev-program) , чтобы получить бесплатную подписку на Office 365.

- [Библиотека проверки подлинности (Майкрософт) для .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).

- [Управляемый API EWS](https://github.com/officedev/ews-managed-api).


Существует два типа разрешений OAuth, которые можно использовать для доступа к API EWS в Exchange Online. Прежде чем приступать к работе с учебником, необходимо выбрать определенный тип разрешений.

* **Делегированные разрешения** используются в приложениях, предусматривающих вход пользователя. Для этих приложений либо пользователь, либо администратор отправляет разрешения, которые приложение запрашивает и приложение может выполнять в качестве вошедшего пользователя при совершении вызовов API. 
* **Разрешения приложений** используются приложениями, которые запускаются без вошедшего пользователя; Например, приложения, которые запускаются как фоновые службы или управляющие программы и могут получать доступ к нескольким почтовым ящикам.

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно иметь идентификатор приложения, выданный Azure Active Directory. В этом руководстве предполагается, что приложение является консольным приложением, поэтому необходимо зарегистрировать приложение в качестве общедоступного клиента с Azure Active Directory.

1. Откройте браузер и перейдите в [Центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите с помощью **личной учетной записи** (т.е. учетной записи Майкрософт) или **рабочей или учебной учетной записи**.

1. Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление**.

1. Выберите **Новая регистрация**. На странице**Зарегистрировать приложение** задайте необходимые значения следующим образом.

    - Задайте в качестве **имени** понятное имя для своего приложения.
    - Установите для **поддерживаемых типов учетных записей** вариант, который имеет смысл для вашего сценария.
    - Для **URI перенаправления**измените раскрывающийся список на **общедоступный клиент (мобильный & Настольный)** и присвойте ему значение `urn:ietf:wg:oauth:2.0:oob` .

1. Нажмите кнопку **Зарегистрировать**. На следующей странице скопируйте значение **идентификатора Application (Client)** и сохраните его, он понадобится позже.

1. Выберите **разрешения API** в левой панели навигации в разделе **Manage (Управление**). 

1. Нажмите кнопку **Добавить разрешение**. На странице **разрешения API запроса** выберите **Exchange** в разделе **Поддерживаемые устаревшие API**. 

1. Чтобы использовать делегированные разрешения, выберите **делегированные разрешения** , а затем выберите **EWS. AccessAsUser. ALL** в **EWS**. Нажмите кнопку **Добавить разрешения**. 

Чтобы использовать разрешения приложения, выполните следующие дополнительные действия.

1. Выберите **разрешения приложения** , а затем выберите **full_access_as_app**. Нажмите кнопку **Добавить разрешения**.

1. Выберите **предоставить согласие администратора для Организации** и примите диалоговое окно согласия. 

1. Выберите **сертификаты & секреты** в левой панели навигации в разделе **Manage (Управление**). 

1. Выберите **новый секрет клиента**, введите краткое описание и нажмите кнопку **Добавить**.

1. Скопируйте **значение** только что добавленного секрета клиента и сохраните его, он понадобится позже. 

## <a name="add-code-to-get-an-authentication-token"></a>Добавление кода для получения маркера проверки подлинности

В следующих фрагментах кода показано, как использовать библиотеку проверки подлинности (Майкрософт) для получения маркеров проверки подлинности для делегированных разрешений и разрешений приложений. В этих фрагментах предполагается, что сведения, необходимые для выполнения запроса проверки подлинности, хранятся в файле **app. config** приложения. В этих примерах не включается проверка ошибок, приведенные в [примерах кода](#code-samples) для полного кода.

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

//Make the toekn request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a>Добавление маркера проверки подлинности в запросы EWS

После получения объекта **аусентикатионресулт** можно использовать свойство **AccessToken** для получения маркера, выданного службой маркеров.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Чтобы использовать разрешения приложения, вам также потребуется експликтли олицетворение почтового ящика, к которому нужно получить доступ. 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Примеры кода

### <a name="delegated-permissions"></a>Делегированные разрешения

Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth с использованием делегированных разрешений.

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

Ниже приведен полный пример кода, демонстрирующий выполнение запроса EWS с проверкой подлинности OAuth с помощью разрешений приложения.

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

В примере кода в обоих случаях требуется файл **app. config** со следующими записями:

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
