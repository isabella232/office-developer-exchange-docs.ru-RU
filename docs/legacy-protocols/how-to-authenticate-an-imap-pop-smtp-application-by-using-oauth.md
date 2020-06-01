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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438438"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Проверка подлинности подключения по протоколу IMAP, POP или SMTP с помощью OAuth

Узнайте, как использовать проверку подлинности OAuth для подключения к протоколам IMAP, POP или SMTP и доступа к данным электронной почты для пользователей Office 365.

> OAuth2 поддержка протоколов IMAP, POP и SMTP, как описано ниже, не поддерживается для пользователей Outlook.com.

Если вы не знакомы с OAuth 2,0, начните с ознакомления с [обзором платформы Microsoft Identity Platform (v 2.0)](/azure/active-directory/develop/v2-overview). В этом документе описываются различные компоненты платформы удостоверений Майкрософт, в том числе пакеты SDK.

Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, чтобы разрешить приложению подключаться с помощью протоколов IMAP, POP или SMTP для доступа к Exchange Online в Office 365. Чтобы использовать OAuth с приложением, необходимо выполнить следующие действия:

1. [Зарегистрируйте свое приложение](#register-your-application) с помощью Azure Active Directory.
1. [Настройте приложение](#configure-your-application) в Azure Active Directory.
1. [Получение маркера доступа](#get-an-access-token) от сервера маркеров.
1. [Проверка подлинности запросов на подключение](#authenticate-connection-requests) с помощью маркера доступа.

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно быть зарегистрировано в Azure Active Directory.

Следуйте инструкциям в статье [Регистрация приложения с помощью платформы удостоверений Майкрософт](/azure/active-directory/develop/quickstart-register-app) для создания нового приложения.

## <a name="configure-your-application"></a>Настройка приложения

Следуйте инструкциям, приведенным в разделе [Настройка клиентского приложения для доступа к веб-API](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)

Не забудьте добавить одну или несколько следующих областей разрешений, соответствующих протоколам, с которыми вы хотите выполнить интеграцию. В мастере **добавления разрешений** выберите **Microsoft Graph** , а затем **делегированные разрешения** , чтобы найти перечисленные ниже области разрешений.

| Протокол  | Область разрешений        |
|-----------|-------------------------|
| IMAP      | `IMAP.AccessAsUser.All` |
| POP       | `POP.AccessAsUser.All`  |
| ПРОВЕРКА ПОДЛИННОСТИ SMTP | `SMTP.Send`             |

## <a name="get-an-access-token"></a>Получение токена доступа

Вы можете использовать одну из наших [клиентских библиотек MSAL](/azure/active-directory/develop/msal-overview) для получения маркера доступа из клиентского приложения.

Кроме того, вы можете выбрать соответствующий поток из приведенного ниже списка и выполнить соответствующие действия, чтобы вызвать базовые API REST платформы идентификации и получить маркер доступа.

1. [Потоки кода авторизации OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Процесс предоставления авторизации устройства OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

Доступ OAuth к протоколам авторизации протокола IMAP, POP, SMTP с помощью OAuth2, потоки предоставления учетных данных клиента не поддерживаются. Если для приложения требуется постоянный доступ ко всем почтовым ящикам в организации Microsoft 365, рекомендуется использовать API Microsoft Graph, которые позволяют доступ без пользователя, включать детализированные разрешения и предоставлять администраторам доступ к определенному набору почтовых ящиков.

Обязательно укажите полные области, в том числе URL-адреса ресурсов Outlook, при авторизации приложения и запросе маркера доступа.

| Протокол  | Строка области разрешений |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| ПРОВЕРКА ПОДЛИННОСТИ SMTP | `https://outlook.office.com/SMTP.Send`             |

Кроме того, вы можете запросить [offline_accessную](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) область. Когда пользователь утверждает область offline_access, ваше приложение может получать маркеры обновления из конечной точки маркера платформы удостоверений Майкрософт. Маркеры обновления долгое время существованы. Ваше приложение может получить новые маркеры доступа, срок действия которых истек.

## <a name="authenticate-connection-requests"></a>Проверка подлинности запросов на подключение

Вы можете инициировать подключение к почтовым серверам Office 365 с помощью [параметров электронной почты IMAP и POP для Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

Для интеграции OAuth с приложением необходимо использовать формат SASL XOAUTH2 для кодирования и передачи маркера доступа. SASL XOAUTH2 кодирует имя пользователя, маркер доступа вместе в следующем формате:

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`представляет **элемент управления**  +  **a** ( `%x01` ).

Например, для доступа `test@contoso.onmicrosoft.com` с помощью маркера доступа используется формат XOAUTH2 SASL `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` :

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

После кодирования Base64 это преобразуется в следующую строку. Обратите внимание, что для удобочитаемости вставляются разрывы строк.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="imap-protocol-exchange"></a>Обмен протоколами IMAP

Для проверки подлинности подключения к серверу IMAP клиент должен ответить на `AUTHENTICATE` команду в следующем формате:

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Обмен протоколом POP

Чтобы проверить подлинность подключения к серверу POP, клиенту необходимо `AUTH` разделить команду на две строки в следующем формате:    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:    

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

Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Обмен протоколами SMTP

Чтобы проверить подлинность подключения SMTP-сервера, клиент должен ответить на `AUTH` команду в следующем формате:

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Пример обмена сообщениями между клиентом и сервером, что приводит к успеху проверки подлинности:

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

Пример обмена сообщениями клиент — сервер, что приводит к сбою проверки подлинности:

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a>См. также

- [Проверка подлинности и EWS в Exchange](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [IMAP, параметры подключения POP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Протокол доступа к сообщениям через Интернет](https://tools.ietf.org/html/rfc3501)
- [Протокол Post Office](https://tools.ietf.org/html/rfc1081)
- [Расширение службы SMTP для проверки подлинности](https://tools.ietf.org/html/rfc4954)
