---
title: Переход на технологии Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Если вы мигрируете из более ранней версии Exchange, используйте сведения в этой статье, чтобы узнать, какие технологии разработки поддерживаются в текущих версиях продуктов и в какие технологии перейти.
ms.openlocfilehash: 3885d6789cedf5de028b64a0658b336bd021b9ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527003"
---
# <a name="migrating-to-exchange-technologies"></a>Переход на технологии Exchange

Если вы мигрируете из более ранней версии Exchange, используйте сведения в этой статье, чтобы узнать, какие технологии разработки поддерживаются в текущих версиях продуктов и в какие технологии перейти.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Определите, доступна ли технология в текущих версиях

Используйте следующую таблицу, чтобы определить, поддерживается ли технология разработки в Exchange Online или Exchange 2019 г. Если технология не поддерживается, см. в этой ленте [Выберите технологию разработки, чтобы перейти на](#bk_choose).

<br/> 

**Exchange разработки и версии продуктов**

|Технология|Office 365 и Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Общие сведения о платформе API Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X²  <br/> |X¹ ²  <br/> ||
|[Управляемый API EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Веб-службы Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Почтовые приложения для Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Outlook Объектная модель (OOM)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Резервное копирование и восстановление](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Интерфейс службы Active Directory (ADSI)  <br/> ||||||X  <br/> |
|Объекты совместных данных для Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Объекты совместной работы Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Exchange Поставщик OLE DB (EXOLEDB)  <br/> ||||||X  <br/> |
|Приемники событий хранилища Exchange  <br/> ||||||X  <br/> |
|Добавочная синхронизация изменений (ICS)  <br/> ||||||X  <br/> |
|Протокол LDAP  <br/> ||||||X  <br/> |
|[API обмена сообщениями (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Outlook Web App настройки  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

API ¹REST и Graph API требуют накопительного обновления 3 для Exchange 2016 г.

Гибридные клиенты ²Only могут использовать API REST как для Office 365, так и для локального почтового ящика.

## <a name="choose-a-development-technology-to-migrate-to"></a>Выберите технологию разработки, чтобы перейти на

Если в 2013 году технология, используемая вашим приложением, не поддерживается или не Exchange Online или Exchange, используйте следующую таблицу, чтобы определить, в какую технологию перейти.
  
**Рекомендуемые пути миграции технологий**

|**Технология**|**Поддерживается Office 365, Exchange Online и Exchange 2019?**|**Миграция в**|**Дополнительные сведения**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |Да, но <br/>|[Командная консоль Exchange](management/exchange-management-shell.md)<br/> |Нет.  <br/> |
|CDOEX  <br/> |Нет  <br/> |[Управляемый API или EWS EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API и EWS EWS могут получать доступ к той же Exchange, что и CDOEX. В отличие от клиентских приложений, построенных с помощью CDOEX, можно запускать приложения EWS на локальном или удаленном компьютере.  <br/> |
|CDOEXM  <br/> |Нет <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Exchange Команда Management Shell управляет Exchange серверами, группами хранения, базами данных и пользователями более просто, чем соответствующие API CDOEXM. Кроме того, вы можете легко перенести свои приложения CDOEXM в Exchange командной оболочки управления.  <br/> |
|CDOSYS<br/> |Нет<br/> |[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Используйте транспортные агенты для приложений на основе уведомлений, которые работают с версиями Exchange начиная Exchange 2010 г.<br/><br/> CDOSYS включен в текущие версии Windows. Функции CDOSYS доступны в платформа .NET Framework.  <br/> |
|CDOWF  <br/> |Нет  <br/> |[Windows Фонд рабочего процесса (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Вы можете использовать WWF для создания расширенных приложений рабочего процесса, которые работают с Exchange 2007 г.   <br/> |
|ExOLEDB  <br/> |Нет  <br/> |[Управляемый API или EWS EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API и EWS EWS предоставляют такой же доступ к Exchange, который предоставляет ExOLEDB. В отличие от клиентских приложений, построенных с помощью ExOLEDB, можно запускать приложения EWS на локальном или удаленном компьютере.  <br/> |
|ICS  <br/> |Да, но  <br/> |Управляемый API или EWS EWS<br/> |Управляемый API или EWS можно использовать [](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) для подписки на уведомления и синхронизации данных [почтовых ящиков.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)  <br/> |
|LDAP  <br/> |Да, но  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Нет.  <br/> |
|MAPI  <br/> |Да, но  <br/> |Office 365 Обзор платформы API, управляемый API EWS, EWS <br/> |Хотя MAPI в настоящее время является поддерживаемой технологией разработки, в конечном итоге вам придется изменить свои приложения MAPI, чтобы использовать более новую технологию.<br/><br/>Если приложение MAPI выполняет простые операции чтения, записи и обновления в почтовых, календарных или контактных объектах и целевых объектах Office 365, Exchange 2019 или Exchange 2016 ², вы можете использовать [API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)rest Office 365 для почты, календарей и контактов .<br/><br/>Если вы ориентированы Exchange локально и вам необходимо получить доступ ко всем свойствам, к которым можно получить доступ MAPI, вы можете использовать управляемый API EWS или EWS и либо [schematized свойства,](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)либо расширенные свойства .<br/><br/>**ПРИМЕЧАНИЕ.** Класс [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) предоставляет доступ к MAPI из управляемого API EWS, а элемент [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) предоставляет доступ к свойствам MAPI из EWS.           |
|Outlook Web App настройки  <br/> |Нет  <br/> |[Почтовые приложения](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Нет.  <br/> |
|Раковины событий магазина  <br/> |Нет  <br/> |Управляемый API или EWS EWS <br/> |Управляемый API или EWS можно использовать [](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) для подписки на уведомления и синхронизации данных [почтовых ящиков.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)<br/><br/>Уведомления в EWS предоставляют одинаковый доступ к Exchange, который предоставляется в хранилище событий. Вы можете использовать Visual Studio, чтобы оптимизировать разработку клиентских приложений для хранения событий, которые используют EWS.  <br/> |
|Потоковое резервное копирование и восстановление  <br/> |Нет  <br/> |[Автор тома Shadow Copy Service (VSS)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Нет.  <br/> |
|WebDAV  <br/> |Нет  <br/> |Office 365 Обзор платформы API, управляемый API EWS или EWS <br/> |Если ваше приложение WebDAV выполняет простые операции чтения, записи и обновления объектов почты, календаря или контактов, и вы будете нацелить на Office 365, Exchange 2019 или Exchange 2016 г. ² можно использовать [API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)rest Office 365 для почты, календарей и контактов .<br/><br/>В противном случае, если вы Exchange локально и вам необходим доступ к тем же свойствам в Exchange магазине, который предоставляет WebDAV, используйте управляемый API EWS или EWS.  <br/> |
|Уведомления WebDAV  <br/> |Нет  <br/> |Управляемый API или EWS EWS<br/> |Для подписки на уведомления можно использовать управляемый API или EWS [EWS.](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)  <br/> |
|Веб-формы  <br/> |Нет  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Переключение ASP.NET и обновление приложений для доступа к данным почтовых ящиков и серверов с помощью EWS.  <br/> |
|Поставщики WMI  <br/> |Нет  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Нет.  <br/> |
   
API ¹REST и Graph API требуют накопительного обновления 3 для Exchange 2016 г.

Гибридные клиенты ²Only могут использовать API REST как для Office 365, так и для локального почтового ящика.

## <a name="see-also"></a>См. также

- [Выбор API или технологии для разработки решений для Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Требования к локальной архитектуре для REST API](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
