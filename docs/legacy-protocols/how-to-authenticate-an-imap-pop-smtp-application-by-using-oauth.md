---
title: Проверка подлинности подключения IMAP, POP или SMTP с помощью OAuth
description: Узнайте, как использовать проверку подлинности OAuth в приложениях IMAP, POP и SMTP.
author: svpsiva
ms.date: 07/08/2021
ms.audience: Developer
ms.openlocfilehash: 4a307a6e329d5320b2b304d17a78a61db6d111bd
ms.sourcegitcommit: 357b882a02e37b380a23b8a45b15f9c006a40b02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58764590"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Проверка подлинности подключения IMAP, POP или SMTP с помощью OAuth

Узнайте, как использовать проверку подлинности OAuth для подключения к протоколам IMAP, POP или SMTP и доступа к данным электронной почты для Office 365 пользователей.

> Поддержка OAuth2 протоколов IMAP, POP, SMTP, как описано ниже, поддерживается как для пользователей Microsoft 365 (включая Office в Интернете), так и для Outlook.com.

Если вы не знакомы с протоколом OAuth 2.0, начните с чтения протокола [OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols)в платформа удостоверений Майкрософт обзоре. Дополнительные сведения о либарисах проверки подлинности Майкрософт (MSAL), реализующих протокол OAuth 2.0 для проверки подлинности пользователей и доступа к безопасным API, см. в обзоре [MSAL.](/azure/active-directory/develop/msal-overview)

Вы можете использовать службу проверки подлинности OAuth, предоставляемую Azure Active Directory, чтобы позволить приложению подключаться к протоколам IMAP, POP или SMTP для доступа к Exchange Online в Office 365. Чтобы использовать OAuth с приложением, необходимо:

1. [Регистрация приложения](#register-your-application) в Azure Active Directory.
1. [Настройка приложения в](#configure-your-application) Azure Active Directory.
1. [Получите маркер доступа с](#get-an-access-token) сервера маркеров.
1. [Проверка подлинности запросов на подключение](#authenticate-connection-requests) с помощью маркера доступа.

## <a name="register-your-application"></a>Регистрация приложения

Чтобы использовать OAuth, приложение должно быть зарегистрировано в Azure Active Directory.

Следуйте инструкциям, перечисленным в [Списке](/azure/active-directory/develop/quickstart-register-app) приложения с платформа удостоверений Майкрософт создать новое приложение.

## <a name="get-an-access-token"></a>Получение токена доступа

Вы можете использовать одну из наших клиентских библиотек [MSAL](/azure/active-directory/develop/msal-overview) для получения маркера доступа из клиентского приложения.

Кроме того, вы можете выбрать соответствующий поток из следующего списка и следуйте соответствующим шагам, чтобы вызвать API-API платформы REST и получить маркер доступа.

1. [Поток кода авторизации OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Поток грантов на авторизацию устройств OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

Доступ OAuth к протоколам IMAP, POP, SMTP AUTH через поток клиентских учетных данных OAuth2 не поддерживается. Если вашему приложению необходим постоянный доступ ко всем почтовым ящикам в Microsoft 365 организации, рекомендуется использовать API Microsoft Graph, которые позволяют получить доступ без пользователя, включить гранулярные разрешения и разрешить администраторам использовать такой доступ к определенному набору почтовых ящиков.

Убедитесь, что при авторизации приложения и запросе маркера доступа укажите полные области, в том числе URL Outlook ресурсов.

| Протокол  | Строка область разрешений |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| SMTP AUTH | `https://outlook.office.com/SMTP.Send`             |

Кроме того, вы можете запросить [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) области. Когда пользователь утверждает область offline_access, ваше приложение может получать маркеры обновления из конечной точки платформа удостоверений Майкрософт маркера. Маркеры обновления являются длительными. Ваше приложение может получать новые маркеры доступа по мере истечения срока действия старых маркеров.

## <a name="authenticate-connection-requests"></a>Проверка подлинности запросов на подключение

Вы можете инициировать подключение к Office 365 почтовым серверам с помощью параметров электронной почты [IMAP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)и POP для Office 365 .

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

Интеграция OAuth с требует от приложения использования формата SASL XOAUTH2 для кодиации и передачи маркера доступа. SASL XOAUTH2 кодирует имя пользователя, маркер доступа вместе в следующем формате:

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`представляет **управление**  +  **A** ( `%x01` ).

Например, формат SASL XOAUTH2 для доступа `test@contoso.onmicrosoft.com` с маркером `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` доступа:

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

После кодирования base64 это переводится на следующую строку. Обратите внимание, что для читаемости вставляются разрывы строк.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Проверка подлинности SASL XOAUTH2 для общих почтовых ящиков в Office 365

В случае общего доступа к почтовым ящикам с помощью OAuth приложению необходимо получить маркер доступа от имени пользователя, но заменить поле userName в закодированной строке SASL XOAUTH2 на адрес электронной почты общего почтового ящика. 

### <a name="imap-protocol-exchange"></a>Протокол IMAP Exchange

Чтобы проверить подлинность подключения к серверу IMAP, клиент должен будет ответить командой `AUTHENTICATE` в следующем формате:

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Пример обмена сообщениями клиента и сервера, который приводит к успеху проверки подлинности:

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Пример обмена сообщениями клиента и сервера, который приводит к сбою проверки подлинности:

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Протокол POP Exchange

Чтобы проверить подлинность подключения к pop-серверу, клиент должен будет ответить командой, разделенной на две строки в `AUTH` следующем формате:    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Пример обмена сообщениями клиента и сервера, который приводит к успеху проверки подлинности:    

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

Пример обмена сообщениями клиента и сервера, который приводит к сбою проверки подлинности:    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Протокол SMTP Exchange

Чтобы проверить подлинность подключения smTP-сервера, клиент должен будет ответить командой `AUTH` в следующем формате:

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Пример обмена сообщениями клиента и сервера, который приводит к успеху проверки подлинности:

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

Пример обмена сообщениями клиента и сервера, который приводит к сбою проверки подлинности:

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
- [Параметры IMAP, pop Connection](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Протокол доступа к интернет-сообщениям](https://tools.ietf.org/html/rfc3501)
- [Протокол Office](https://tools.ietf.org/html/rfc1081)
- [Расширение службы SMTP для проверки подлинности](https://tools.ietf.org/html/rfc4954)
