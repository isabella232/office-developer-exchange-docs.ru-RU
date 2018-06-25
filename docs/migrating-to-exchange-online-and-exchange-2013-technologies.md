---
title: Переход на Exchange технологий
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Если вы переход с предыдущей версии Exchange, чтобы узнать, какие технологии разработки, поддерживаются в текущей версии продуктов и технологии для переноса в используйте сведения в этой статье.
ms.openlocfilehash: 82362b7bcdb79d6ca43603335d51a8bd8c1df239
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761284"
---
# <a name="migrating-to-exchange-technologies"></a>Переход на Exchange технологий

Если вы переход с предыдущей версии Exchange, чтобы узнать, какие технологии разработки, поддерживаются в текущей версии продуктов и технологии для переноса в используйте сведения в этой статье.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Определение доступности в текущей версии технологии

Используйте следующую таблицу для определения технологии разработки, поддерживает ли в Exchange Online или Exchange 2013. Технологии не поддерживается, в статье [Choose технологии разработки для переноса](#bk_choose).

<br/> 

**Технологии разработки Exchange и версий продукта**

|Технология|Office 365 и Exchange Online|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|
|[Обзор платформы Office 365 API-интерфейсы](http://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X   <br/> ||||
|[Управляемый API EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Веб-служб Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Почтовые приложения для Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |||
|[Объектная модель Outlook (OOM)](http://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Резервное копирование и восстановление](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X   <br/> |X   <br/> |X   <br/> |
|[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X   <br/> |X   <br/> |X   <br/> |
|Интерфейс служб Active Directory (ADSI)  <br/> ||||X   <br/> |
|Объекты данных совместной работы для Exchange (CDOEX)  <br/> ||||X   <br/> |
|Объекты данных совместной работы для Windows 2000 (CDOSYS)  <br/> ||||X   <br/> |
|Поставщик Exchange OLE DB (EXOLEDB)  <br/> ||||X   <br/> |
|Приемники событий хранилища Exchange  <br/> ||||X   <br/> |
|Добавочные изменения синхронизации (ICS)  <br/> ||||X   <br/> |
|Протокол Lightweight Directory Access Protocol (LDAP)  <br/> ||||X   <br/> |
|[Интерфейс Messaging API (MAPI)](http://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Настройка Outlook Web App  <br/> |||X   <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||X   <br/> |

<a name="bk_choose"> </a>

## <a name="choose-a-development-technology-to-migrate-to"></a>Выбор технологии разработки для переноса

Если технологии, используемые приложением не поддерживается или deemphasized в Exchange Online или Exchange 2013, используйте следующую таблицу, чтобы решить, какие технологии для переноса.
  
**Рекомендуется использовать технологию пути миграции**

|**Технология**|**Поддерживается в Office 365 и Exchange Online и Exchange 2013?**|**Перенос в**|**Дополнительные сведения**|
|:-----|:-----|:-----|:-----|
|РЕДАКТОР ADSI  <br/> |Да, но deemphasized <br/>|[Командная консоль Exchange](management/exchange-management-shell.md)<br/> |Нет.  <br/> |
|CDOEX  <br/> |Нет  <br/> |[Управляемый API или веб-служб Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API EWS и веб-служб Exchange можно получить доступ к одной хранилища Exchange, который предоставляет CDOEX. В отличие от клиентских приложений с помощью CDOEX можно запускать приложения веб-служб Exchange на локальный или удаленный компьютер.  <br/> |
|CDOEXM  <br/> |Нет <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Командная консоль Exchange команд элементов управления Exchange серверы, группы хранения, базы данных и пользователи просто более чем соответствующие CDOEXM API. Кроме того, можно легко переносить приложения CDOEXM команд командной консоли Exchange.  <br/> |
|CDOSYS<br/> |Нет<br/> |[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Используйте агенты транспорта для приложений на основе уведомлений, которые работают с версии Exchange, начиная с Exchange 2010.<br/><br/> CDOSYS включен в текущей версии Windows. Функциональные возможности в CDOSYS доступна в .NET Framework.  <br/> |
|CDOWF  <br/> |Нет  <br/> |[Windows Workflow Foundation (WWF)](http://msdn.microsoft.com/en-us/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |WWF можно использовать для создания приложений дополнительных рабочих процессов, которые работают с Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Нет  <br/> |[Управляемый API или веб-служб Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API EWS и веб-служб Exchange обеспечивают такой же доступ к хранилищу Exchange, который предоставляет ExOLEDB. В отличие от клиентских приложений с помощью ExOLEDB можно запускать приложения веб-служб Exchange на локальный или удаленный компьютер.  <br/> |
|ICS  <br/> |Да, но deemphasized  <br/> |Управляемый API или веб-служб Exchange<br/> |[Подписаться на уведомления](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) и [синхронизировать данные почтовых ящиков](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)можно использовать управляемый API EWS или веб-служб Exchange.  <br/> |
|LDAP  <br/> |Да, но deemphasized  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Нет.  <br/> |
|MAPI  <br/> |Да, но deemphasized  <br/> |Обзор Office 365 интерфейсы API платформы, управляемый API EWS веб-служб Exchange <br/> |Несмотря на то, что MAPI в настоящее время — это технология поддерживаемые разработки, в конечном счете имеется переработать приложений MAPI для использования новой технологии.<br/><br/>Если приложение MAPI выполняет простой чтение, запись и операции обновления на почты, календарь, или контактных объектов и целевых показателей Office 365, можно использовать [Интерфейсы API REST Office 365 для почты, календари и контакты](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Если вы используете локальную систему Exchange и требуется получить доступ к все свойства, которые могут получить доступ к MAPI, можно использовать управляемый API EWS или веб-служб Exchange и [Схематизированный свойства или расширенные свойства](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Примечание**: класс [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) предоставляет доступ к MAPI из управляемого интерфейса API веб-служб Exchange и элемент [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) предоставляет доступ к свойства MAPI из веб-служб Exchange.           |
|Настройка Outlook Web App  <br/> |Нет  <br/> |[Почтовые приложения](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Нет.  <br/> |
|Приемники событий хранилища  <br/> |Нет  <br/> |Управляемый API или веб-служб Exchange <br/> |[Подписаться на уведомления](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) и [синхронизировать данные почтовых ящиков](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)можно использовать управляемый API EWS или веб-служб Exchange.<br/><br/>Уведомления в веб-служб Exchange предоставляют такой же доступ к хранилищу Exchange, что полностью приемники событий хранилища. Набор средств Visual Studio можно использовать для упрощения разработки хранилища принять во внимание события клиентских приложений, использующих веб-служб Exchange.  <br/> |
|Потоковая передача по технологии резервного копирования и восстановления  <br/> |Нет  <br/> |[Модуль записи службы теневого копирования томов (VSS) тома](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Нет.  <br/> |
|Протокол WebDAV  <br/> |Нет  <br/> |Обзор платформы Office 365 API-интерфейсы, управляемый API EWS или веб-служб Exchange <br/> |Если приложение WebDAV выполняется простое чтение, запись и операции обновления электронной почты, календарь и контактные объекты и ориентация Office 365, использования [Office 365 API -интерфейсы REST для почты, календари и контакты](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>В противном случае, если вы используете локальную систему Exchange и требуется доступ к одной свойств в хранилище Exchange, WebDAV обеспечивает, с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.  <br/> |
|Уведомления о WebDAV  <br/> |Нет  <br/> |Управляемый API или веб-служб Exchange<br/> |Подписаться [на уведомления](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)можно использовать управляемый API EWS или веб-служб Exchange.  <br/> |
|Веб-форм  <br/> |Нет  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Переключитесь в ASP.NET и обновления приложений для доступа к сведениям почтовых ящиков и сервера с помощью веб-служб Exchange.  <br/> |
|Поставщики WMI  <br/> |Нет  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Нет.  <br/> |
   
## <a name="see-also"></a>См. также

- [Выбор API или технологий для разработки решений для Outlook](http://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
    

