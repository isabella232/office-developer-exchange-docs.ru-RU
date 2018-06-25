---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: Элемент ResponseCode предоставляет сведения о состоянии о запросе.
ms.openlocfilehash: 7baeb0ab87ffb43ba9d6b4016477888aa4ed613e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835294"
---
# <a name="responsecode"></a>ResponseCode

Элемент **ResponseCode** предоставляет сведения о состоянии о запросе. 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|Элемент|Описание|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Содержит описательные сведения о состоянии ответа.<br/><br/>  Ниже приведены возможные выражения XPath для этого элемента.<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [DeleteItem операции](deleteitem-operation.md) .  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции SendItem](senditem-operation.md) .  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [DeleteFolder операции](deletefolder-operation.md) .  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [DeleteAttachment операции](deleteattachment-operation.md) .  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции отказа от подписки](unsubscribe-operation.md) .  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CreateFolder операции](createfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [GetFolder операции](getfolder-operation.md) .  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [UpdateFolder операции](updatefolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [MoveFolder операции](movefolder-operation.md) .  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CopyFolder операции](copyfolder-operation.md).  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CreateManagedFolder операции](createmanagedfolder-operation.md) .  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [FindFolder операции](findfolder-operation.md) .  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат один запрос [CreateItem операции](createitem-operation.md) .  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат одной [операции GetItem](getitem-operation.md) запроса.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [UpdateItem операции](updateitem-operation.md) .  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [MoveItem операции](moveitem-operation.md) .  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CopyItem операции](copyitem-operation.md) .  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CreateAttachment операции](createattachment-operation.md) .  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetAttachment](getattachment-operation.md) .  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [FindItem операции](finditem-operation.md) .  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат [операции ResolveNames](resolvenames-operation.md) запроса.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [ExpandDL операции](expanddl-operation.md) .  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат одной [подписки на операции](subscribe-operation.md) запроса.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [GetEvents операции](getevents-operation.md) .  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendNotification операции.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) запроса.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат [операции SyncFolderItems](syncfolderitems-operation.md) запроса.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат [операции ConvertId](convertid-operation.md) запроса.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат [операции GetDelegate](getdelegate-operation.md) запроса.  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Содержит состояние и результат [операции RemoveDelegate](removedelegate-operation.md) запроса.  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Содержит состояние и результат [операции UpdateDelegate](updatedelegate-operation.md) запроса.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Содержит состояние и результат [операции GetServerTimeZones](getservertimezones-operation.md) запроса.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат [операции GetSharingFolder](getsharingfolder-operation.md) запроса.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос [GetSharingFolder операции](getsharingfolder-operation.md) .  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Содержит состояние и результат [операции GetSharingMetadata](getsharingmetadata-operation.md) запроса.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат [операции RefreshSharingFolder](refreshsharingfolder-operation.md) запроса.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Определяет ответ на запрос [RefreshSharingFolder операции](refreshsharingfolder-operation.md) .  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Содержит состояние и результаты [операции FindConversation](findconversation-operation.md) ответа.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Содержит состояние и результаты запроса [ApplyConversationAction операции](applyconversationaction-operation.md) .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [EmptyFolder операции](emptyfolder-operation.md) .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Содержит состояние и результат [операции UpdateInboxRules](updateinboxrules-operation.md) запроса.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Содержит состояние и результат [операции UploadItems](uploaditems-operation.md) запроса.  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Содержит ответ на [операцию GetInboxRules](getinboxrules-operation.md) *** запроса.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Содержит ответ на запрос [GetServiceConfiguration операции](getserviceconfiguration-operation.md) .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным, если данный элемент используется. В следующей таблице описываются значений, возвращаемых с этим элементом.
  
