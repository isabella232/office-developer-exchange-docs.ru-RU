---
title: Операции EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Сведения об операциях EWS, доступных в Exchange.
ms.openlocfilehash: c56c3be746138cec251836fcb61ee3738d168869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762424"
---
# <a name="ews-operations-in-exchange"></a>Операции EWS в Exchange

Сведения об операциях EWS, доступных в Exchange.
  
Получить доступ к данным в хранилище Exchange вы можете с помощью множества операций веб-служб Exchange (EWS). Статьи в этом разделе описывают общую структуру запросов, ответов и сообщений об ошибочных ответах, касающихся операций EWS, а также содержат примеры XML для каждой такой операции. В них кратко рассмотрены структуры сообщений, которыми обмениваются клиент и сервер. Эти сведения позволят отладить структуры сообщений, а также узнать, какие действия доступны в запросе EWS. Дополнительные сведения о том, что представляет собой структура XML, см. в статье [XML-элементы EWS в Exchange](ews-xml-elements-in-exchange.md).
  
Функциональность EWS связана с версией схемы. Новые версии схемы EWS вводятся в новых выпусках Exchange Server или Exchange Online. Элемент [RequestServerVersion](requestserverversion.md) содержит атрибут **Version**, который сопоставляет версию сервера с версией схемы. В данной статье указано, когда была введена каждая операция. Для использования определенных возможностей операций может потребоваться более поздняя версия службы. Версионирование схем позволяет клиентам, разработанным для старой версии веб-служб Exchange, работать с новой их версией. 
  
Целевым объектом этих операций может быть конечная точка EWS, которая обслуживает почтовый ящик. Перейти к конечной точке EWS можно с помощью URL-адреса, подобного http://<clientaccessserver>.com/ews/exchange.asmx, где <clientaccessserver>  это сервер клиентского доступа Exchange, обслуживающий почтовый ящик. Получить URL-адрес сервера клиентского доступа, обслуживающего почтовый ящик, можно с помощью службы автообнаружения. Дополнительные сведения об автообнаружении см. в статье [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
## <a name="ediscovery-operations"></a>Операции обнаружения электронных данных
<a name="bk_eDiscovery"> </a>

Операции обнаружения электронных данных позволяют выполнять поиск в случае удержания по юридическим причинам, а также определять данные почтового ящика, которые невозможно индексировать и возвратить в результатах поиска для обнаружения.
  
