---
title: Проверка подлинности подключения по протоколу IMAP, POP или SMTP с помощью OAuth
description: Узнайте, как использовать проверку подлинности OAuth с приложениями IMAP, POP и SMTP.
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: fbe4eaefc5befcc173096c9b8526adebf74a0aad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44438438"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a><span data-ttu-id="12527-103">Проверка подлинности подключения по протоколу IMAP, POP или SMTP с помощью OAuth</span><span class="sxs-lookup"><span data-stu-id="12527-103">Authenticate an IMAP, POP or SMTP connection using OAuth</span></span>

<span data-ttu-id="12527-104">Узнайте, как использовать проверку подлинности OAuth для подключения к протоколам IMAP, POP или SMTP и доступа к данным электронной почты для пользователей Office 365.</span><span class="sxs-lookup"><span data-stu-id="12527-104">Learn how to use OAuth authentication to connect with IMAP, POP or SMTP protocols and access email data for Office 365 users.</span></span>

> <span data-ttu-id="12527-105">OAuth2 поддержка протоколов IMAP, POP и SMTP, как описано ниже, не поддерживается для пользователей Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="12527-105">OAuth2 support for IMAP, POP, SMTP protocols as described below is not supported for Outlook.com users.</span></span>

<span data-ttu-id="12527-106">Если вы не знакомы с OAuth 2,0, начните с ознакомления с [обзором платформы Microsoft Identity Platform (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="12527-106">If you're not familiar with OAuth 2.0, start by reading the [Microsoft identity platform (v2.0) overview](/azure/active-directory/develop/v2-overview).</span></span> <span data-ttu-id="12527-107">В этом документе описываются различные компоненты платформы удостоверений Майкрософт, в том числе пакеты SDK.</span><span class="sxs-lookup"><span data-stu-id="12527-107">That document introduces you to different components of Microsoft identity platform, including SDKs.</span></span>

<span data-ttu-id="12527-108">Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, чтобы разрешить приложению подключаться с помощью протоколов IMAP, POP или SMTP для доступа к Exchange Online в Office 365.</span><span class="sxs-lookup"><span data-stu-id="12527-108">You can use the OAuth authentication service provided by Azure Active Directory to enable your application to connect with IMAP, POP or SMTP protocols to access Exchange Online in Office 365.</span></span> <span data-ttu-id="12527-109">Чтобы использовать OAuth с приложением, необходимо выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="12527-109">To use OAuth with your application you need to:</span></span>

1. <span data-ttu-id="12527-110">[Зарегистрируйте свое приложение](#register-your-application) с помощью Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12527-110">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="12527-111">[Настройте приложение](#configure-your-application) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12527-111">[Configure your application](#configure-your-application) in Azure Active Directory.</span></span>
1. <span data-ttu-id="12527-112">[Получение маркера доступа](#get-an-access-token) от сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="12527-112">[Get an access token](#get-an-access-token) from a token server.</span></span>
1. <span data-ttu-id="12527-113">[Проверка подлинности запросов на подключение](#authenticate-connection-requests) с помощью маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="12527-113">[Authenticate connection requests](#authenticate-connection-requests) with an access token.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="12527-114">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="12527-114">Register your application</span></span>

<span data-ttu-id="12527-115">Чтобы использовать OAuth, приложение должно быть зарегистрировано в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12527-115">To use OAuth, an application must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="12527-116">Следуйте инструкциям в статье [Регистрация приложения с помощью платформы удостоверений Майкрософт](/azure/active-directory/develop/quickstart-register-app) для создания нового приложения.</span><span class="sxs-lookup"><span data-stu-id="12527-116">Follow the instructions listed in [Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app) to create a new application.</span></span>

## <a name="configure-your-application"></a><span data-ttu-id="12527-117">Настройка приложения</span><span class="sxs-lookup"><span data-stu-id="12527-117">Configure your application</span></span>

<span data-ttu-id="12527-118">Следуйте инструкциям, приведенным в разделе [Настройка клиентского приложения для доступа к веб-API](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span><span class="sxs-lookup"><span data-stu-id="12527-118">Follow the instructions listed in [Configure a client application to access web APIs](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span></span>

<span data-ttu-id="12527-119">Не забудьте добавить одну или несколько следующих областей разрешений, соответствующих протоколам, с которыми вы хотите выполнить интеграцию.</span><span class="sxs-lookup"><span data-stu-id="12527-119">Make sure to add one or more of the following permission scopes that correspond to the protocols you would like to integrate with.</span></span> <span data-ttu-id="12527-120">В мастере **добавления разрешений** выберите **Microsoft Graph** , а затем **делегированные разрешения** , чтобы найти перечисленные ниже области разрешений.</span><span class="sxs-lookup"><span data-stu-id="12527-120">In the **Add a permission** wizard, select **Microsoft Graph** and then **Delegated permissions** to find the following permission scopes listed.</span></span>

| <span data-ttu-id="12527-121">Протокол</span><span class="sxs-lookup"><span data-stu-id="12527-121">Protocol</span></span>  | <span data-ttu-id="12527-122">Область разрешений</span><span class="sxs-lookup"><span data-stu-id="12527-122">Permission scope</span></span>        |
|-----------|-------------------------|
| <span data-ttu-id="12527-123">IMAP</span><span class="sxs-lookup"><span data-stu-id="12527-123">IMAP</span></span>      | `IMAP.AccessAsUser.All` |
| <span data-ttu-id="12527-124">POP</span><span class="sxs-lookup"><span data-stu-id="12527-124">POP</span></span>       | `POP.AccessAsUser.All`  |
| <span data-ttu-id="12527-125">ПРОВЕРКА ПОДЛИННОСТИ SMTP</span><span class="sxs-lookup"><span data-stu-id="12527-125">SMTP AUTH</span></span> | `SMTP.Send`             |

## <a name="get-an-access-token"></a><span data-ttu-id="12527-126">Получение токена доступа</span><span class="sxs-lookup"><span data-stu-id="12527-126">Get an access token</span></span>

<span data-ttu-id="12527-127">Вы можете использовать одну из наших [клиентских библиотек MSAL](/azure/active-directory/develop/msal-overview) для получения маркера доступа из клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="12527-127">You can use one of our [MSAL client libraries](/azure/active-directory/develop/msal-overview) to fetch an access token from your client application.</span></span>

<span data-ttu-id="12527-128">Кроме того, вы можете выбрать соответствующий поток из приведенного ниже списка и выполнить соответствующие действия, чтобы вызвать базовые API REST платформы идентификации и получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="12527-128">Alternatively, you can select an appropriate flow from the following list and follow the corresponding steps to call the underlying identity platform REST APIs and retrieve an access token.</span></span>

1. [<span data-ttu-id="12527-129">Потоки кода авторизации OAuth2</span><span class="sxs-lookup"><span data-stu-id="12527-129">OAuth2 authorization code flow</span></span>](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [<span data-ttu-id="12527-130">Процесс предоставления авторизации устройства OAuth2</span><span class="sxs-lookup"><span data-stu-id="12527-130">OAuth2 Device authorization grant flow</span></span>](/azure/active-directory/develop/v2-oauth2-device-code)

<span data-ttu-id="12527-131">Доступ OAuth к протоколам авторизации протокола IMAP, POP, SMTP с помощью OAuth2, потоки предоставления учетных данных клиента не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="12527-131">OAuth access to IMAP, POP, SMTP AUTH protocols via OAuth2 client credentials grant flow is not supported.</span></span> <span data-ttu-id="12527-132">Если для приложения требуется постоянный доступ ко всем почтовым ящикам в организации Microsoft 365, рекомендуется использовать API Microsoft Graph, которые позволяют доступ без пользователя, включать детализированные разрешения и предоставлять администраторам доступ к определенному набору почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="12527-132">If your application needs persistent access to all mailboxes in a Microsoft 365 organization, we recommend that you use the Microsoft Graph APIs which allow access without a user, enable granular permissions and let administrators scope such access to a specific set of mailboxes.</span></span>

<span data-ttu-id="12527-133">Обязательно укажите полные области, в том числе URL-адреса ресурсов Outlook, при авторизации приложения и запросе маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="12527-133">Make sure to specify the full scopes, including Outlook resource URLs, when authorizing your application and requesting an access token.</span></span>

| <span data-ttu-id="12527-134">Протокол</span><span class="sxs-lookup"><span data-stu-id="12527-134">Protocol</span></span>  | <span data-ttu-id="12527-135">Строка области разрешений</span><span class="sxs-lookup"><span data-stu-id="12527-135">Permission scope string</span></span> |
|-----------|-------------------------|
| <span data-ttu-id="12527-136">IMAP</span><span class="sxs-lookup"><span data-stu-id="12527-136">IMAP</span></span>      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| <span data-ttu-id="12527-137">POP</span><span class="sxs-lookup"><span data-stu-id="12527-137">POP</span></span>       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| <span data-ttu-id="12527-138">ПРОВЕРКА ПОДЛИННОСТИ SMTP</span><span class="sxs-lookup"><span data-stu-id="12527-138">SMTP AUTH</span></span> | `https://outlook.office.com/SMTP.Send`             |

<span data-ttu-id="12527-139">Кроме того, вы можете запросить [offline_accessную](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) область.</span><span class="sxs-lookup"><span data-stu-id="12527-139">In addition, you can request for [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) scope.</span></span> <span data-ttu-id="12527-140">Когда пользователь утверждает область offline_access, ваше приложение может получать маркеры обновления из конечной точки маркера платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="12527-140">When a user approves the offline_access scope, your app can receive refresh tokens from the Microsoft identity platform token endpoint.</span></span> <span data-ttu-id="12527-141">Маркеры обновления долгое время существованы.</span><span class="sxs-lookup"><span data-stu-id="12527-141">Refresh tokens are long-lived.</span></span> <span data-ttu-id="12527-142">Ваше приложение может получить новые маркеры доступа, срок действия которых истек.</span><span class="sxs-lookup"><span data-stu-id="12527-142">Your app can get new access tokens as older ones expire.</span></span>

## <a name="authenticate-connection-requests"></a><span data-ttu-id="12527-143">Проверка подлинности запросов на подключение</span><span class="sxs-lookup"><span data-stu-id="12527-143">Authenticate connection requests</span></span>

<span data-ttu-id="12527-144">Вы можете инициировать подключение к почтовым серверам Office 365 с помощью [параметров электронной почты IMAP и POP для Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span><span class="sxs-lookup"><span data-stu-id="12527-144">You can initiate a connection to Office 365 mail servers using the [IMAP and POP email settings for Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span></span>

### <a name="sasl-xoauth2"></a><span data-ttu-id="12527-145">SASL XOAUTH2</span><span class="sxs-lookup"><span data-stu-id="12527-145">SASL XOAUTH2</span></span>

<span data-ttu-id="12527-146">Для интеграции OAuth с приложением необходимо использовать формат SASL XOAUTH2 для кодирования и передачи маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="12527-146">OAuth integration with requires your application to use SASL XOAUTH2 format for encoding and transmitting the access token.</span></span> <span data-ttu-id="12527-147">SASL XOAUTH2 кодирует имя пользователя, маркер доступа вместе в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="12527-147">SASL XOAUTH2 encodes the username, access token together in the following format:</span></span>

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

<span data-ttu-id="12527-148">`^A`представляет **элемент управления**  +  **a** ( `%x01` ).</span><span class="sxs-lookup"><span data-stu-id="12527-148">`^A` represents a **Control** + **A** (`%x01`).</span></span>

<span data-ttu-id="12527-149">Например, для доступа `test@contoso.onmicrosoft.com` с помощью маркера доступа используется формат XOAUTH2 SASL `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` :</span><span class="sxs-lookup"><span data-stu-id="12527-149">For example, the SASL XOAUTH2 format to access `test@contoso.onmicrosoft.com` with access token `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` is:</span></span>

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

<span data-ttu-id="12527-150">После кодирования Base64 это преобразуется в следующую строку.</span><span class="sxs-lookup"><span data-stu-id="12527-150">After base64 encoding, this translates to the following string.</span></span> <span data-ttu-id="12527-151">Обратите внимание, что для удобочитаемости вставляются разрывы строк.</span><span class="sxs-lookup"><span data-stu-id="12527-151">Note that line breaks are inserted for readability.</span></span>

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="imap-protocol-exchange"></a><span data-ttu-id="12527-152">Обмен протоколами IMAP</span><span class="sxs-lookup"><span data-stu-id="12527-152">IMAP Protocol Exchange</span></span>

<span data-ttu-id="12527-153">Для проверки подлинности подключения к серверу IMAP клиент должен ответить на `AUTHENTICATE` команду в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="12527-153">To authenticate a IMAP server connection, the client will have to respond with an `AUTHENTICATE` command in the following format:</span></span>

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="12527-154">Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-154">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

<span data-ttu-id="12527-155">Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-155">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a><span data-ttu-id="12527-156">Обмен протоколом POP</span><span class="sxs-lookup"><span data-stu-id="12527-156">POP Protocol Exchange</span></span>

<span data-ttu-id="12527-157">Чтобы проверить подлинность подключения к серверу POP, клиенту необходимо `AUTH` разделить команду на две строки в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="12527-157">To authenticate a POP server connection, the client will have to respond with an `AUTH` command split into two lines in the following format:</span></span>    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

<span data-ttu-id="12527-158">Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-158">Sample client-server message exchange that results in an authentication success:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYX   
JlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0  
Q2cBAQ==    
S: +OK User successfully authenticated. 
[connection continues...]   
``` 

<span data-ttu-id="12527-159">Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-159">Sample client-server message exchange that results in an authentication failure:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a><span data-ttu-id="12527-160">Обмен протоколами SMTP</span><span class="sxs-lookup"><span data-stu-id="12527-160">SMTP Protocol Exchange</span></span>

<span data-ttu-id="12527-161">Чтобы проверить подлинность подключения SMTP-сервера, клиент должен ответить на `AUTH` команду в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="12527-161">To authenticate a SMTP server connection, the client will have to respond with an `AUTH` command in the following format:</span></span>

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="12527-162">Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-162">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 235 2.7.0 Authentication successful
[connection continues...]
```

<span data-ttu-id="12527-163">Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="12527-163">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a><span data-ttu-id="12527-164">См. также</span><span class="sxs-lookup"><span data-stu-id="12527-164">See also</span></span>

- [<span data-ttu-id="12527-165">Проверка подлинности и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="12527-165">Authentication and EWS in Exchange</span></span>](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [<span data-ttu-id="12527-166">IMAP, параметры подключения POP</span><span class="sxs-lookup"><span data-stu-id="12527-166">IMAP, POP Connection settings</span></span>](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [<span data-ttu-id="12527-167">Протокол доступа к сообщениям через Интернет</span><span class="sxs-lookup"><span data-stu-id="12527-167">Internet Message Access Protocol</span></span>](https://tools.ietf.org/html/rfc3501)
- [<span data-ttu-id="12527-168">Протокол Post Office</span><span class="sxs-lookup"><span data-stu-id="12527-168">Post Office Protocol</span></span>](https://tools.ietf.org/html/rfc1081)
- [<span data-ttu-id="12527-169">Расширение службы SMTP для проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="12527-169">SMTP Service extension for Authentication</span></span>](https://tools.ietf.org/html/rfc4954)