|Значение|Описание|
|:-----|:-----|
|NoError  <br/> |Без ошибок для запроса.  <br/> |
|ErrorAccessDenied  <br/> |Эта ошибка возникает, когда вызывающей учетной записи нет прав на выполнение запрошенное действие.  <br/> |
|ErrorAccessModeSpecified  <br/> |Эта ошибка — только для внутреннего использования. Эта ошибка не возвращается.  <br/> |
|ErrorAccountDisabled  <br/> |Эта ошибка происходит, когда интересующую учетную запись была отключена.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Эта ошибка возникает, когда список с добавлены делегаты не могут быть сохранены.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Эта ошибка возникает, когда запись адресного пространства или имя домена доменных имен (DNS), для обеспечения доступности между лесами не найден в базе данных Active Directory.  <br/> |
|ErrorADOperation  <br/> |Эта ошибка происходит, когда операция завершилась неудачно из-за проблем связи с доменными службами Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Эта ошибка возвращается в том случае, когда запрос операции **ResolveNames** указывает имя, которое не является допустимым.  <br/> |
|ErrorADUnavailable  <br/> |Эта ошибка возникает при недоступности Доменные службы Active Directory. Повторите попытку позже.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Эта ошибка указывает, что атрибут **AffectedTaskOccurrences** не указан. Когда элемент [DeleteItem](deleteitem.md) используется для удаления по крайней мере один элемент, который является задачей, и независимо от того, является ли эту задачу повторяющейся или не должно быть указано, чтобы определить **DeleteItem** атрибут **AffectedTaskOccurrences** ли Удаление текущего экземпляра или всего ряда.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Отображается сообщение об ошибке в создание путь папки архива.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Указывает, что архивного почтового ящика не был включен.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Указывает, что обнаружение службы архивного почтового ящика не удалось.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Указывает, что предпринята попытка, чтобы создать элемент с более чем 10 вложений. Это значение появился в Exchange Server 2010 с пакетом обновления 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |Элемент [CreateAttachment](createattachment.md) возвращает эту ошибку при попытке создания вложения с размером превышение Int32.MaxValue, в байтах.  <br/> Элемент [GetAttachment](getattachment.md) возвращает эту ошибку, если при попытке получить существующий вложения с размером превышение Int32.MaxValue, в байтах.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Эта ошибка указывает, что веб-служб Exchange попытка определения расположения между лесами компьютер, на котором работает Exchange 2010, которая имеет роль сервера клиентского доступа, установленные с помощью службы автообнаружения, но обращение к службе автообнаружения не удалось.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Эта ошибка указывает, что сведения о конфигурации доступности в локальном лесу отсутствует в Доменных службах Active Directory.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Эта ошибка указывает, что возникает исключение при обработке элемента и что исключение скорее всего, будет выполнена для элементов, следуйте. Запросы могут включать несколько элементов; Например запрос операции GetItem может включать несколько идентификаторов. В общем случае элементы, обработанные одному за раз. Если возникает исключение при обработке элемента и, скорее всего, будет выполнена для элементов, следуйте исключение, элементы, следующие за не обрабатывается.  <br/><br/>  Ниже приведены примеры ошибок, которые будут Остановка обработки элементов, выполните:<br/>  <br/>-ErrorAccessDenied  <br/>-ErrorAccountDisabled  <br/>-ErrorADUnavailable  <br/>-ErrorADOperation  <br/>-ErrorConnectionFailed  <br/>-ErrorMailboxStoreUnavailable  <br/>-ErrorMailboxMoveInProgress  <br/>-ErrorPasswordChangeRequired  <br/>-ErrorPasswordExpired  <br/>-ErrorQuotaExceeded  <br/>-ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Эта ошибка возникает при попытке переместить или скопировать вхождение повторяющегося элемента календаря.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Эта ошибка возникает при попытке обновления элемента календаря, который находится в папке «Удаленные» и при изменения или отмены собраний, отправляются в соответствии с значение атрибута **SendMeetingInvitationsOrCancellations** . <br/><br/>Ниже приведены возможные значения этого атрибута.  <br/><br/>-SendToAllAndSaveCopy  <br/>-SendToChangedAndSaveCopy  <br/>-SendOnlyToAll  <br/>-SendOnlyToChanged  <br/>  <br/>Тем не менее такое обновление допускается только в том случае, если значение этого атрибута имеет значение SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Эта ошибка происходит, когда операция UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem или SendItem называется и идентификатор, который был указан не является Идентификатором вхождение любой повторяющегося элемента календаря.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Эта ошибка происходит, когда операция **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem**или **SendItem** называется и идентификатор, который был указан не является Идентификатором любого повторяющегося элемента шаблона.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem** при длительность элемента календаря превышает максимально допустимое, который в данный момент находится 5 лет.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Эта ошибка возникает, когда установлено время окончания календаря, в то же время или после времени начала.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Эта ошибка возникает, если указанная папка для операции **FindItem** с элементом [представления календаря](calendarview.md) не типа папки календаря.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Этот код ответа не используется.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem** при недопустимые значения даты, WeekendDay и день недели используются для определения изменений шаблон времени.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem** недопустимые значения даты, день недели и WeekendDay используемый для задания еженедельного повторения.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Эта ошибка происходит, когда состояние календаря элемента повторения больших двоичных объектов (BLOB) в хранилище Exchange является недопустимым.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Этот код ответа не используется.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Эта ошибка возникает, когда не удается создать указанный экземпляр.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Эта ошибка возникает, когда обнаружен недопустимый часовой пояс.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Эта ошибка означает, что было отменено элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Эта ошибка указывает, что было отменено элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Эта ошибка указывает, что было отменено элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Эта ошибка указывает, что было отменено элемента календаря.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Эта ошибка указывает, что элемент [AcceptItem](acceptitem.md) является недопустимым для календаря элемента или приглашения на собрание в делегированных сценарии.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Эта ошибка указывает, что элемент [DeclineItem](declineitem.md) является недопустимым для календаря элемента или приглашения на собрание в делегированных сценарии.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Эта ошибка указывает, что элемент [RemoveItem](removeitem.md) является недопустимым для отмены собрания в делегированных сценария.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Эта ошибка указывает, что элемент [TentativelyAcceptItem](tentativelyacceptitem.md) является недопустимым для календаря элемента или приглашения на собрание в делегированных сценарии.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Эта ошибка указывает, что операция (в настоящее время CancelItem) на элемент календаря не является допустимым для участника. Только организатор собрания можно отменить собрание.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Эта ошибка указывает, что [AcceptItem](acceptitem.md) является недопустимым для организатора элемента календаря.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Эта ошибка указывает, что [DeclineItem](declineitem.md) является недопустимым для организатора элемента календаря.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Эта ошибка указывает, что [RemoveItem](removeitem.md) является недопустимым для организатора элемента календаря. Удаление собрания из календаря, организатор необходимо использовать CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Эта ошибка указывает, что [TentativelyAcceptItem](tentativelyacceptitem.md) является недопустимым для организатора элемента календаря.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Эта ошибка указывает, что приглашения на собрание, устарел и не могут быть обновлены.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Эта ошибка указывает индекс вхождения не ведет появления в текущем повторения. Например если вы попытаетесь обратиться к пятому вхождение в расписании повторов определяет набор из трех вхождений собрания, приведет к данный код ответа.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Эта ошибка указывает, что любые операции на удаленных вхождение (адресуемый посредством повторяющихся главного индекса идентификатор и вхождение) является недопустимым.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Эта ошибка отчета о CreateItem и UpdateItem операции для элементов календаря или свойства повторения задачи, когда значение свойства находится вне диапазона. Например указание пятнадцатый недели, месяца приведет к данный код ответа.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Эта ошибка возникает при запуске диапазон окончания для [представления календаря](calendarview.md) элемент превышает максимально допустимое, в настоящее время через 2 года.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Эта ошибка указывает, что запрашивающая учетная запись не является допустимую учетную запись в базу данных каталога.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Указывает, что была предпринята попытка архивировать папки контактов задач календаря.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Указывает, что была предпринята попытка архивировать элементы в общедоступных папках.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Указывает, что была предпринята попытка архивировать элементы в архивный почтовый ящик.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Эта ошибка возникает при создании элемента календаря и **SavedItemFolderId** атрибут относится к папке календаря, отличного от.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Эта ошибка возникает при создании контакта и **SavedItemFolderId** атрибут относится к папке не контакта.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Эта ошибка указывает, что элемента записи не могут создаваться в папке, отличной от папки почты, например календаря, контактов, задач, заметки и т. д.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Эта ошибка возникает при создании задачи и **SavedItemFolderId** атрибут относится к папке не задач.  <br/> |
|ErrorCannotDeleteObject  <br/> |Эта ошибка происходит, когда элемент или папку для удаления не может быть удален.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |[Операция DeleteItem](deleteitem-operation.md) возвращает эту ошибку, если не удается удалить текущее вхождение повторяющейся задачи. Происходит, только если атрибут **AffectedTaskOccurrences** имеет значение SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Указывает, что предпринята попытка, чтобы отключить расширение mandatorty.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Эта ошибка должна возвращаться при серверу не удается очистить папку.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Указывает, что не удалось получить путь к исходной папке.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Указывает, что сервер не удалось получить внешний URL-адрес для параметры Outlook Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |Операция **GetAttachment** возвращает эту ошибку, если он не удается извлечь тело вложенный файл.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Эта ошибка указывает, что вызывающий попытался задать разрешения календаря для календаря, отличного от папки.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Эта ошибка указывает, что вызывающий попытался задать разрешения календаря, отличного от папки календаря.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Эта ошибка указывает, что нельзя задать Неизвестный разрешения в наборе разрешений.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Указывает, что предпринята попытка, чтобы указать папки поиска в качестве исходной папки.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Эта ошибка возникает, когда запрос, который требуется идентификатор элемента присваивается идентификатор папки.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Эта ошибка возникает, когда запрос, который требуется идентификатор папки присваивается идентификатор элемента.  <br/> |
|ErrorChangeKeyRequired  <br/> |Этот код ответа была заменена **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Если изменить ключ для элемента отсутствующие или устаревшие этой ошибки. <br/><br/>Для операции SendItem, UpdateItem и UpdateFolder вызывающий объект должен передать в правильное и текущей изменить ключ для элемента. Обратите внимание, что в случае с UpdateItem даже в том случае, если разрешения конфликтов задано значение всегда overwrite.  <br/> |
|ErrorClientDisconnected  <br/> |Указывает, что клиент был отключен.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorClientIntentNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorConnectionFailed  <br/> |Эта ошибка возникает, когда веб-служб Exchange не удается подключиться к почтовому ящику.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Эта ошибка указывает, что свойство, который был проверен для фильтра содержит не строковый тип.  <br/> |
|ErrorContentConversionFailed  <br/> |Операции **GetItem** возвращает эту ошибку, когда веб-служб Exchange не удается получить содержимого MIME для элемента запроса. <br/><br/>Операции **CreateItem** возвращает эту ошибку, если веб-служб Exchange не удается создать элемент из предоставленного содержимого MIME. Обычно это указывает на то, что свойство item повреждена или усечено.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Эта ошибка происходит, когда запрос поиска выполняется с помощью параметра строки запроса и индексации содержимого не включен для целевого почтового ящика.  <br/> |
|ErrorCorruptData  <br/> |Эта ошибка возникает, когда данные повреждена и не может обработать.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Эта ошибка возникает, когда вызывающий не имеет разрешения на создание элемента.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Эта ошибка возникает, когда один или несколько управляемых папок, которые были указаны в запрос операции CreateManagedFolder не удалось создать. Выполните поиск каждой папки, чтобы определить, какие папки были созданы и папки, которые не существуют.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Эта ошибка возникает, когда вызывающий учетная запись не имеет разрешения, необходимые для создания вложенной папке.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Эта ошибка возникает при попытке переместить элемент или папку из одного почтового ящика в другой. Эта ошибка может возникнуть, если исходный почтовый ящик и почтового ящика назначения отличаются.  <br/> |
|ErrorCrossSiteRequest  <br/> |Эта ошибка указывает на то, что запрос не допускается, так как сервер клиентского доступа, который должен обработать запрос на другом сайте.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Эта ошибка может возникнуть в следующих сценариях:<br/>  <br/>-Попытка получить доступ или запись свойства элемента, а значение свойства слишком велик.<br/>-Base64 кодировке MIME содержимого, что длина в запросе XML превышает предел.<br/>-Размер текста существующего основной текст элемента, превышает ограничение.<br/>-Получатель пытается записать HTML или текст body, чьи (или объединенный длины в случае append) превышает предел. |
|ErrorDataSourceOperation  <br/> |Эта ошибка возникает при сбое базового поставщика данных для выполнения операции.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Эта ошибка возникает в рамках одной операции **AddDelegate** , когда указанный пользователь уже существует в список делегатов.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Эта ошибка возникает в рамках одной операции **AddDelegate** после указанного пользователя добавляется владелец почтового ящика.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Эта ошибка возникает в ходе операции **GetDelegate** при либо нет не делегат или сведения о на локальном занятости сообщение без Active Directory открытый делегат (без «открытый делегат» или нет записи «Отправить от имени» в AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Эта ошибка возникает, когда указанный пользователь не может быть сопоставлен пользователя в Доменных службах Active Directory.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Эта ошибка возникает в операции **AddDelegate** , когда добавлены делегированного пользователя не является допустимым.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Эта ошибка возникает при попытке удалить именованной папки.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Эта ошибка указывает, что идентификатор различающееся пользователя не является допустимым для операции. **DistinguishedUserType** не должны присутствовать в запросе.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Эта ошибка указывает, что списка рассылки запроса не существует в списке рассылки.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Эта ошибка возникает при указании одинаковые имена папок в элементе [FolderNames](foldernames.md) **CreateManagedFolder** операции запроса.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Эта ошибка означает, что повторяющиеся заголовки SOAP.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Эта ошибка указывает, что идентификатор пользователя найден в наборе разрешений анонимной или по умолчанию задается несколько раз, либо существуют повторяющиеся идентификаторы безопасности или получателей.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Эта ошибка возникает при попытке выполнить запрос на создание или изменение параметров поиска папки поиска. Например это может произойти при создании папки поиска в почтовом ящике, но направляются папки поиска необходимо выполнить поиск другого почтового ящика.  <br/> |
|ErrorEventNotFound  <br/> |Эта ошибка возникает при удалении событий, который связан с водяного знака перед возвращением события. При появлении этой ошибки также удаляется подписки.  <br/> |
|ErrorExceededConnectionCount  <br/> |Эта ошибка - указывает, что ничего существует несколько параллельных запросов на сервере превышает допустимый политикой пользователя.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Эта ошибка указывает, что пользователь регулирование политики, которую превышено максимальное подписки число.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Эта ошибка указывает, что вызов операции поиска превысил общее число элементов, которые могут быть возвращены.  <br/> |
|ErrorExpiredSubscription  <br/> |Эта ошибка возникает, если [операция GetEvents](getevents-operation.md) вызывается как подписки удаляется, так как он истек.  <br/> |
|ErrorExtensionNotFound  <br/> |Указывает, что данное расширение имени файла не найден.  <br/> |
|ErrorFolderCorrupt  <br/> |Эта ошибка происходит, когда папка повреждена и не могут быть сохранены.  <br/> |
|ErrorFolderExists  <br/> |Эта ошибка возникает при попытке создайте папку с таким же именем в другую папку в же родительским. Использование повторяющихся имен не допускается.  <br/> |
|ErrorFolderNotFound  <br/> |Эта ошибка указывает, что идентификатор папки, которая была указана не соответствует допустимую папку или том, что делегат не имеет разрешения на доступ к папке.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Эта ошибка указывает, что свойство не удалось получить. Указывает, что свойство не существует, но, что оно повреждено каким-либо образом, чтобы не удалось выполнить извлечение.  <br/> |
|ErrorFolderSave  <br/> |Эта ошибка указывает, что папка не удалось созданные или обновленные из-за недопустимом состоянии.  <br/> |
|ErrorFolderSaveFailed  <br/> |Эта ошибка указывает, что папка не удалось созданные или обновленные из-за недопустимом состоянии.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Эта ошибка указывает, что папка не удалось созданные или обновленные из-за недопустимости значений свойства. Код ответа список свойств, которые проблемы, возникающие.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Эта ошибка указывает, что группа максимальное число элементов достигнут для получения сведений о доступности для списка рассылки.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Если не удается получить сведения о доступности из-за промежуточного сбоя этой ошибки.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorImContactLimitReached  <br/> |Эта ошибка возвращается, когда нельзя добавить новый обмена мгновенными сообщениями контакты обмена Мгновенными сообщениями, так как достигнуто максимальное число контактов. Эта ошибка была представлена в Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |При попытке добавить отображаемое имя группы при существующей группы уже имеет то же отображаемое имя этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Эта ошибка возвращается, когда нельзя добавить новые группы обмена мгновенными Сообщениями, так как достигнуто максимальное число групп. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |Ошибка возвращается в случае сервер сервер авторизации для олицетворения Exchange при вызывающий не имеет необходимых прав для олицетворения определенного пользователя в вопросе. Эта ошибка сопоставляет ms-Exch-EPI-May-Impersonate расширенные право Active Directory.  <br/> |
|ErrorImpersonationDenied  <br/> |Эта ошибка возвращается в сервер сервер авторизации для олицетворения Exchange при вызывающий не имеет необходимых прав для олицетворения через сервер клиентского доступа, который они берут запрос к. Сопоставляет ms-Exch-EPI-Impersonation расширенные право Active Directory.  <br/> |
|ErrorImpersonationFailed  <br/> |Эта ошибка указывает, что возникла непредвиденная ошибка при попытке выполнения проверки подлинности сервер сервер. Этот код ответа указывает на то, что учетная запись службы, на котором работает веб-служб Exchange, пул приложений настроен неправильно, что веб-служб Exchange не могут обратиться к каталогу или то, что отношение доверия между лесами не правильно настроить.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Эта ошибка указывает, что запрос является допустимым для текущей версии сервера Exchange, но был недействителен для версии сервера запросов, который был указан.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Эта ошибка указывает, что каждое описание изменений в элементах [UpdateItem](updateitem.md) или [UpdateFolder](updatefolder.md) должно содержать только одно свойство для обновления.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Эта ошибка возникает, когда запрос содержит слишком много участников для разрешения конфликтов. По умолчанию максимальное количество участников для разрешения конфликтов равно 100.  <br/> |
|ErrorInsufficientResources  <br/> |Эта ошибка возникает, когда перегрузки сервера почтовых ящиков. Повторите попытку позже.  <br/> |
|ErrorInternalServerError  <br/> |Эта ошибка указывает, что веб-служб Exchange произошла ошибка, которая не удалось восстановить из и более конкретные код ответа, связанного с возникшей ошибки не существует.  <br/> |
|ErrorInternalServerTransientError  <br/> |Эта ошибка указывает, что произошла ошибка внутреннего сервера и что запрос необходимо повторить попытку позже.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Эта ошибка указывает, что уровень доступа с абонентом на данные о доступности является недопустимым.  <br/> |
|ErrorInvalidArgument  <br/> |Эта ошибка указывает ошибки, возникающие при всех недопустимых аргументов, передаваемых [GetMessageTrackingReport операции](getmessagetrackingreport-operation.md).<br/><br/> Эта ошибка возвращается в следующих случаях: <br/><br/>-Пользователя, указанного в _отправки-как_ параметр не существует в каталоге. <br/>-Пользователя, указанного в _отправки-как_ параметр не является уникальным в каталоге. <br/>- _Отправки-как_ адрес будет пустым.<br/>- _Отправки-как_ адрес не является адресом электронной почты.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Этой ошибки [операция GetAttachment](getattachment-operation.md) или [DeleteAttachment операции](deleteattachment-operation.md) при вложения, соответствующий указанным Идентификатором не найден.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Эта ошибка возникает при попытке выполнить привязку к существующей папки поиска с помощью ограничение сложных вложений в таблице. Простой поддерживает только веб-служб Exchange содержит фильтров к таблице вложений. При попытке привязки к существующей папке поиска с более сложным ограничением таблицы вложений (вложенный фильтр), веб-служб Exchange не удается обработать XML-код для него и возвращает данный код ответа. <br/><br/>Обратите внимание, что по-прежнему можно вызвать операции GetFolder в общей папке, но не запросить элемент [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Эта ошибка возникает при попытке выполнить привязку к существующей папки поиска с помощью ограничение сложных вложений в таблице. Простой поддерживает только веб-служб Exchange содержит фильтров к таблице вложений. <br/><br/>При попытке выполнить привязку к существующей папке поиска с более сложным ограничением для таблицы вложений, веб-служб Exchange не удается отобразить XML-код для этого фильтра. В этом случае вложенный фильтр вложений содержит текст фильтр, но не посмотрев отображаемое имя вложения.<br/><br/> Обратите внимание, что по-прежнему можно вызвать операции GetFolder в общей папке, но не запросить элемент [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Эта ошибка указывает, что не удалось выполнить процедуру авторизации для инициатора запроса.  <br/> |
|ErrorInvalidChangeKey  <br/> |Эта ошибка происходит, когда получатель проходит в папке или идентификатор элемента с изменить ключ, который невозможно выполнить синтаксический анализ. Например это может быть содержимое недопустимый base64 или пустая строка.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Эта ошибка указывает, что возникла внутренняя ошибка при попытка разрешить удостоверения вызывающей стороны.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Эта ошибка возвращается при попытке задать значение элемента [CompleteDate](completedate.md) задачи на время в будущем. После преобразования местного времени сервера клиентского доступа [CompleteDate](completedate.md) задачи не может быть присвоено значение, более поздней, чем местного времени на сервере клиентского доступа.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Эта ошибка указывает, что предоставляется недопустимый адрес электронной почты контакта.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Эта ошибка указывает, что указанное значение индекса недопустимый электронной почты запись электронной почты.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Эта ошибка возникает, когда учетные данные, используемые для прокси-сервера запрос на лес службы другой каталог не выполняется проверка подлинности.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Эта ошибка указывает, что разрешения указанной папки являются недопустимыми.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Эта ошибка указывает, что идентификатор пользователя указанный делегат является недопустимым.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Эта ошибка возникает во время олицетворения Exchange, когда Звонящий не указывает имя участника-пользователя, адрес электронной почты или ИД безопасности пользователя. Это также возникает, если вызывающего указывает одно или несколько из них и значения будут пустыми.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Эта ошибка возникает, когда Битовая маска, переданный в элемент ограничению [Excludes](excludes.md) не удается выполнить синтаксический анализ.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Эта ошибка возникает при возникновении следующих событий: <br/> <br/>-Вызывающего пытается использовать расширенное свойство, не поддерживаемый веб-служб Exchange.  <br/>-Вызывающего абонента передает Недопустимое сочетание значений атрибутов для расширенного свойства. Это также происходит, если передается без атрибутов. Разрешены только определенные сочетания.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Эта ошибка возникает, когда в разделе значение расширенного свойства не соответствует типу свойства. <br/><br/>Например, Установка расширенного свойства, которое имеет PropertyType = «String» для массива целых чисел приведет к данной ошибки. Любое строковое представление, который не является принудительного в тип, который задан для расширенного свойства предоставит Эта ошибка.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Эта ошибка указывает, общего доступа отправителю приглашения не была создана общего доступа с приглашением метаданных.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Эта ошибка указывает, что сообщение общего доступа не предназначен для вызывающего абонента.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Эта ошибка указывает, что объекты федерации организации инициатора не настроены правильно.  <br/> |
|ErrorInvalidFolderId  <br/> |Эта ошибка возникает, когда ИД папки поврежден.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Эта ошибка указывает, что тип указанная папка является недопустимым для текущей операции. Например не удается создать папку поиска в общей папке.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Эта ошибка возникает в дробная разбиение на страницы, когда задан один из следующих: <br/> <br/>-Числителем, больше, чем делителя  <br/>-Числителем, меньше нуля  <br/>-Делителя, меньше или равно нулю  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Эта ошибка указывает, что элементы [типа данных](datatype.md) и ShareFolderId операции присваивания являются присутствует в запросе.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Эта ошибка возникает, когда [операция GetUserAvailability](getuseravailability-operation.md) вызывается с [FreeBusyViewType](freebusyviewtype.md) нет.  <br/> |
|ErrorInvalidId  <br/> |Эта ошибка указывает, что ключ идентификатора и/или изменение неверный формат.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Эта ошибка происходит, когда Звонящий указывает атрибут **Id** , пуст.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Эта ошибка происходит, когда элемент не может быть нравится, что. Версии Exchange, начиная с номер сборки 15.00.0913.09 включать это значение.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Эта ошибка возникает, когда Звонящий указывает атрибут **Id** , имеет неверный формат.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Эта ошибка указывает, что идентификатор папки или элемента, в формате Exchange 2007 был указанного запроса с версией Exchange 2007 с пакетом обновления 1 или более поздней версии. Нельзя использовать идентификаторы Exchange 2007 в Exchange 2007 с пакетом обновления 1 или более поздней версии запросы. Необходимо сначала преобразовать с помощью [операции ConvertId](convertid-operation.md) .  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Эта ошибка возникает, когда Звонящий указывает атрибут **Id** , слишком много времени.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Эта ошибка возвращается в том случае, когда идентификатор, который не является вложение элемента, идентификатор передается в метод веб-службы, требующей идентификатор вложения.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Эта ошибка возникает, когда контакт в свой почтовый ящик поврежден.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Эта ошибка возникает, когда Звонящий указывает атрибут **Id** , слишком много времени.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Когда иерархия вложений элемента превышает максимум 255 уровней этой ошибки.  <br/> |
|ErrorInvalidIdXml  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidImContactId  <br/> |Если указанный идентификатор контакта обмена мгновенными Сообщениями не представляет допустимый идентификатор этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Если адрес SMTP идентификатор для указанного обмена мгновенными Сообщениями рассылки группы не представляет допустимый идентификатор этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Если указанный идентификатор группы обмена мгновенными Сообщениями не представляет допустимый идентификатор этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Эта ошибка возникает, если Смещение индексированного постраничного просмотра является отрицательным.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Указывает, что элемент был недействителен для операции **ArchiveItem** .  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Эта ошибка возникает при попытке использовать объект ответа AcceptItem тип элемента не приглашения на собрание или элемента календаря или при попытке принять вхождение элемента календаря, который находится в папку «Удаленные».  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Эта ошибка возникает при попытке использовать объект CancelItem ответа на тип элемента, отличного от элемента календаря.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | При попытке создать вложение элемента неподдерживаемый тип этой ошибки.  <br/><br/>  Типы поддерживаемых элементов для вложений элемента включают следующие объекты:  <br/><br/>- [Элемент](item.md) <br/>- [Сообщение](message-ex15websvcsotherref.md) <br/>- [Элемента календаря, имеющего](calendaritem.md) <br/>- [Задача](task.md) <br/>- [Контакт](contact.md) <br/> <br/> Например если попытаться создать подключение к [MeetingMessage](meetingmessage.md) , встречающиеся этот код ответа.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Эта ошибка возвращается из [операции CreateItem](createitem-operation.md) , если запрос содержит тип не поддерживается. <br/><br/>Поддерживаемые элементы включают следующие объекты:<br/>  <br/>- [Элемент](item.md) <br/>- [Сообщение](message-ex15websvcsotherref.md) <br/>- [Элемента календаря, имеющего](calendaritem.md) <br/>- [Задача](task.md) <br/>- [Контакт](contact.md) <br/><br/>  Определенные типы создаются в качестве побочные эффекты выполнения. Собрания сообщений, например, создаются при отправке элемента календаря для участников; они не создаются явным образом.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Эта ошибка возникает при попытке использовать объект ответа DeclineItem тип элемента не приглашения на собрание или элемента календаря или при попытке отклонить вхождение элемента календаря, который находится в папку «Удаленные».  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Эта ошибка указывает, что [операция ExpandDL](expanddl-operation.md) действителен только в частные списки рассылки.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Эта ошибка возвращается из объекта ответа RemoveItem, если запрос указывает элемент, который не является собрания элемент отмены.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Эта ошибка возвращается из [операции SendItem](senditem-operation.md) , если запрос указывает элемент, который не является элемента сообщения.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Эта ошибка возникает при попытке использовать [TentativelyAcceptItem](tentativelyacceptitem.md) тип элемента не приглашения на собрание или элемента календаря или при попытке принять под вопросом вхождение элемента календаря, который находится в папку «Удаленные».  <br/> |
|ErrorInvalidLogonType  <br/> |Эта ошибка — только для внутреннего использования. Эта ошибка не возвращается.  <br/> |
|ErrorInvalidMailbox  <br/> |Эта ошибка указывает, что [UpdateItem операции](updateitem-operation.md) или [операции CreateItem](createitem-operation.md) сбой при создании или обновлении списка рассылки.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Эта ошибка возникает, когда структура управляемой папки повреждена и не может быть обработана.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Эта ошибка возникает, когда квот, заданное для управляемой папки меньше нуля указывает поврежденные управляемых папок.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Эта ошибка возникает, когда размер, заданное для управляемой папки меньше нуля указывает поврежденные управляемых папок.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Эта ошибка происходит, когда объединенные обмен сведениями о доступности внутреннего заданному является недопустимым. Минимальное значение по умолчанию — 5 минут. Максимальное значение по умолчанию — 1440 минут.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Эта ошибка происходит, когда [операция ResolveNames](resolvenames-operation.md)недопустимое имя. Например строку нулевой длины, пробелом, запятой и тире являются все недопустимые имена.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Эта ошибка указывает на ошибку в учетную запись сетевой службы на сервере клиентского доступа.  <br/> |
|ErrorInvalidOofParameter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidOperation  <br/> | Это общая ошибка, которая будет использоваться при Запрошенная операция является недопустимым. <br/><br/>Например нельзя выполните следующее: <br/> <br/>-Выполните «Глубокий» обзор с помощью [операции FindFolder](findfolder-operation.md) для общей папки.  <br/>-Перемещение или копирование корневой общей папки.  <br/>-Удаление связанного элемента с помощью любого режима, за исключением «Жестко» удалить.  <br/>-Переместить или скопировать связанный элемент.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Эта ошибка указывает, что вызывающего запрошено сведения о доступности для пользователей в другой организации, но организационное отношение не имеет сведений о доступности включен.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Эта ошибка возникает, если потребитель передает ноль или отрицательное значение для максимальное число строк должно быть возвращено.  <br/> |
|ErrorInvalidParentFolder  <br/> |Эта ошибка возникает, если потребитель передает недопустимый родительской папки для операции. Например, для этой ошибки при попытке создания папки внутри папки поиска.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Эта ошибка возвращается при попытке задать процент завершения задач недопустимое значение. Значение должно быть между 0 и 100 (включительно).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Эта ошибка указывает, что уровень разрешений не соответствует параметры разрешений.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Эта ошибка указывает, что идентификатор звонящего не является допустимым.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Эта ошибка указывает, что номер телефона неправильно или не соответствуют телефонным обдумайте правила.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Эта ошибка возникает, если свойство, которое требуется добавить, не поддерживает добавление. <br/><br/>Ниже приведены только свойства, которые поддерживает добавление. <br/> <br/>-Получателя семейств сайтов (ToRecipients, CcRecipients, BccRecipients)  <br/>-Attendee семейств сайтов (RequiredAttendees, OptionalAttendees, кадров)  <br/>-Body  <br/>-ReplyTo  <br/><br/>  Кроме того эта ошибка происходит, когда текст сообщения добавляется, если формата, указанного в запросе не соответствует формату элемента в хранилище.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Эта ошибка возникает, если операция удаления указан в вызове [UpdateItem операции](updateitem-operation.md) или [операции UpdateFolder](updatefolder-operation.md) для свойства, которое не поддерживает операцию удаления. Например нельзя удалить элемент [ItemId](itemid.md) объекта [Item](item.md) .  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Эта ошибка возникает, если получатель проходит по одному из свойств флаг в фильтре [Exists](exists.md) . Например Эта ошибка возникает, если флаги [IsRead](isread.md) или [IsFromMe](isfromme.md) заданы в элементе [Exists](exists.md) . Запрос следует использовать элемент [выражение IsEqualTo](isequalto.md) для этих как есть флаги и, следовательно, частью отдельное свойство.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Эта ошибка возникает, если свойство, которое требуется для работы с не поддерживает операции.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Эта ошибка возникает, если свойство, указанное в запросе не доступен с типом элемента. Например этой ошибки при запросе свойство, которое доступно только на элементы календаря в ходе [операции GetItem](getitem-operation.md) звонок для сообщения или обновляется в рамках одной [операции UpdateItem](updateitem-operation.md) звонков для сообщения. <br/> <br/>  Этот шаг выполняется в следующих операций: <br/> <br/>- [Операции GetItem](getitem-operation.md) <br/>- [Операция GetFolder](getfolder-operation.md) <br/>- [Операция UpdateItem](updateitem-operation.md) <br/>- [Операция UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Эта ошибка указывает, что свойство, которое требуется для работы с не поддерживает операции. Например Эта ошибка возвращается, если свойство, которое вы пытаетесь установить доступен только для чтения.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Эта ошибка возникает во время [операции UpdateItem](updateitem-operation.md) , когда клиент пытается обновить определенные свойства, которое уже было отправлено сообщение.<br/><br/> Например на отправленное сообщение не удается обновить следующие свойства: <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Эта ошибка возникает при вызове с помощью идентификатора подписки push [GetEvents операции](getevents-operation.md) или [операции отказа от подписки](unsubscribe-operation.md) Чтобы отписаться от принудительной подписки, необходимо ответить на запрос push отказом от подписки, или отключите веб-службы и дождитесь push-уведомления для времени ожидания.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Эта ошибка возвращается [подписки на операции](subscribe-operation.md) , если он создает подписки «push» и указывает, что URL-адрес, который включен в запрос является недопустимым.<br/><br/>Для веб-служб Exchange для приема URL-адреса должны быть выполнены следующие условия: <br/> <br/>-Длина строки \> 0 и \< 2083.  <br/>-Является http или https.  <br/>— URL-адрес можно преобразовать в классе URI Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Эта ошибка указывает, что набор получателей сообщения или набор приглашенных элементу календаря является недопустимым. Например будут возвращены Эта ошибка при попытке отправить элемент, который не имеет получателей.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Эта ошибка указывает, что папка поиска имеет фильтра получателей таблицы, которая не может представлять веб-служб Exchange. Чтобы обойти эту ошибку, извлеките папку, не запрашивая параметры поиска.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Эта ошибка указывает, что папка поиска имеет фильтра получателей таблицы, которая не может представлять веб-служб Exchange. Чтобы обойти эту ошибку, извлеките папку, не запрашивая параметры поиска.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Эта ошибка указывает, что папка поиска имеет фильтра получателей таблицы, которая не может представлять веб-служб Exchange. Чтобы обойти эту ошибку, извлеките папку, не запрашивая параметры поиска.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Эта ошибка указывает, что папка поиска имеет фильтра получателей таблицы, которая не может представлять веб-служб Exchange. Чтобы обойти эту ошибку, извлеките папку, не запрашивая параметры поиска.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Эта ошибка возвращается из [операции CreateItem](createitem-operation.md) для прямого и ответ объекты ответа в следующих сценариях:<br/>  <br/>-Идентификатор указанного элемента не [сообщения](message-ex15websvcsotherref.md), [элемента календаря, имеющего](calendaritem.md)или потомком **сообщения** или **элемента календаря, имеющего**.  <br/>— Идентификатор элемента ссылки для **элемента календаря, имеющего** и организатора пытается Reply или ReplyAll для самого себя.  <br/>-Сообщение является черновиком и Reply или ReplyAll.  <br/>-Элемент ссылки для [SuppressReadReceipt](suppressreadreceipt.md), не является потомком **сообщения**или **сообщения** .  <br/> |
|ErrorInvalidRequest  <br/> |Эта ошибка возникает, если запрос SOAP содержит заголовок действия SOAP, но не в тексте сообщения SOAP. Обратите внимание, что заголовок действия SOAP не требуется, как веб-служб Exchange можно определить метод, вызываемый из локального имя корневого элемента в тексте запроса SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Эта ошибка возвращается, когда тега хранения указанного имеет неправильные действие, связанное с ним. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Когда попытка задать тег несуществующий или невидимой для свойства **PolicyTag** этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Когда попытка задать неявных тег для свойства **PolicyTag** этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Указывает недопустимый идентификатор GUID тега хранения.  <br/> |
|ErrorInvalidRoutingType  <br/> |Эта ошибка возникает, если тип маршрутизации, которое передается для элемента [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) является недопустимым. Как правило типа маршрутизации задается для SMTP Simple Mail Transfer Protocol ().  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Эта ошибка возникает, если заданное время окончания периода не превышает время начала или время окончания не происходит в будущем.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Эта ошибка указывает, что запрос прокси-сервера, который был отправлен на другой сервер не может обслуживать запрос из-за несоответствие управления версиями.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Эта ошибка указывает, что поврежден дескриптор безопасности в папке календаря в хранилище Exchange.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Эта ошибка возникает при попытке отправить элемент, где [SavedItemFolderId](saveditemfolderid.md) указан в запросе, но свойство **SaveItemToFolder** имеет значение **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Эта ошибка указывает, что маркер, который был передан в заголовке, имеет неверный формат, не ссылается на допустимую учетную запись в каталоге или отсутствует основной группы **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Эта ошибка указывает, что общего доступа метаданных является недопустимым. Это может быть вызвано недопустимый XML.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Эта ошибка указывает на то, что общего доступа сообщение не является допустимым. Это может быть вызвано отсутствующие свойства.  <br/> |
|ErrorInvalidSid  <br/> |Эта ошибка возникает, когда недопустимое, которое передается ИД безопасности в запросе.  <br/> |
|ErrorInvalidSIPUri  <br/> |Эта ошибка указывает, что имя SIP, абонентской группы или номер телефона неправильных URI SIP.  <br/> |
|ErrorInvalidServerVersion  <br/> |Эта ошибка указывает, что версия сервера недопустимый запрос был задан в запросе.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Эта ошибка происходит, когда невозможно выполнить синтаксический анализ SMTP-адрес.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubscription  <br/> |Эта ошибка указывает, что подписки больше не является допустимым. Это может быть, так как перезапуск сервера клиентского доступа или истечения срока действия подписки.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Эта ошибка указывает, что запрос подписки на включить несколько общих папок идентификаторы. Подписка может включать несколько папок из этого почтового ящика или один идентификатор общей папки.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Эта ошибка возвращается по [SyncFolderItems](syncfolderitems.md) или [SyncFolderHierarchy](syncfolderhierarchy.md) , если [состояние](syncstate-ex15websvcsotherref.md) данных, которое передается является недопустимым. Чтобы устранить эту ошибку, необходимо повторно выполнить синхронизацию без состояние синхронизации. Убедитесь, что при наличии Сохранение синхронизации состоянии большие двоичные объекты, можно не был случайно усечен больших двоичных ОБЪЕКТОВ.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Эта ошибка указывает, что для указанного временного интервала является недопустимым. Время начала должно быть больше или равно времени окончания.  <br/> |
|ErrorInvalidUserInfo  <br/> |Эта ошибка указывает, что во внутреннем несогласованные [UserId](userid.md) был задан для выполнения операции разрешения. Например если идентификатор различающееся пользователя указанного (по умолчанию или анонимный доступ), этой ошибки при попытке также указать идентификатор безопасности или основной SMTP-адрес или отображаемое имя для этого пользователя.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Эта ошибка указывает, что параметры пользователя об отсутствии на работе Office (OOF) недопустимы из-за отсутствующих внутреннего или внешнего ответа.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Эта ошибка возникает во время олицетворения Exchange. При вызове передан в недопустимое имя участника-пользователя в заголовке SOAP, который недоступен в каталоге.  <br/> |
|ErrorInvalidUserSid  <br/> |Эта ошибка возникает, когда недопустимое, которое передается ИД безопасности в запросе.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Эта ошибка указывает, что для свойства, которое оно сравнивается недопустимое значение сравнения в ограничении.<br/><br/> Например, для сравнения значения [DateTimeCreated](datetimecreated.md) > **значение true,** будет возвращен данный код ответа. <br/><br/>Этот код ответа возвращается также в том случае, если для сравнения задано свойство перечисления, но значение, оно сравнивается не допустимое значение для перечисления.  <br/> |
|ErrorInvalidWatermark  <br/> |Эта ошибка возникает по недопустимый водяного знака.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Эта ошибка указывает, что допустимый шлюз VoIP недоступно.  <br/> |
|ErrorIrresolvableConflict  <br/> |Эта ошибка указывает, что разрешения конфликтов не удалось разрешить изменения свойств. Элементы в хранилище были изменены и необходимо обновить. Получите обновленный ключ изменения и повторите попытку.  <br/> |
|ErrorItemCorrupt  <br/> |Эта ошибка указывает, что состояние объекта повреждена и не может быть извлечен. При извлечении элемента в этом состоянии, такие как [текст](body.md) и [MimeContent](mimecontent.md)будет только определенные элементы. Пропустить эти элементы и повторите операцию.  <br/> |
|ErrorItemNotFound  <br/> |Эта ошибка происходит, когда элемент не найден или нет разрешения на доступ к элемента.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Эта ошибка возникает, если не удается выполнить запрос свойства элемента. Свойство существует, но его не удалось получить.  <br/> |
|ErrorItemSave  <br/> |Эта ошибка возникает, когда не удалось сохранить элемент или папку.  <br/> |
|ErrorItemSavePropertyError  <br/> |Эта ошибка возникает, когда не удалось сохранить элемент или папку из-за недопустимости значений свойства. Код ответа включает путь недопустимые свойства.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Этот код ответа не используется.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Этот код ответа не используется.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Эта ошибка указывает, что служба доступности не удалось выполнить вход в качестве сетевой службы для запросов прокси-сервера для соответствующих сайтов или лесов. В этом ответа указывает на то, ошибки в конфигурации.  <br/> |
|ErrorMailboxConfiguration  <br/> |Эта ошибка указывает, что сведения о почтовых ящиках в Доменных службах Active Directory настроен неправильно.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Эта ошибка указывает, что элемент [MailboxDataArray](mailboxdataarray.md) в запросе пуст. Необходимо указать по крайней мере один идентификатор почтового ящика.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Эта ошибка возникает при более чем 100 записей поставляются в элементе [MailboxDataArray](mailboxdataarray.md) ...  <br/> |
|ErrorMailboxFailover  <br/> |Эта ошибка указывает, что при попытке получить доступ к почтовому ящику сбой при почтовый ящик в процессе перехода на другой ресурс.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Указывает, что удержание почтовых ящиков не найден.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Эта ошибка возникает при сбое подключения к почтовому ящику для получения информации о представлении календаря.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Эта ошибка указывает, что почтовый ящик перемещается в другое хранилище или сервера. Эта ошибка также может указывать, что почтовый ящик в другую базу данных сервера или почтового ящика.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Эта ошибка указывает, что один следующее сообщение об ошибке возникновения условий:  <br/><br/>-Поврежден хранилища почтовых ящиков.  <br/>-В хранилище почтовых ящиков остановлена.  <br/>-В хранилище почтовых ящиков находится в автономном режиме.  <br/>-Ошибка сети при попытке доступа к хранилищу данных почтовых ящиков.  <br/>-В хранилище почтовых ящиков перегружен и не может принимать дополнительные подключения.  <br/>-В хранилище почтовых ящиков был приостановлен.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Эта ошибка возникает, если данные элемента [MailboxData](mailboxdata.md) не может быть сопоставлен допустимый почтовый ящик учетной записи.  <br/> |
|ErrorMailTipsDisabled  <br/> |Эта ошибка указывает, что почтовые подсказки отключены.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Эта ошибка возникает, если управляемой папки, который вы пытаетесь создать, уже существует в почтовом ящике.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Эта ошибка возникает, когда имя папки, который был указан в запросе не соответствует определению управляемой папки в Доменные службы Active Directory. Можно создавать только экземпляры управляемых папок для папок, которые определены в Доменных службах Active Directory. Проверьте имя и повторите попытку.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Эта ошибка указывает, что корневой элемент управляемых папок удален из почтового ящика или, что папка существует в той же родительской папке с именем корневой управляемой папки. Это также возникает, если попытка создания корневой управляемой папки возникает ошибка.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Эта ошибка указывает, что модуль предложений произошла ошибка при попытке создания предложений.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Эта ошибка возникает, если атрибут **MessageDisposition** не установлен.<br/><br/> Этот атрибут является обязательным для следующих: <br/> <br/>- [Операции CreateItem](createitem-operation.md) , а [операция UpdateItem](updateitem-operation.md) при элемента созданные или обновленные [сообщения](message-ex15websvcsotherref.md).  <br/>- Объекты ответа [CancelCalendarItem](cancelcalendaritem.md), [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)или [TentativelyAcceptItem](tentativelyacceptitem.md) .  <br/> |
|ErrorMessageSizeExceeded  <br/> |Эта ошибка указывает, что сообщение, которое вы пытаетесь отправить превышает допустимое.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Эта ошибка указывает, что не удается найти указанного домена.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Эта ошибка указывает, что служба отслеживания сообщений не может отслеживать сообщения.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Эта ошибка указывает, что служба отслеживания сообщений — вниз или занят. Эта ошибка указывает на временные ошибки. Клиенты можно повторить для подключения к серверу при получении данной ошибки.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Эта ошибка возникает при содержимого MIME не является допустимым для [операции CreateItem](createitem-operation.md)iCal. Для выполнения [операции GetItem](getitem-operation.md)такой ответ означает, что содержимого MIME не удалось создать.  <br/> |
|ErrorMimeContentInvalid  <br/> |Эта ошибка возникает при недопустимом содержимого MIME.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Эта ошибка возникает, когда содержимого MIME в запросе не является допустимой базовый 64 строкой.  <br/> |
|ErrorMissingArgument  <br/> |Эта ошибка указывает, что обязательный аргумент не указаны в запросе. Текст сообщения ответа указывает, какой аргумент для проверки.  <br/> |
|ErrorMissingEmailAddress  <br/> |Эта ошибка указывает ИД именованной папки указанного в запросе, что учетная запись, отправившего запрос не имеет почтового ящика в системе. В этом случае необходимо задать дочерний элемент [почтовых ящиков](mailbox.md) в группе [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Эта ошибка указывает ИД именованной папки указанного в запросе, что учетная запись, отправившего запрос не имеет почтового ящика в системе. В этом случае необходимо задать дочерний элемент [почтовых ящиков](mailbox.md) в группе [DistinguishedFolderId](distinguishedfolderid.md). Этот ответ возвращается из [CreateManagedFolder операции](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Эта ошибка возникает, если элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) отсутствует.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Эта ошибка возникает, если отсутствует [ReferenceItemId](referenceitemid.md) .  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Этот код ошибки, никогда не возвращается.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Эта ошибка возвращается при попытке включает элемент в элементе **ItemAttachment** [CreateAttachment операции](createattachment-operation.md) запроса.  <br/> |
|ErrorMissingManagedFolderId  <br/> |Эта ошибка возникает, когда свойство идентификаторов политики тег свойства 0x6732 для папки отсутствует. Необходимо учитывать это поврежденные папки.  <br/> |
|ErrorMissingRecipients  <br/> |Эта ошибка указывает, что вы указали для отправки элемента, не включая получателей. Обратите внимание на то, что при вызове [операции CreateItem](createitem-operation.md) с ликвидации сообщения, создающий сообщение было отправлено, вы получите следующий код ответа: **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Эта ошибка указывает на то, что [идентификатор пользователя](userid.md) не был полностью указан в наборе разрешений.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Эта ошибка указывает, что указано более одного элемента значение [ExchangeImpersonation](exchangeimpersonation.md) внутри запроса.  <br/> |
|ErrorMoveCopyFailed  <br/> |Эта ошибка указывает на то, что не удалось выполнить операцию перемещения или копирования. Перемещение выполняется в [операции CreateItem](createitem-operation.md) при принятии приглашения на собрание, находящийся в папку «Удаленные». Кроме того Если отклонение приглашения на собрание, отмены элемента календаря или удаление собрания из календаря, перемещении для папки «Удаленные».  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Эта ошибка возникает при попытке перемещения именованной папки.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Эта ошибка возникает, когда запрос пытается получить доступ к несколько серверов почтовых ящиков. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Эта ошибка возникает, если [операция ResolveNames](resolvenames-operation.md) возвращает несколько результатов или неоднозначное имя, указанное соответствует нескольким объектам в каталоге. Код ответа содержатся совпадающие имена из данных ответа.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Эта ошибка указывает, что вызывающий не имеет почтового ящика в системе. [ResolveNames операции](resolvenames-operation.md) или [операции ExpandDL](expanddl-operation.md) является недопустимым для подключения пользователей без почтового ящика.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Эта ошибка указывает, что [операция ResolveNames](resolvenames-operation.md) не возвращает результатов.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Этот код ошибки должны возвращаться при веб-службы не удается найти сервер для обработки запроса.  <br/> |
|ErrorNoCalendar  <br/> |Эта ошибка возникает, если нет папки календаря для почтового ящика.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Эта ошибка указывает, что запрос делается ссылка в почтовый ящик на другом сайте Active Directory, но нет серверов клиентского доступа в целевом сайте были настроены для проверки подлинности Windows и таким образом запрос не может быть прокси.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Эта ошибка указывает, что запрос делается ссылка в почтовый ящик на другом сайте Active Directory, но нет серверов клиентского доступа в целевом сайте были настроены для SSL-соединений и таким образом запрос не может быть прокси.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Эта ошибка указывает, что запрос делается ссылка в почтовый ящик на другом сайте Active Directory, но не серверы клиентского доступа в целевом сайте, версии продукта приемлемой для получения запроса и таким образом запрос не может быть прокси.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Эта ошибка возникает, если значение элемента [FolderClass](folderclass.md) при создании элемента, не общей папки. Для типизированных папок, таких как [CalendarFolder](calendarfolder.md) и [TasksFolder](tasksfolder.md)подразумевается класс папки. Установка класса папки в одной папке с тип с помощью результаты [операции UpdateFolder](updatefolder-operation.md) в ответ **ErrorObjectTypeChanged** . Вместо этого использовать папкой стандартного типа, но присвоено значение, которое требуется класс папки. Веб-служб Exchange создадим строго типизированные нужную папку.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Эта ошибка указывает на то, что вызывающий не имеет права на просмотр сведений о доступности на в папке календаря.  <br/> |
|ErrorNonExistentMailbox  <br/> | Эта ошибка возникает в следующих случаях: <br/> <br/>— В [CreateManagedFolder](createmanagedfolder.md)пуст адрес электронной почты.  <br/>— Адрес электронной почты не ссылается на допустимую учетную запись в запросе, который принимает адрес электронной почты, в тексте или в заголовке SOAP, например, в вызове олицетворения Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Эта ошибка возникает, если вызывающий объект передает не основной SMTP-адрес. Ответ включает правильный SMTP-адрес для использования.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Эта ошибка указывает, что свойства MAPI в настраиваемом диапазоне 0x8000 и более поздних версий, не могут быть созданы с помощью свойства тегов. Необходимо использовать управляемый API EWS [PropertySetId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)свойство или элемент веб-служб Exchange [ExtendedFieldURI](extendedfielduri.md) с помощью атрибута PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Этот код ответа не используется.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Этот код ошибки должны возвращаться при наличии без сервера общих папок или если вызывающий не имеет Домашняя страница общедоступный сервер.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Эта ошибка указывает, что запрос делается ссылка почтового ящика в другом сайте Active Directory, но ни один из серверов клиентского доступа, ответил сайта, а следовательно запроса не удалось через прокси.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Эта ошибка указывает, что вызывающий попытался для предоставления разрешений в папке календаря и контакты, которые пользователю в другую организацию и попытка не удалась.  <br/> |
|ErrorNotDelegate  <br/> |Эта ошибка указывает, что пользователь не делегат для почтового ящика. Он возвращается в виде [GetDelegate операции](getdelegate-operation.md), [RemoveDelegate операции](removedelegate-operation.md)и [операции UpdateDelegate](updatedelegate-operation.md) при указанного делегата не найден в список делегатов.  <br/> |
|ErrorNotEnoughMemory  <br/> |Эта ошибка указывает на то, что операция не удалось из-за нехватки памяти.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Эта ошибка указывает, что сообщение о совместном доступе не поддерживается.  <br/> |
|ErrorObjectTypeChanged  <br/> |Эта ошибка возникает при изменении типа объекта.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Эта ошибка возникает при обновлении времени [запуска](start.md) или [окончания](end-ex15websvcsotherref.md) вхождения, чтобы этот экземпляр планируется происходить более ранних версий или более поздней, чем соответствующие предыдущему или следующему вхождение.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Эта ошибка указывает, что определенное время для это вхождение перекрывается с другим вхождения одной повторяющегося элемента. В этом ответа также происходит, когда продолжительность в минутах вхождение больше, чем Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Эта ошибка указывает, что текущей операции не является допустимым для корневой общей папки.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Эта ошибка указывает, что организации инициатора не являющийся ни федеративным источник запроса не удается создать сообщения о совместном использовании для отправки для внешних пользователей или не может принимать общего доступа к сообщениям, полученных от внешнего пользователя.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Этот код ответа не используется.  <br/> |
|ErrorParentFolderNotFound  <br/> |Эта ошибка возникает в [операции CreateFolder](createfolder-operation.md) при родительской папки не найден.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Эта ошибка указывает, что необходимо изменить пароль для доступа к этому почтовому ящику. Происходит, когда был создан новой учетной записи и администратор указал, что Требовать смену пароля при первом входе в систему. Не удается обновить пароль с помощью веб-служб Exchange. Средства, такие как Microsoft Office Outlook Web App необходимо использовать для изменения пароля.  <br/> |
|ErrorPasswordExpired  <br/> |Эта ошибка указывает, что истек срок действия пароля. Нельзя изменить пароль с помощью веб-служб Exchange. Средства, такие как Outlook Web App необходимо использовать для изменения пароля.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Эта ошибка указывает, что источник запроса попытка предоставить разрешения в его календаря или папки «Контакты» для внешних пользователей, но политики общего доступа, назначенный источник запроса указывает, что запрошенный уровень выше, чем позволяет какие политики общего доступа.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Эта ошибка указывает, что номер телефона не должен иметь формат.  <br/> |
|ErrorPropertyUpdate  <br/> |Эта ошибка указывает, что не удалось обновить из-за недопустимости значений свойства. Ответное сообщение, которое включает в себя пути к недопустимым свойствам.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Этот код ответа не используется.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Эта ошибка указывает, что запрос делается ссылка подписки, который существует на другой сервер клиентского доступа, но произошла ошибка прокси-сервера запросов к серверу клиентского доступа.  <br/> |
|ErrorProxyCallFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Эта ошибка указывает, что запрос делается ссылка в почтовый ящик на другом сайте Active Directory и инициатор должна быть членом группы более 3000.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Эта ошибка указывает, что запрос отправки веб-служб Exchange на другой сервер клиентского доступа при попытке выполнения запроса [GetUserAvailabilityRequest](getuseravailabilityrequest.md) недопустима. Этот код ответа указывает на то, что произошла ошибка конфигурации или права или что кто-то неудачной попытки для имитации запроса доступности прокси-сервера.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Эта ошибка указывает, что веб-служб Exchange попытка прокси-сервера на другой сервер клиентского доступа для выполнения запроса доступности, но не удалось выполнить запрос. В этом ответа может быть вызвана проблем с сетевым подключением или запроса проблемы времени ожидания.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Этот код ошибки должны возвращаться, если веб-службы не может определить ли запрос должна выполняться на целевом сервере или будет прокси-сервером на другой сервер.  <br/> |
|ErrorProxyTokenExpired  <br/> |Этот код ответа не используется.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Эта ошибка возникает, когда почтовый ящик общедоступных папок не удается найти URL-адрес. Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Эта ошибка возникает при попытке получить доступ к общей папке и попытка завершается неудачно. Эта ошибка была введена в 2013Exchange Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Эта ошибка возникает, когда получатель, переданный [операция GetUserAvailability](getuseravailability-operation.md) находится на компьютере, на котором выполняется версия Exchange Server, который является более ранней, чем Exchange 2007 и запрос на получение сведений о доступности для не удалось получателя с сервера общих папок.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Эта ошибка возникает, когда получатель, переданный [операция GetUserAvailability](getuseravailability-operation.md) находится на компьютере, на котором выполняется версия Exchange Server, который является более ранней, чем Exchange 2007 и запрос на получение сведений о доступности для подразделение не имеет связанных общих папок сервера сбой получателя с сервера общих папок.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Эта ошибка возникает при синхронизации операция успешно для почтового ящика общей папки основного, но не удается с почтовым ящиком общей папке вторичного. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Эта ошибка указывает, что ограничения папки поиска могут стать недействительными, но не поддерживается веб-служб Exchange. Для не более 255 выражений фильтров ограничений веб-служб Exchange. При попытке выполнить привязку к существующей папки поиска, превышающее 255, возвращается этот код ответа.  <br/> |
|ErrorQuotaExceeded  <br/> |Эта ошибка возникает при превышении квоты почтового ящика.  <br/> |
|ErrorReadEventsFailed  <br/> |Эта ошибка возвращается [GetEvents операции](getevents-operation.md) или извещающих уведомлений при сбое при получении сведений о событиях. При появлении этой ошибки удаляется подписки. Повторно создайте события синхронизации, на основании последнего известные водяного знака.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Эта ошибка возвращается [операции CreateItem](createitem-operation.md) при попытке не отображать уведомление, когда отправитель сообщения не запросил прочтении в окне сообщения, или если сообщение находится в папку нежелательной почты.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Эта ошибка возникает, когда дата окончания повторения после 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Эта ошибка возникает, если указанный экземпляр любого экземпляров вхождений в указанном диапазоне.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Эта ошибка указывает, что список делегатов не удалось сохранить после делегаты были удалены.  <br/> |
|ErrorRequestAborted  <br/> |Этот код ответа не используется.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Эта ошибка возникает, когда поток запросов больше, чем 400 КБ.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |При отсутствии в запросе [CreateAttachment операция](createattachment-operation.md) обязательное свойство этой ошибки. Отсутствует свойство URI включается в ответе.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Эта ошибка указывает, что Звонящий задан в папку, которая не является папкой контактов к [ResolveNames операции](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Эта ошибка указывает, что Звонящий указала несколько папок контактов к [ResolveNames операции](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Этот код ответа не используется.  <br/> |
|ErrorRestrictionTooLong  <br/> |Эта ошибка возникает при ограничении содержит более 255 узлы.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Эта ошибка возникает при ограничении не могут выполняться с веб-служб Exchange.  <br/> |
|ErrorResultSetTooBig  <br/> |Эта ошибка указывает, что число записей календаря для данного получателя превышает максимально допустимое значение 1000. Уменьшение окна и повторите попытку.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Эта ошибка возникает, когда [SavedItemFolderId](saveditemfolderid.md) не найден.  <br/> |
|ErrorSchemaValidation  <br/> | Эта ошибка возникает, если запрос не удается проверить соответствие схеме.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Эта ошибка указывает, что папка поиска была создана, но не заданы критерии поиска в общей папке. Это возникает только при получении доступа к поврежденные поиска папок, которые были созданы с помощью другого интерфейса API или клиента. Чтобы устранить эту ошибку, с помощью [операции UpdateFolder](updatefolder-operation.md) установка [SearchParameters](searchparameters.md) элемента, который требуется включить ограничение, которое должно быть в общей папке.  <br/> |
|ErrorSendAsDenied  <br/> | Эта ошибка возникает при оба из следующих условий: <br/> <br/>— Пользователь имеет разрешений CanActAsOwner, но не предоставлены права делегатом почтового ящика участника.  <br/>-Тот же пользователь попытается для создания и отправки сообщения электронной почты в почтовом ящике участника с помощью параметра SendAndSaveCopy.<br/>  <br/>  Результатом будет ошибка ErrorSendAsDenied и создание сообщения электронной почты в папке «Черновики» участника.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Эта ошибка возвращается [операция DeleteItem](deleteitem-operation.md) Если отсутствует атрибут **SendMeetingCancellations** в запрос и элемент для удаления элемента календаря.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Эта ошибка возвращается [операция UpdateItem](updateitem-operation.md) Если отсутствует атрибут **SendMeetingInvitationsOrCancellations** в запрос и элемент для обновления элементов календаря.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Эта ошибка возвращается [операции CreateItem](createitem-operation.md) Если отсутствует атрибут **SendMeetingInvitations** в запрос и элемент для создания элемента календаря.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Эта ошибка указывает, что после организатора отправки приглашения на собрание, запрос не удается обновить. Для изменения собрания, измените элемент календаря не приглашения на собрание.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Эта ошибка указывает, что после инициатором отправки запроса на задачу, этот запрос не удается обновить.  <br/> |
|ErrorServerBusy  <br/> |Эта ошибка возникает, когда сервер занят.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Эта ошибка указывает, что веб-служб Exchange попытка прокси-сервер пользовательского запроса доступности в соответствующий лес для получателя, но он не может определить where для отправки запроса из-за сбоя обнаружения служб.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Эта ошибка указывает, что свойство внешний URL-адрес не установлен в базе данных Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Эта ошибка указывает, что Сбой попытки синхронизации папки общего доступа. <br/><br/>Этот код ошибки возвращается в следующих случаях:<br/><br/>-Подписки для общего доступа к папке не найден.<br/>-Папку совместного доступа не найден.<br/>— Пользователю соответствующий каталог не найден.<br/>— Пользователю больше не существует.<br/>-Встречи является недопустимым.<br/>-Контакт является недопустимым.<br/>-Имеется ошибка связи с удаленным сервером.  <br/> |
|ErrorStaleObject  <br/> |Эта ошибка возникает в [UpdateItem операции](updateitem-operation.md) или [операции SendItem](senditem-operation.md) при изменить ключ не обновлена или не было указано. Вызов [операции GetItem](getitem-operation.md) , чтобы получить обновленный ключ изменения, а затем повторите попытку.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Эта ошибка означает, что пользователь не удается отправить сразу несколько запросов недоступности квот отправки.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Эта ошибка возникает при попытке доступа к подписке с использованием учетной записи, которая не была создана этой подписки. Доступ к каждой подписки можно только для создатель подписки.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Эта ошибка указывает, что нельзя создать подписку, если не является владельцем или нет доступа к почтовому ящику.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Эта ошибка возникает, если не удастся найти подписки, соответствующий указанным [SubscriptionId (GetEvents)](subscriptionid-getevents.md) . Подписки может истечь, процесс веб-служб Exchange был перезагружен или передано недопустимое подписки. Если подписки был действительным, повторно создайте подписки с последними водяного знака. Эта [операция отказа от подписки](unsubscribe-operation.md) или возвращает ответы [GetEvents операции](getevents-operation.md) .  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Этот код ошибки должны возвращаться при запросе для подписки, которая была отменена.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Эта ошибка возвращается [операции SyncFolderItems](syncfolderitems-operation.md) Если не удается найти указанной родительской папки.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Эта ошибка указывает, что почтовый ящик группы не найден. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Эта ошибка указывает, что почтовый ящик группы был найден, но не связаны на сервер SharePoint. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Эта ошибка указывает, что почтовый ящик группы найден, но ссылка на сервере SharePoint не является допустимым. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Этот код ошибки не используется. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Этот код ошибки не используется. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Эта ошибка указывает, что при попытке отправить уведомление владельцев группы почтовых ящиков не удалось выполнить. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Эта ошибка указывает Общая ошибка, которая может возникнуть при попытке получения доступа к почтовому ящику группы. Попробуйте отправки запроса в дальнейшем. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Эта ошибка указывает, что временной интервал, который был указан превышает максимально допустимое значение. По умолчанию максимально допустимое значение равно 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Эта ошибка возникает, когда не достаточное время для завершения обработки запроса.  <br/> |
|ErrorTimeZone  <br/> |Эта ошибка указывает на наличие ошибок часового пояса.  <br/> |
|ErrorToFolderNotFound  <br/> |Эта ошибка указывает, что папка не существует.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Эта ошибка возникает, если вызывающий объект пытается выполнить запрос сериализации маркера, но не имеет ms-Exch-EPI-TokenSerialization прямо на сервере клиентского доступа.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Эта ошибка возникает, когда превысил внутреннее ограничение на открытых объектов.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Эта ошибка указывает, что абонентской группы пользователя недоступно.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Эта ошибка указывает, что пользователь не найден.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Эта ошибка указывает, что действительный сервер для абонентской группы можно найти для обработки запроса.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Эта ошибка возникает при попытке удалить для обмена мгновенными Сообщениями контакта из группы неудачной попытки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Эта ошибка возникает при попытке задать свойство **языка и региональных параметров** в значение, которое не является разбору с помощью класса **System.Globalization.CultureInfo** .  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Эта ошибка возникает при попытке использовать расширенные свойства типов объектов, массив объектов, ошибки или null абонента.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Эта ошибка возникает при попытке получить или задать содержимого MIME для элемента, не [PostItem](postitem.md), [сообщения](message-ex15websvcsotherref.md)или [элемента календаря, имеющего](calendaritem.md) объекта.  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Эта ошибка возникает, когда при вызове свойства, которое является недопустимым для запроса. Это может произойти при использовании вычисляемых свойств.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Эта ошибка возникает, когда при вызове свойства, которое является недопустимым для сортировки или группы по свойству. Это может произойти при использовании вычисляемых свойств.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Эта ошибка указывает, что ограничения папки поиска могут стать недействительными, но не поддерживается веб-служб Exchange.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Эта ошибка указывает, что указанный экземпляр не поддерживается для задачи.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Эта ошибка указывает, что веб-служб Exchange тип свойства в хранилище, но он не удается создать XML для типа свойства.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Эта ошибка указывает, что список делегатов не удалось сохранить после делегаты были обновлены.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Эта ошибка возникает, когда отдельное свойство путь, указанный в описании изменения не соответствует отдельное свойство, которое задано в объекте фактический [элемент](item.md) или [папку](folder.md) .  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Эта ошибка указывает, что источник запроса не включено.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Эта ошибка указывает, что источник запроса попытка предоставить разрешения в его календаря или папки «Контакты» для внешних пользователей, но политики общего доступа, назначенный источник запроса указывает, что домен внешнего пользователя не указано в политике.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Указывает, что организации инициатора имеет ряд федеративных доменов, но организации инициатора не имеет все SMTP-адреса прокси-сервера с одним из федеративных доменов.  <br/> |
|ErrorValueOutOfRange  <br/> |Эта ошибка указывает, что представление календаря Дата начала или дату окончания было задано значение 1/1/0001 12:00:00 AM или 12/31/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Эта ошибка указывает, что в хранилище Exchange, обнаруженных в сообщении вирус.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Эта ошибка указывает, что хранилище Exchange вирус, обнаруженных в сообщении и он удален.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWin32InteropError  <br/> |Эта ошибка указывает, что возникла внутренняя ошибка во время связи с управляемым кодом.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWrongServerVersion  <br/> |Эта ошибка указывает на то, что запрос можно выполнить только на сервере, который является той же версии, что и сервер почтовых ящиков.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Эта ошибка указывает, что создан запрос делегатом, который имеет другой сервер версии, чем основной сервер почтовых ящиков.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Этот код ошибки, никогда не возвращается.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Указывает, что существуют повторяющиеся заголовки SOAP.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Указывает, что Сбой попытки синхронизации папки общего доступа.<br/><br/> Этот код ошибки должны возвращаться когда:<br/><br/>-Подписки для общего доступа к папке не найден.  <br/>-Не найден общую папку.  <br/>— Пользователю соответствующий каталог не найден.  <br/>— Пользователю больше не существует.  <br/>-Встречи является недопустимым.  <br/>-Контакт является недопустимым.  <br/>-Возникла ошибка связи с удаленным сервером.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Указывает, что свойство внешний URL-адрес не установлен в базе данных Active Directory. Этот код ошибки должны возвращаться, если свойство внешний URL-адрес не были установлены в базе данных Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Указывает, что группа максимальное число элементов достигнут для получения сведений о доступности для списка рассылки. Эта ошибка должна возвращаться при достижении группы максимальное число элементов для получения сведений о доступности для списка рассылки.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Указывает, что элемент типа данных и ShareFolderId оба присутствует в запросе. Этот код ошибки должны возвращаться, если тип данных и ShareFolderId элемент присутствует в запросе.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Указывает, вызывающего попытка предоставить разрешения в папке календаря и контакты, которые пользователю в другую организацию и Сбой попытки. Этот код ошибки должны возвращаться при отключении политики общего доступа для вызывающего абонента или когда политики общего доступа, назначенный вызывающего абонента запрещает общий доступ для запрошенный уровень или тип запрошенного папки.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Указывает, что попытка инициатора запроса для предоставления разрешений в его календаря или папки «Контакты» для внешних пользователей, но политики общего доступа, назначенный для инициатора запроса указывает, что домен внешнего пользователя не указано в политике.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Указывает, что инициатора запроса, попытка предоставить разрешения в папке календаря и контакты, для внешних пользователей, но политики общего доступа, назначенный для инициатора запроса указывает, что запрошенный уровень выше чем какие политики общего доступа позволяет.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Указывает, что организация запрашивающего не являющийся ни федеративным инициатора запроса не удается создать сообщения о совместном использовании для отправки для внешних пользователей или не может принимать общего доступа к сообщениям, полученных от внешнего пользователя. Этот код ошибки должны возвращаться Если запрашивающего организации не являющийся ни федеративным.  <br/> |
|ErrorMailboxFailover  <br/> |Указывает, что при попытке получить доступ к почтовому ящику сбой при почтовый ящик в процессе перехода на другой ресурс.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Указывает, общего доступа отправителю приглашения не была создана общего доступа с приглашением метаданных. Этот код ошибки должны возвращаться Если общего доступа отправителю приглашения не была создана общего доступа с приглашением метаданных.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Указывает, что служба отслеживания сообщений не может отслеживать сообщения.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Указывает, что сообщение, службы отслеживания — вниз или занят. Этот код ошибки указывает временные ошибки. Клиенты можно повторить для подключения к серверу при получении данной ошибки.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Указывает, что не удается найти указанного домена.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Указывает, что организация запрашивающего имеет ряд федеративных доменов, но организации запросившая сторона не имеет все SMTP-адреса прокси-сервера с одним из федеративных доменов.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Указывает, что вызывающего запрошено сведения о доступности для пользователей в другой организации, но организационное отношение не имеет сведений о доступности включен.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Указывает, что объекты федерации организации запрашивающего настроены неправильно.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Указывает, что сообщение общего доступа не предназначен для вызывающего абонента.  <br/> |
|ErrorInvalidSharingData  <br/> |Указывает, что общего доступа метаданных является недопустимым. Это может быть вызвано недопустимый XML.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Указывает, что общего доступа сообщение не является допустимым. Это может быть вызвано отсутствующие свойства.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Указывает, что сообщение о совместном доступе не поддерживается.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Эта ошибка должна возвращаться Если действие, которое не может использоваться для одного или нескольких элементов в окне беседы.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Эта ошибка должно возвращаться, если все правила не выполняет проверку.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Эта ошибка необходимо снова, когда происходит при попытке управлять правила папки «Входящие» после другой клиент доступ к правила папки «Входящие».  <br/> |
|ErrorRulesOverQuota  <br/> |Эта ошибка должна возвращаться при превышении квот правила пользователя.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Эта ошибка должно возвращаться для первого подключения подписки при открытии второго соединения подписки.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Эта ошибка должна возвращаться при пропущенные уведомления о событиях.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Эта ошибка возвращается при наличии повторяющихся устаревшие различающиеся имена в доменных службах Active Directory (AD DS). Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Эта ошибка указывает, что недопустимый запрос на получение маркера клиентского доступа. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Если заголовок [ManagementRole](managementrole.md) в заголовке SOAP неверен этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |При выполнении поиска с заданной областью попытки без использования элемент [строки запроса (String)](querystring-string.md) для индексирования поиска содержимого этой ошибки. Это применимо для операций **SearchMailboxes** и **FindConversation** . Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Эта ошибка возвращается при поискового запроса архивного почтового ящика не выполняется. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Эта ошибка возвращается, когда URL-адрес архивного почтового ящика не может быть найдена. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Эта ошибка возникает, когда не удалось выполнить операцию для получения удаленный архив почтового ящика.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Эта ошибка возникает при сбое операцию, чтобы найти папку архивного почтового ящика.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Эта ошибка возникает, когда не удалось выполнить операцию для получения элемента архивного почтового ящика.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Эта ошибка возникает, когда не удалось выполнить операцию для экспорта элементов архивного почтового ящика.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Эта ошибка возвращается в том случае, если размер недопустимый фотографии, запрашиваемый с сервера. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |При запросе размер непредвиденные фотографии в запрос операции **GetUserPhoto** этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Если запрос операции **SearchMailboxes** содержит слишком много почтовые ящики для поиска этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Эта ошибка указывает, что для этого пользователя не найдены без тегов хранения. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |При отключении операций поиска обнаружения на клиента или сервера для этой ошибки. Эта ошибка была представлена в Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Эта ошибка возникает при попытке вызова [операции FindItem](finditem-operation.md) с [SeekToConditionPageItemView](seektoconditionpageitemview.md) на извлечение элементов календаря, который не поддерживается.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |Клиент будет помечено для удаления.  <br/> |
|ErrorInvalidLicense  <br/> |У пользователя нет действительная лицензия.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Получать сообщения в папке Квота превышена.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент не является обязательным и не добавляется во все ответы. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