В таблице ниже перечислены операции обнаружения электронных данных.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция SearchMailboxes](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Операции с данными почтовых ящиков Exchange
<a name="bk_Exchange_mailbox_data"> </a>

Операции с данными почтовых ящиков Exchange позволяют клиентам обрабатывать и упорядочивать папки, вложения и другие элементы, а также выполнять разрешение неоднозначных имен и расширение списков рассылки. Операции с данными почтовых ящиков Exchange включают операции с папками, вложениями, другими элементами, а также служебными программами.
  
В таблице ниже перечислены операции с данными почтовых ящиков Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция ArchiveItem](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[CreateItem Operation](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[CopyItem Operation](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция DeleteItem](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[FindItem Operation](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[GetItem Operation](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция MarkAllItemsAsRead](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[MoveItem Operation](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[SendItem Operation](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[UpdateItem Operation](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
В таблице ниже перечислены операции с папками данных в почтовых ящиках Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[CreateFolder Operation](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция CreateFolderPath](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция CreateManagedFolder](createmanagedfolder-operation.md) <br/> |Exchange 2007. Вместо этой возможности в Exchange 2010 и более поздних версий используются другие. Дополнительные сведения о том, как применять теги и политики хранения для управления записями сообщений, см. в статье [Переход от использования управляемых папок к использованию политик хранения](http://technet.microsoft.com/ru-RU/library/dd298032%28v=exchg.141%29.aspx).  <br/> |
|[Операция CopyFolder](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция DeleteFolder](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция EmptyFolder](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[FindFolder Operation](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[GetFolder Operation](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция MoveFolder](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[Операцию UpdateFolder](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
В таблице ниже перечислены операции с вложениями в почтовых ящиках Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция CreateAttachment](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция GetAttachment](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция DeleteAttachment](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
В таблице ниже перечислены операции с напоминаниями в почтовых ящиках Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetReminders](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция PerformReminderAction](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
В таблице ниже перечислены операции с беседами в почтовых ящиках Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция ApplyConversationAction](applyconversationaction-operation.md) <br/> |Exchange 2010 с пакетом обновления 1 (SP1)  <br/> |
|[FindConversation Operation](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[GetConversationItems operation](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
В таблице ниже перечислены операции с использованием служебных программ в почтовых ящиках Exchange.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция ConvertId](convertid-operation.md) <br/> |Exchange 2007 с пакетом обновления 1 (SP1)  <br/> |
|[Операция ExpandDL](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция GetUserPhoto](getuserphoto-operation.md) <br/> |Exchange 2013. Эта операция может выполняться как с помощью REST, так и с помощью протокола SOAP.  <br/> |
|[MarkAsJunk Operation](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция ResolveNames](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>Операции проверки доступности
<a name="bk_Availability"> </a>

Операции проверки доступности повышают удобство работы с календарем и обмена сведениями о доступности, так как предоставляют защищенные, актуальные и полные сведения о доступности. Сведения о доступности критически важны при планировании собраний. Поэтому операции проверки доступности обеспечивают его эффективность. 
  
В таблице ниже перечислены операции проверки доступности.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetUserAvailability](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция GetRoomLists](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetRooms](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetUserOofSettings](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция SetUserOofSettings](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>Операции массовой передачи данных
<a name="bk_bulk_transfer"> </a>

С помощью операций массовой передачи данных клиенты могут выполнять потоковую передачу элементов в почтовый ящик и из него. 
  
В таблице ниже перечислены операции массовой передачи данных.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция UploadItems](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Операция ExportItems](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>Операции управления делегированием
<a name="bk_delegate_management"> </a>

С помощью операций управления делегированием клиенты могут добавлять, получать, обновлять и удалять делегатов в почтовых ящиках. 
  
В таблице ниже перечислены операции управления делегированием.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция AddDelegate](adddelegate-operation.md) <br/> |Exchange 2007 с пакетом обновления 1 (SP1)  <br/> |
|[Операция GetDelegate](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Операция UpdateDelegate](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[Операция RemoveDelegate](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>Операции с правилами для папки "Входящие"
<a name="bk_inbox_rules"> </a>

Операции с правилами для папки "Входящие" позволяют клиентам получать правила для папки "Входящие" и обновлять их для сообщений на сервере. Правила для папки "Входящие"  это наборы условий и связанных с ними действий, с помощью которых клиенты могут автоматически упорядочивать и классифицировать сообщения, доставляемые в папки, а также выполнять с ними действия. 
  
В таблице ниже перечислены операции с правилами для папки "Входящие"
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetInboxRules](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Операция UpdateInboxRules](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>Операции управления почтовыми приложениями
<a name="bk_mail_apps"> </a>

Операции управления почтовыми приложениями позволяют управлять почтовыми приложениями для Outlook. С помощью этих операций можно устанавливать, удалять и отключать почтовые приложения, доступные для Outlook Web App и Outlook 2013, а также получать о них информацию.
  
В таблице ниже перечислены операции управления почтовыми приложениями.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция DisableApp](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetAppManifests](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetAppMarketplaceUrl](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetClientAccessToken](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция InstallApp](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция UninstallApp](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>Операция с подсказками электронной почты
<a name="bk_mail_tips"> </a>

Операция с подсказками электронной почты позволяет клиентам запрашивать у сервера сведения о почтовых ящиках получателей, когда автор составляет сообщение. В таблице ниже указана операция с подсказками электронной почты.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetMailTips](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>Операции отслеживания сообщений
<a name="bk_message_tracking"> </a>

С помощью операций отслеживания сообщений клиенты могут находить сообщения, соответствующие определенным условиям, и получать подробные сведения об отслеживании каждого сообщения в отчетах об отслеживании сообщений. 
  
В таблице ниже перечислены операции отслеживания сообщений.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>Операции с уведомлениями
<a name="bk_notification"> </a>

Операции с уведомлениями сообщают клиентскому приложению о событиях, связанных с элементами и папками в определенном почтовом ящике. Модель подписки может базироваться на push- и pull-технологии, а также потоковой передаче данных. 
  
В таблице ниже перечислены операции с уведомлениями.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetEvents](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция GetStreamingEvents](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[Операции подписки](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Отписаться операции](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Операции с пользователями
<a name="bk_personas"> </a>

При использовании операции с пользователями доступен интерфейс, с помощью которого можно находить и получать сведения о связанном контакте. В таблице ниже перечислены операции с пользователями.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция FindPeople](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetPersona](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>Операция с политиками хранения
<a name="bk_retention_policy"> </a>

Операция с политиками хранения предоставляет список всех тегов хранения, связанных с политикой хранения пользователя. 
  
В таблице ниже указана операция с политикой хранения.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetUserRetentionPolicyTags](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>Операция с конфигурацией служб
<a name="bk_service_config"> </a>

Операция с конфигурацией служб позволяет клиентам получать сведения о конфигурации для служб единой системы обмена сообщениями, правил защиты, подсказок политики и подсказок электронной почты. 
  
В таблице ниже указана операция с конфигурацией служб.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetServiceConfiguration](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>Операции общего доступа
<a name="bk_sharing"> </a>

С помощью операций общего доступа клиенты могут обмениваться данными календарей и контактов. 
  
В таблице ниже перечислены операции общего доступа.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010. Хотя операция **CreateItem** применима ко всем версиям EWS, объект ответа **AcceptSharingInvitation** применим только к EWS в Exchange 2010 и более поздних версий.  <br/> |
|[Операция GetSharingFolder](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetSharingMetadata](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция RefreshSharingFolder](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>Операции синхронизации
<a name="bk_synchronization"> </a>

Операции синхронизации предоставляют односторонне синхронизированную кэшированную копию папок и элементов пользователя. 
  
В таблице ниже перечислены операции синхронизации.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[Операция SyncFolderItems](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>Операция с часовыми поясами
<a name="bk_timezone"> </a>

Операция с часовыми поясами позволяет клиентам получить список определений часовых поясов, поддерживаемых сервером. 
  
В таблице ниже указана операция с часовыми поясами.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция GetServerTimeZones](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>Операции с единой системой обмена сообщениями
<a name="bk_um"> </a>

При помощи операций с единой системой обмена сообщениями клиенты могут читать сведения о свойствах единой системы обмена сообщениями и воспроизводить сообщения голосовой почты по телефону. 
  
В таблице ниже перечислены операции с единой системой обмена сообщениями.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция DisconnectPhoneCall](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetPhoneCallInformation](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция PlayOnPhone (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
[Операция GetServiceConfiguration](getserviceconfiguration-operation.md) позволяет получить сведения о конфигурации единой системы обмена сообщениями для почтового ящика. Для приложений единой системы обмена сообщениями, предназначенных для Exchange 2007, используйте веб-службу единой системы обмена сообщениями. Дополнительные сведения см. в статье [Единой системы обмена сообщениями веб-службы ссылки для Exchange](unified-messaging-web-service-reference-for-exchange.md).
  
## <a name="unified-contact-store-operations"></a>Операции с единым хранилищем контактов
<a name="bk_ucs"> </a>

Единое хранилище контактов позволяет использовать общий список контактов для всех продуктов Office и выполняет роль точки интеграции для сторонних приложений, чтобы они использовали то же самое хранилище контактов. С помощью него пользователи и приложения могут хранить сведения о контактах, управлять ими, получать к ним доступ, а также открывать глобальный доступ к ним в Lync, Exchange 2013, Outlook, Outlook Web App и других приложениях, в которых реализован доступ к единому хранилищу контактов. Exchange выполняет функцию хранилища содержимого для единого хранилища контактов.
  
В таблице ниже перечислены операции с единым хранилищем контактов.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция AddNewImContactToGroup](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция AddImContactToGroup](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция AddImGroup](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция AddNewTelUriContactToGroup](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetImItemList](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция GetImItems](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция RemoveContactFromImList](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция RemoveImContactFromGroup](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция RemoveDistributionGroupFromImList](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция RemoveImGroup](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Операция SetImGroup](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>Операции с конфигурациями пользователей
<a name="bk_user_config"> </a>

Операции с конфигурациями пользователей позволяют клиентам создавать, удалять, получать и обновлять сведения о конфигурации пользователей. 
  
В таблице ниже перечислены операции с конфигурациями пользователей.
  
|**Имя операции**|**Версия, где параметр был представлен**|
|:-----|:-----|
|[Операция CreateUserConfiguration](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция DeleteUserConfiguration](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция GetUserConfiguration](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[Операция UpdateUserConfiguration](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

