---
title: Setting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: Элемент Setting представляет возвращаемую настройку конфигурации.
ms.openlocfilehash: 2e03bfacaf36676ee4687c148f3b08732a9f17b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539145"
---
# <a name="setting-soap"></a>Setting (SOAP)

Элемент **Setting** представляет возвращаемую настройку конфигурации. 
  
```XML
<Setting/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена параметров запрашиваемой конфигурации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для этого элемента — параметр конфигурации. В следующей таблице перечислены возможные параметры конфигурации.
  
|**Параметр конфигурации**|**Описание**|
|:-----|:-----|
|UserDisplayName  <br/> |Отображаемое имя пользователя.  <br/> |
|UserDN  <br/> |Устаревшее отличительное имя пользователя.  <br/> |
|UserDeploymentId  <br/> |Идентификатор развертывания пользователя.  <br/> |
|InternalMailboxServer  <br/> |Полное доменное имя (FQDN) сервера почтовых ящиков.  <br/> |
|InternalRpcClientServer  <br/> |Полное доменное имя клиентского сервера RPC.  <br/> |
|InternalMailboxServerDN  <br/> |Устаревшее отличительное имя сервера почтовых ящиков.  <br/> |
|InternalEcpUrl  <br/> |Внутренний URL-адрес панели Exchange управления.  <br/> |
|InternalEcpVoicemailUrl  <br/> |Внутренний URL-адрес панели Exchange для настройки голосовой почты.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |Внутренний URL-адрес панели Exchange для подписок электронной почты.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |Внутренний URL-адрес панели Exchange для текстовых сообщений.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |Внутренний URL-адрес панели Exchange для отчетов о доставке.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |Внутренний URL-адрес панели Exchange для тегов RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |Внутренний URL-адрес панели Exchange для публикации.  <br/> |
|InternalEwsUrl  <br/> |Внутренний URL-адрес Exchange веб-служб.  <br/> |
|InternalOABUrl  <br/> |Внутренний URL-адрес автономной адресной книги (OAB).  <br/> |
|InternalUMUrl  <br/> |Внутренний URL-адрес служб единой системы обмена сообщениями.  <br/> |
|InternalWebClientUrls  <br/> |Внутренние URL-адреса веб Exchange клиента.  <br/> |
|Почтовый ящикDN  <br/> |Отличительное имя базы данных почтовых ящиков почтового ящика пользователя.  <br/> |
|PublicFolderServer  <br/> |Имя сервера общедоступных папок.  <br/> |
|ActiveDirectoryServer  <br/> |Имя сервера Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |Имя RPC на http-сервере.  <br/> |
|ExternalMailboxServerRequiresSL  <br/> |Индикатор того, требуется ли RPC для http-сервера SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Методы проверки подлинности, поддерживаемые RPC на http-сервере.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |Фрагмент URL-адреса панели Exchange для настройки голосовой почты.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |Фрагмент URL-адреса панели Exchange для подписок электронной почты.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |Фрагмент URL-адреса панели Exchange для текстовых сообщений.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |Фрагмент URL-адреса панели Exchange для отчетов о доставке.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Фрагмент URL-адреса панели Exchange для тегов RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |Фрагмент URL-адреса панели Exchange для публикации.  <br/> |
|ExternalEcpUrl  <br/> |Внешний URL-адрес Exchange панели управления.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |Внешний URL-адрес панели Exchange для настройки голосовой почты.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |Внешний URL-адрес панели Exchange для подписки на электронную почту.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |Внешний URL-адрес панели Exchange для текстовых сообщений.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |Внешний URL-адрес панели Exchange для отчетов о доставке.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |Внешний URL-адрес панели Exchange для тегов retentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |Внешний URL-адрес панели Exchange для публикации.  <br/> |
|ExternalEwsUrl  <br/> |Внешний URL-адрес Exchange веб-служб.  <br/> |
|ExternalOABUrl  <br/> |Внешний URL-адрес OAB.  <br/> |
|ExternalUMUrl  <br/> |Внешний URL-адрес служб единой системы обмена сообщениями.  <br/> |
|ExternalWebClientUrls  <br/> |Внешние URL-адреса веб Exchange клиента.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Указывает, что меж организации общего доступа включен.  <br/> |
|Альтернативные почтовые ящики  <br/> |Коллекция альтернативных почтовых ящиков.  <br/> |
|CasVersion  <br/> |Версия сервера клиентского доступа, обслуживающий запрос (например, 14.XX.YYYYY). ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Разделенный запятой список версий схемы, поддерживаемых Exchange веб-службами. Значения версии схемы будут такие же, как и значения переоценки **ExchangeServerVersion.**  <br/> |
|InternalPop3Connections  <br/> |Список параметров внутреннего подключения для подключений протокола POP3.  <br/> |
|ExternalPop3Connections  <br/> |Список внешних параметров подключения для подключений протокола POP3.  <br/> |
|InternalImap4Connections  <br/> |Список параметров внутреннего подключения для подключений протокола IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |Список внешних параметров подключения для подключений протокола IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |Список параметров внутреннего подключения для подключений SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |Список внешних параметров подключения для подключений SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |Флажок подключения внутреннего сервера. Если заданной для "Off", клиенты не должны подключаться через этот протокол.  <br/> |
|ExternalServerExclusiveConnect  <br/> |Исключительный флаг подключения внешнего сервера. Если установлено "На", клиенты должны подключиться с помощью этого протокола.  <br/> |
|ExchangeRpcUrl  <br/> |URL-адрес, используемый для удаленных вызовов процедур. Этот URL-адрес является внутренним для сервера и не используется клиентами.  <br/> |
|ShowGalAsDefaultView  <br/> |Указывает значение Boolean, которое указывает, следует ли показывать GAL в качестве адресной книги. Текстовое значение "true" указывает, что GAL должен быть показан по умолчанию. Текстовое значение "false" указывает, что список контактов должен быть показан.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |Основной SMTP-адрес автооткрытия для пользователя. Это прокси-адрес вместо адреса электронной почты пользователя, если прокси-адрес существует.  <br/> |
|InteropExternalEwsUrl  <br/> |Внешний URL-адрес конечной точки веб-службы сервера. Это URL-адрес сервера, который может обслуживать почтовые ящики, на которые не имеются веб-службы.  <br/> |
|ExternalEwsVersion  <br/> |Версия сервера веб-служб, который доставляет указанный запрос.  <br/> |
|InteropExternalEwsVersion  <br/> |На это указывают версии сервера InteropExternalEwsUrl.  <br/> |
|MobileMailboxPolicyInterop  <br/> |Параметры политики мобильных почтовых ящиков.  <br/> |
|GroupingInformation  <br/> |Значение, используемее в сочетании с параметром ExternalEwsUrl [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) для группировки нескольких почтовых ящиков для сохранения сродства при подписке на уведомления.  <br/> |
|UserMSOnline  <br/> |Значение Boolean, которое указывает, является ли почтовый ящик пользователя Exchange Online или Exchange Online частью Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Значение Boolean, которое указывает, доступен ли почтовый ящик пользователя с помощью протокола MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

