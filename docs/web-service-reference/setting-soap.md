---
title: Параметр (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: Элемент Setting представляет с помощью параметра должно быть возвращено.
ms.openlocfilehash: cb5b1d6ab2109b48810b96221b76c6b8fc9803ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835472"
---
# <a name="setting-soap"></a>Параметр (SOAP)

Элемент **Setting** представляет с помощью параметра должно быть возвращено. 
  
```XML
<Setting/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена параметров запрошенные конфигурации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для этого элемента — параметр конфигурации. В следующей таблице перечислены возможные параметры.
  
|**Параметр конфигурации**|**Описание**|
|:-----|:-----|
|UserDisplayName  <br/> |Отображаемое имя пользователя.  <br/> |
|UserDN  <br/> |Устаревшее различающееся имя пользователя.  <br/> |
|UserDeploymentId  <br/> |Развертывание идентификатор пользователя.  <br/> |
|InternalMailboxServer  <br/> |Полное доменное имя (FQDN) сервера почтовых ящиков.  <br/> |
|InternalRpcClientServer  <br/> |Полное доменное имя сервера клиентского RPC.  <br/> |
|InternalMailboxServerDN  <br/> |Устаревшее различающееся имя сервера почтовых ящиков.  <br/> |
|InternalEcpUrl  <br/> |Внутренний URL-адрес панели управления Exchange.  <br/> |
|InternalEcpVoicemailUrl  <br/> |Внутренний URL-адрес панели управления Exchange для настройки голосовой почты.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |Внутренний URL-адрес панели управления Exchange для подписок электронной почты.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |Внутренний URL-адрес панели управления Exchange для обмена текстовыми сообщениями.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |Внутренний URL-адрес панели управления Exchange для отчетов о доставке.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |Внутренний URL-адрес панели управления Exchange для RetentionPolicy тегов.  <br/> |
|InternalEcpPublishingUrl  <br/> |Внутренний URL-адрес панели управления Exchange для публикации.  <br/> |
|InternalEwsUrl  <br/> |Внутренний URL-адрес для веб-служб Exchange.  <br/> |
|InternalOABUrl  <br/> |Внутренний URL-адрес автономной адресной книги (OAB).  <br/> |
|InternalUMUrl  <br/> |Внутренний URL-адрес службы единой системы обмена сообщениями.  <br/> |
|InternalWebClientUrls  <br/> |Внутренние URL-адреса Exchange веб-клиент.  <br/> |
|MailboxDN  <br/> |Различающееся имя базы данных почтовых ящиков из почтового ящика пользователя.  <br/> |
|PublicFolderServer  <br/> |Имя сервера общих папок.  <br/> |
|ActiveDirectoryServer  <br/> |Имя сервера службы каталогов Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |Имя RPC через HTTP-сервера.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |Индикатор для ли RPC через HTTP-сервере требуется протокол SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Методы проверки подлинности, поддерживаемых приложением RPC через HTTP-сервера.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |Фрагмент URL-адреса панели управления Exchange для настройки голосовой почты.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |Фрагмент URL-адреса панели управления Exchange для подписок электронной почты.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |Фрагмент URL-адреса панели управления Exchange для обмена текстовыми сообщениями.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |Фрагмент URL-адреса панели управления Exchange для отчетов о доставке.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Фрагмент URL-адреса панели управления Exchange для RetentionPolicy тегов.  <br/> |
|EcpPublishingUrlFragment  <br/> |Фрагмент URL-адреса панели управления Exchange для публикации.  <br/> |
|ExternalEcpUrl  <br/> |Внешний URL-адрес панели управления Exchange.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |Внешний URL-адрес панели управления Exchange для настройки голосовой почты.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |Внешний URL-адрес панели управления Exchange для подписок электронной почты.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |Внешний URL-адрес панели управления Exchange для обмена текстовыми сообщениями.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |Внешний URL-адрес панели управления Exchange для отчетов о доставке.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |Внешний URL-адрес панели управления Exchange для RetentionPolicy тегов.  <br/> |
|ExternalEcpPublishingUrl  <br/> |Внешний URL-адрес панели управления Exchange для публикации.  <br/> |
|ExternalEwsUrl  <br/> |Внешний URL-адрес веб-служб Exchange.  <br/> |
|ExternalOABUrl  <br/> |Внешний URL-адрес автономной адресной книги.  <br/> |
|ExternalUMUrl  <br/> |Внешний URL-адрес службы единой системы обмена сообщениями.  <br/> |
|ExternalWebClientUrls  <br/> |Внешний URL-адресов Exchange веб-клиент.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Указывает, что включен общий доступ к организации нескольких.  <br/> |
|AlternateMailboxes  <br/> |Коллекции альтернативного почтовые ящики.  <br/> |
|CasVersion  <br/> |Версия сервера клиентского доступа, обслуживающих запрос (например, 14.XX. ГГГГ. ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Разделенный запятыми список версий схемы, поддерживаемых веб-служб Exchange. Значения версии схемы будет совпадать с значений перечисления **ExchangeServerVersion** .  <br/> |
|InternalPop3Connections  <br/> |Список параметров внутреннее соединение для подключения протокола POP3.  <br/> |
|ExternalPop3Connections  <br/> |Список параметров внешнего подключения для подключений протокола POP3.  <br/> |
|InternalImap4Connections  <br/> |Список параметров внутреннее соединение для подключения протокола IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |Список параметров внешнего подключения для подключений протокола IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |Список параметров внутреннее соединение для подключения SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |Список параметров внешнего подключения для подключения SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |Внутренний сервер исключительных подключение флаг. Если задать «Отключено» нажмите клиенты должны не подключаются через этот протокол.  <br/> |
|ExternalServerExclusiveConnect  <br/> |Внешний сервер исключительных подключение флаг. Если параметр имеет значение «На» нажмите клиентов следует подключение через этот протокол.  <br/> |
|ExchangeRpcUrl  <br/> |URL-адрес, который используется для удаленного вызова процедуры. Этот URL-адрес внутреннего сервера и не должен использоваться клиентами.  <br/> |
|ShowGalAsDefaultView  <br/> |Задает логическое значение, указывающее, является ли глобальный список адресов, отображаемые как в адресной книге. Текстовое значение «true» указывает, что глобальный список адресов для отображения по умолчанию. Текстовое значение «false» указывает, что список контактов, которые будут показаны.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |Автообнаружение основного SMTP-адреса для пользователя. Это адрес прокси-сервера вместо адреса электронной почты пользователя, если существует адрес прокси-сервера.  <br/> |
|InteropExternalEwsUrl  <br/> |Внешний URL-адрес конечной точки службы веб-сервера. Это URL-адрес сервера, который может выполнять почтовых ящиков, размещенных на сервере, для которого не веб-служб.  <br/> |
|ExternalEwsVersion  <br/> |Версия веб-сервера службы, которая предоставляет указанному запросу.  <br/> |
|InteropExternalEwsVersion  <br/> |Версия сервера InteropExternalEwsUrl с указанием.  <br/> |
|MobileMailboxPolicyInterop  <br/> |Параметры политики почтовых ящиков мобильных устройств.  <br/> |
|GroupingInformation  <br/> |Значение, используемое в сочетании с параметром ExternalEwsUrl для группировки нескольких почтовых ящиков вместе, чтобы [поддерживать сходства](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) при подписки на уведомления о.  <br/> |
|UserMSOnline  <br/> |Логическое значение, которое указывает почтовый ящик пользователя размещается ли в Exchange Online или Exchange Online в составе Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Логическое значение, указывающее, доступен ли почтовый ящик пользователя с помощью протокола MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

