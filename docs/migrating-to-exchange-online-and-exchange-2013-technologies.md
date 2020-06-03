---
title: Переход на технологии Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Если вы выполняете миграцию с более ранней версии Exchange, используйте сведения из этой статьи, чтобы узнать, какие технологии разработки поддерживаются в текущих версиях продуктов, а также какую технологию перенести.
ms.openlocfilehash: d82f1b305fd1cc30e48cddbf9bf2981d3d829a5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459155"
---
# <a name="migrating-to-exchange-technologies"></a>Переход на технологии Exchange

Если вы выполняете миграцию с более ранней версии Exchange, используйте сведения из этой статьи, чтобы узнать, какие технологии разработки поддерживаются в текущих версиях продуктов, а также какую технологию перенести.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Определение доступности технологии в текущих версиях

Используйте приведенную ниже таблицу, чтобы определить, поддерживается ли технология разработки в Exchange Online или Exchange 2019. Если технология не поддерживается, ознакомьтесь со статьей [Выбор технологии разработки для переноса](#bk_choose).

<br/> 

**Технологии разработки и версии продуктов Exchange**

|Технологии|Office 365 и Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Общие сведения о платформе API Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X ²  <br/> |X ¹ ²  <br/> ||
|[Управляемый API EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Веб-службы Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Почтовые приложения для Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Объектная модель Outlook (некоторая)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Резервное копирование и восстановление](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Интерфейс службы Active Directory (ADSI)  <br/> ||||||X  <br/> |
|Объекты совместных данных для Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Объекты совместных данных для Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Поставщик OLE DB для Exchange (ЕКСОЛЕДБ)  <br/> ||||||X  <br/> |
|Приемники событий хранилища Exchange  <br/> ||||||X  <br/> |
|Добавочная синхронизация изменений (ICS)  <br/> ||||||X  <br/> |
|Протокол LDAP  <br/> ||||||X  <br/> |
|[API обмена сообщениями (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Настройка Outlook Web App  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Распределенная веб-разработка и управление версиями (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

для использования API REST REST и Graph API требуется накопительный пакет обновления 3 для Exchange 2016.

² только пользователи с гибридными средами могут воспользоваться преимуществами REST API для Office 365 и локальных почтовых ящиков.

## <a name="choose-a-development-technology-to-migrate-to"></a>Выбор технологии разработки для переноса в

Если технология, используемая приложением, не поддерживается или не будет выделяться в Exchange Online или Exchange 2013, используйте приведенную ниже таблицу, чтобы определить, на какую технологию необходимо перенести.
  
**Рекомендуемые пути переноса технологий**

|**Технологии**|**Поддерживается в Office 365, Exchange Online и Exchange 2019?**|**Миграция в**|**Дополнительные сведения**|
|:-----|:-----|:-----|:-----|
|ИНТЕРФЕЙСЫ  <br/> |Да, без выделения <br/>|[Командная консоль Exchange](management/exchange-management-shell.md)<br/> |Отсутствуют.  <br/> |
|CDOEX  <br/> |Нет  <br/> |[Управляемый API EWS или EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API EWS и EWS могут получать доступ к тому же хранилищу Exchange, которое предоставляет CDOEX. В отличие от клиентских приложений, созданных с помощью CDOEX, вы можете запускать приложения EWS на локальном или удаленном компьютере.  <br/> |
|кдоексм  <br/> |Нет <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Команды командной консоли Exchange управляют серверами Exchange, группами хранения, базами данных и пользователями проще, чем соответствующие API КДОЕКСМ. Кроме того, вы можете легко перенести приложения КДОЕКСМ в командную консоль Exchange.  <br/> |
|CDOSYS<br/> |Нет<br/> |[Агенты транспорта](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Используйте агенты транспорта для приложений на основе уведомлений, работающих с версиями Exchange, начиная с Exchange 2010.<br/><br/> CDOSYS включена в текущие версии Windows. Функции CDOSYS доступны в платформе .NET Framework.  <br/> |
|кдовф  <br/> |Нет  <br/> |[Windows Workflow Foundation (ВВФ)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Вы можете использовать ВВФ для создания сложных приложений рабочих процессов, работающих с Exchange 2007.   <br/> |
|ексоледб  <br/> |Нет  <br/> |[Управляемый API EWS или EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Управляемый API EWS и EWS предоставляют такой же доступ к хранилищу Exchange, предоставляемому Ексоледб. В отличие от клиентских приложений, созданных с помощью Ексоледб, вы можете запускать приложения EWS на локальном или удаленном компьютере.  <br/> |
|ICS  <br/> |Да, без выделения  <br/> |Управляемый API EWS или EWS<br/> |Вы можете [подписаться на уведомления](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) и [синхронизировать данные почтовых ящиков](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)с помощью управляемого API EWS или EWS.  <br/> |
|LDAP  <br/> |Да, без выделения  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Отсутствуют.  <br/> |
|MAPI  <br/> |Да, без выделения  <br/> |Общие сведения о платформе API Office 365, управляемый API EWS, EWS <br/> |Несмотря на то, что в настоящее время поддерживается технология разработки для MAPI, потребуется перерабатывать приложения MAPI, чтобы использовать новую технологию.<br/><br/>Если приложение MAPI выполняет простые операции чтения, записи и обновления для электронной почты, календаря или контактных объектов, а также целевых объектов Office 365, Exchange 2019 ² или Exchange 2016 ¹ ², вы можете использовать [REST API Office 365 для почты, календарей и контактов](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Если вы нацелены на локальную среду Exchange и вам нужно получить доступ ко всем свойствам, к которым имеет доступ MAPI, вы можете использовать управляемый API EWS или EWS и [Свойства схематизированные или расширенные свойства](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Note**: класс [екстендедпропертидефинитион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) предоставляет доступ к MAPI из управляемого API EWS, а элемент [екстендедфиелдури](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) предоставляет доступ к свойствам MAPI из EWS.           |
|Настройка Outlook Web App  <br/> |Нет  <br/> |[Почтовые приложения](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Отсутствуют.  <br/> |
|Приемники событий хранилища  <br/> |Нет  <br/> |Управляемый API EWS или EWS <br/> |Вы можете [подписаться на уведомления](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) и [синхронизировать данные почтовых ящиков](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)с помощью управляемого API EWS или EWS.<br/><br/>Уведомления в службах EWS обеспечивают такой же доступ к хранилищу Exchange, в котором хранятся приемники событий. С помощью Visual Studio можно упростить разработку клиентских приложений, поддерживающих события, которые используют EWS.  <br/> |
|Потоковая Архивация и восстановление  <br/> |Нет  <br/> |[Средство записи службы теневого копирования томов (VSS)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Отсутствуют.  <br/> |
|Протокол  <br/> |Нет  <br/> |Общие сведения о платформе API Office 365, управляемый API EWS или EWS <br/> |Если приложение WebDAV выполняет простые операции чтения, записи и обновления для объектов mail, Calendar и Contact, и вы будете нацелены на Office 365, Exchange 2019 ² или Exchange 2016 ¹ ², вы можете использовать [REST API Office 365 для почты, календарей и контактов](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>В противном случае, если вы нацелены на локальную среду Exchange и вам требуется доступ к тем же свойствам в хранилище Exchange, которое предоставляет WebDAV, используйте управляемый API EWS или EWS.  <br/> |
|Уведомления WebDAV  <br/> |Нет  <br/> |Управляемый API EWS или EWS<br/> |Вы можете [подписаться на уведомления с](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)помощью управляемого API EWS или EWS.  <br/> |
|Веб-формы  <br/> |Нет  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Переключитесь на ASP.NET и обновите приложения, чтобы получить доступ к сведениям о почтовом ящике и сервере с помощью EWS.  <br/> |
|Поставщики WMI  <br/> |Нет  <br/> |[Командная консоль Exchange](management/exchange-management-shell.md) <br/> |Отсутствуют.  <br/> |
   
для использования API REST REST и Graph API требуется накопительный пакет обновления 3 для Exchange 2016.

² только пользователи с гибридными средами могут воспользоваться преимуществами REST API для Office 365 и локальных почтовых ящиков.

## <a name="see-also"></a>См. также

- [Выбор API или технологии для разработки решений для Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Требования к локальной архитектуре для REST API](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
