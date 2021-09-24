---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: Элемент ResponseCode предоставляет сведения о состоянии запроса.
ms.openlocfilehash: 9d662ee93870c2aabe045d801222deb881d0a28b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512389"
---
# <a name="responsecode"></a>ResponseCode

Элемент **ResponseCode** предоставляет сведения о состоянии запроса. 
  
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
|[ResponseMessage](responsemessage.md) <br/> | Предоставляет описательные сведения о состоянии ответа.<br/><br/>  Возможные выражения XPath к этому элементу:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции DeleteItem.](deleteitem-operation.md)  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции SendItem.](senditem-operation.md)  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции DeleteFolder.](deletefolder-operation.md)  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции DeleteAttachment.](deleteattachment-operation.md)  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [отписки.](unsubscribe-operation.md)  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateFolder.](createfolder-operation.md)  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetFolder.](getfolder-operation.md)  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции UpdateFolder.](updatefolder-operation.md)  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [MoveFolder.](movefolder-operation.md)  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CopyFolder.](copyfolder-operation.md)  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateManagedFolder.](createmanagedfolder-operation.md)  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции FindFolder.](findfolder-operation.md)  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateItem.](createitem-operation.md)  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [GetItem.](getitem-operation.md)  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции UpdateItem.](updateitem-operation.md)  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [MoveItem.](moveitem-operation.md)  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CopyItem.](copyitem-operation.md)  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateAttachment.](createattachment-operation.md)  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [GetAttachment.](getattachment-operation.md)  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции FindItem.](finditem-operation.md)  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции ResolveNames.](resolvenames-operation.md)  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции ExpandDL.](expanddl-operation.md)  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса [на операцию Подписка.](subscribe-operation.md)  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса на операцию [GetEvents.](getevents-operation.md)  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса операции SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [SyncFolderHierarchy.](syncfolderhierarchy-operation.md)  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [SyncFolderItems.](syncfolderitems-operation.md)  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса [на операцию ConvertId.](convertid-operation.md)  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат запроса [операции AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [GetDelegate.](getdelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Содержит состояние и результат запроса [на операцию RemoveDelegate.](removedelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Содержит состояние и результат запроса на операцию [UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [GetServerTimeZones.](getservertimezones-operation.md)  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос [операции GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Определяет ответ на запрос [операции RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Содержит состояние и результаты ответа операции [FindConversation.](findconversation-operation.md)  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Содержит состояние и результаты запроса [операции ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции EmptyFolder.](emptyfolder-operation.md)  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Содержит состояние и результат запроса [операции UpdateInboxRules.](updateinboxrules-operation.md)  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [UploadItems.](uploaditems-operation.md)  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Содержит ответ на запрос [на операцию GetInboxRules](getinboxrules-operation.md) ****  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Содержит ответ на запрос [операции GetServiceConfiguration.](getserviceconfiguration-operation.md)  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение. В следующей таблице описываются значения, возвращаемые с помощью этого элемента.
  
|Значение|Описание|
|:-----|:-----|
|NoError  <br/> |Ошибка запроса не произошла.  <br/> |
|ErrorAccessDenied  <br/> |Эта ошибка возникает, когда учетная запись вызова не имеет прав на выполнение запрашиваемой меры.  <br/> |
|ErrorAccessModeSpecified  <br/> |Эта ошибка используется только для внутреннего использования. Эта ошибка не возвращается.  <br/> |
|ErrorAccountDisabled  <br/> |Эта ошибка возникает при отключении учетной записи.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Эта ошибка возникает, когда список с добавленными делегатами не удается сохранить.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Эта ошибка возникает, когда запись пространства адресов или доменное имя системы доменных имен (DNS) для межлесной доступности не удалось найти в базе данных Active Directory.  <br/> |
|ErrorADOperation  <br/> |Эта ошибка возникает при сбойе операции из-за проблем с связью с службами домена Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Эта ошибка возвращается, когда запрос операции **ResolveNames** указывает имя, которое не является допустимым.  <br/> |
|ErrorADUnavailable  <br/> |Эта ошибка возникает, когда AD DS недоступен. Попробуйте свой запрос еще раз позже.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Эта ошибка указывает, что **атрибут AffectedTaskOccurrences** не указан. Когда элемент [DeleteItem](deleteitem.md) используется для удаления по крайней мере одного элемента, который является задачей, и независимо от того, является ли эта задача повторяющейся или нет, атрибут **AffectedTaskOccurrences** должен быть указан, чтобы **DeleteItem** мог определить, следует ли удалять текущее событие или всю серию.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Указывает на ошибку при создании пути пути папки архива.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Указывает, что архивный почтовый ящик не включен.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Указывает, что обнаружение службы архивных почтовых ящиков не удалось.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Указывает, что была предпринята попытка создания элемента с более чем 10 вложенными вложениями. Это значение было введено в Exchange Server 2010 Пакет обновления 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |Элемент [CreateAttachment](createattachment.md) возвращает эту ошибку, если предпринята попытка создать вложения с размером, превышающий int32.MaxValue, в bytes.  <br/> Элемент [GetAttachment](getattachment.md) возвращает эту ошибку, если попытка получить существующее вложение с размером, превышающий int32.MaxValue, в bytes.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Эта ошибка указывает, что Exchange веб-службы пытались определить расположение межлесного компьютера, который работает Exchange 2010 г., который имеет роль сервера клиентского доступа, установленную с помощью службы автооткрытия, но вызов в службу автооткрытия не удалось.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Эта ошибка указывает, что сведения о конфигурации доступности для локального леса отсутствуют в AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Эта ошибка указывает на то, что при обработке элемента произошло исключение, и это исключение, скорее всего, произойдет для последующих элементов. Запросы могут включать несколько элементов; например, запрос на операцию GetItem может включать несколько идентификаторов. Как правило, элементы обрабатываются по одному. Если при обработке элемента возникает исключение, и это исключение, скорее всего, произойдет для последующих элементов, последующие элементы не будут обработаны.  <br/><br/>  Ниже следуют примеры ошибок, которые перестанут обрабатывать следующие элементы:<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Эта ошибка возникает при попытке перемещения или копирования повторяющегося элемента календаря.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Эта ошибка возникает при попытке обновления элемента календаря, расположенного в папке "Удаленные элементы", и при отправке обновлений или отмен собраний в соответствии со значением атрибута **SendMeetingInvitationsOrCancellations.** <br/><br/>Возможные значения для этого атрибута:  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>Однако такое обновление допускается только в том случае, если значение этого атрибута установлено для SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Эта ошибка возникает, когда вызвана операция UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem или SendItem, а указанный ID не является ИД возникновения любого повторяющегося элемента календаря.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Эта ошибка возникает, когда вызвана операция **UpdateItem,** **GetItem,** **DeleteItem,** **MoveItem,** **CopyItem** или **SendItem,** и указанный ID не является ID любого повторяющегося элемента.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem,** когда продолжительность элемента календаря превышает максимально допустимый срок, который в настоящее время составляет 5 лет.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Эта ошибка возникает, когда время окончания календаря заданной в одно и то же время или после начала.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Эта ошибка возникает, когда указанная папка для операции **FindItem** с элементом [CalendarView](calendarview.md) не имеет типа папки календаря.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Этот код ответа не используется.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem,** когда для определения шаблона изменения времени используются недопустимые значения Дня, WeekendDay и Weekday.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Эта ошибка возникает во время операции **CreateItem** или **UpdateItem,** когда для указания недельного повторения используются недействительные значения Day, WeekDay и WeekendDay.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Эта ошибка возникает, когда состояние двоичного большого объекта повторного хранения элементов календаря (BLOB) в Exchange является недействительным.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Этот код ответа не используется.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Эта ошибка возникает, когда указанное повторение невозможно создать.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Эта ошибка возникает, когда возникает недействительный часовой пояс.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Эта ошибка указывает на отмену элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Эта ошибка указывает на отмену элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Эта ошибка указывает на отмену элемента календаря.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Эта ошибка указывает на отмену элемента календаря.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Эта ошибка указывает, что элемент [AcceptItem](acceptitem.md) недействителен для элемента календаря или запроса на собрание в делегированном сценарии.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Эта ошибка указывает, что элемент [DeclineItem](declineitem.md) является недействительным для элемента календаря или запроса на собрание в делегированном сценарии.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Эта ошибка указывает, что элемент [RemoveItem](removeitem.md) недействителен для отмены собрания в делегированного сценария.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Эта ошибка указывает, что элемент [TentativelyAcceptItem](tentativelyacceptitem.md) недействителен для элемента календаря или запроса собрания в делегированном сценарии.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Эта ошибка указывает, что операция (в настоящее время CancelItem) в элементе календаря не допустима для участника. Отменить собрание может только организатор собрания.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Эта ошибка указывает, что [AcceptItem](acceptitem.md) является недействительным для элемента календаря организатора.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Эта ошибка указывает, что [declineItem](declineitem.md) является недействительным для элемента календаря организатора.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Эта ошибка указывает, что [RemoveItem](removeitem.md) является недействительным для элемента календаря организатора. Чтобы удалить собрание из календаря, организатор должен использовать CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Эта ошибка указывает, что [условноAcceptItem](tentativelyacceptitem.md) является недействительным для элемента календаря организатора.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Эта ошибка указывает на то, что запрос собрания устарел и не может быть обновлен.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Эта ошибка указывает на то, что индекс возникновения не указывает на возникновение в текущем повторе. Например, если шаблон повторения определяет набор из трех случаев собраний и вы пытаетесь получить доступ к пятому появлению, этот код отклика приведет к этому.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Эта ошибка указывает на то, что любая операция по удаляемой случайности (адресована с помощью повторяющегося мастера ID и индекса возникновения) является недействительной.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Эта ошибка сообщается в операциях CreateItem и UpdateItem для элементов календаря или свойств повторения задач, когда значение свойства находится вне диапазона. Например, указание пятнадцатой недели месяца приведет к этому коду ответа.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Эта ошибка возникает, когда диапазон "Начните с конца" для элемента [CalendarView](calendarview.md) превышает максимально допустимый срок в настоящее время 2 года.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Эта ошибка указывает на то, что учетная запись запроса не является допустимой учетной записью в базе данных каталога.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Указывает, что была предпринята попытка архивировать папку задач контактов календаря.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Указывает, что была предпринята попытка архивировать элементы в общедоступных папках.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Указывает, что была предпринята попытка архивировать элементы в почтовом ящике архива.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Эта ошибка возникает, когда элемент календаря создается, а атрибут **SavedItemFolderId** относится к папке, не являемой календарем.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Эта ошибка возникает, когда создается контакт и атрибут **SavedItemFolderId** относится к папке без контакта.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Эта ошибка указывает на то, что почтовый элемент не может быть создан в папке, кроме почтовой папки, например Calendar, Contact, Tasks, Notes и так далее.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Эта ошибка возникает, когда создается задача, а атрибут **SavedItemFolderId** относится к папке, не являемой задачей.  <br/> |
|ErrorCannotDeleteObject  <br/> |Эта ошибка возникает, когда удалить элемент или папку невозможно.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Операция [DeleteItem](deleteitem-operation.md) возвращает эту ошибку, когда не удается удалить текущее возникновение повторяющейся задачи. Это может произойти только в том случае, если атрибут **AffectedTaskOccurrences** был задан в SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Указывает, что была предпринята попытка отключить обязательное расширение.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Эта ошибка должна быть возвращена, если сервер не может очистить папку.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Указывает, что путь исходных папок не удалось получить.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Указывает, что сервер не мог получить внешний URL-адрес для Outlook Web App Параметры.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |Операция **GetAttachment** возвращает эту ошибку, если она не может получить тело вложения файла.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Эта ошибка указывает на то, что вызываемая ошибка попыталась установить разрешения календаря в папке, не вложенной в календарь.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Эта ошибка указывает на то, что вызываемая попыталась установить разрешения, не вложенные в календарь, в папку календаря.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Эта ошибка указывает на невозможность установить неизвестные разрешения в наборе разрешений.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Указывает, что была предпринята попытка указать папку поиска в качестве папки источника.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Эта ошибка возникает, когда запросу, требуемом идентификатору элемента, предоставляется идентификатор папки.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Эта ошибка возникает, когда запросу, требуемом идентификатору папки, предоставляется идентификатор элемента.  <br/> |
|ErrorChangeKeyRequired  <br/> |Этот код ответа был заменен **errorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Эта ошибка возвращается, когда ключ изменения элемента отсутствует или устарел. <br/><br/>Для операций SendItem, UpdateItem и UpdateFolder вызываемая должна передать правильный и текущий ключ изменения элемента. Обратите внимание, что это происходит с UpdateItem, даже если для разрешения конфликтов установлено всегда перезаписывать.  <br/> |
|ErrorClientDisconnected  <br/> |Указывает, что клиент был отключен.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorClientIntentNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorConnectionFailed  <br/> |Эта ошибка возникает, Exchange веб-службы не могут подключиться к почтовому ящику.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Эта ошибка указывает, что свойство, которое было проверено для фильтра Contains, не является типом строки.  <br/> |
|ErrorContentConversionFailed  <br/> |Операция **GetItem** возвращает эту ошибку, Exchange веб-службы не могут получить содержимое MIME для запрашиваемой номенклатуры. <br/><br/>Операция **CreateItem** возвращает эту ошибку, Exchange веб-службы не могут создать элемент из предоставленного контента MIME. Обычно это указывает на то, что свойство элемента повреждено или усечено.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Эта ошибка возникает, когда запрос на поиск выполнен с помощью параметра QueryString, а индексация контента не включена для целевого почтового ящика.  <br/> |
|ErrorCorruptData  <br/> |Эта ошибка возникает, когда данные повреждены и не могут быть обработаны.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Эта ошибка возникает, когда вызываемая не имеет разрешения на создание элемента.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Эта ошибка возникает, когда одна или несколько управляемых папок, указанных в запросе операции CreateManagedFolder, не были созданы. Поиск каждой папки, чтобы определить, какие папки были созданы и какие папки не существуют.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Эта ошибка возникает, когда учетная запись вызова не имеет разрешений, необходимых для создания подмостков.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Эта ошибка возникает при попытке переместить элемент или папку из одного почтового ящика в другой. Если исходный почтовый ящик и почтовый ящик назначения отличаются, вы получите эту ошибку.  <br/> |
|ErrorCrossSiteRequest  <br/> |Эта ошибка указывает, что запрос не разрешен, так как сервер клиентского доступа, который должен обслужить запрос, находится на другом сайте.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Эта ошибка может возникать в следующих сценариях:<br/>  <br/>— предпринята попытка доступа к элементу или записи свойства, а значение свойства слишком большое.<br/>- Длина кода содержимого MIME в XML запроса превышает предельно допустимую.<br/>- Размер тела существующего тела элемента превышает предел.<br/>- Потребитель пытается установить HTML или текстовое тело, длина которого (или совокупная длина в случае приложения) превышает ограничение. |
|ErrorDataSourceOperation  <br/> |Эта ошибка возникает, когда поставщик данных не завершает операцию.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Эта ошибка возникает в операции **AddDelegate,** когда указанный пользователь уже существует в списке делегатов.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Эта ошибка возникает в операции **AddDelegate,** когда указанный пользователь, который будет добавлен, является владельцем почтового ящика.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Эта ошибка возникает в операции **GetDelegate,** когда либо нет сведений о делегирования локального сообщения FreeBusy, либо нет публичного делегата Active Directory (в AD DS нет записи "Отправить от имени" или "Отправить от имени").  <br/> |
|ErrorDelegateNoUser  <br/> |Эта ошибка возникает, когда указанный пользователь не может быть соедино с пользователем в AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Эта ошибка возникает в операции **AddDelegate,** когда добавленный пользователь делегата не действителен.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Эта ошибка возникает при попытке удаления отличительной папки.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Эта ошибка указывает на то, что удостоверение пользователя не допустимо для операции. **DistinguishedUserType** не должен присутствовать в запросе.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Эта ошибка указывает на то, что член списка рассылки запросов не существует в списке рассылки.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Эта ошибка возникает при указании имен дублирующихся папок в элементе [FolderNames](foldernames.md) запроса **операции CreateManagedFolder.**  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Эта ошибка указывает на то, что имеются дубликаты заглавных окантов SOAP.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Эта ошибка указывает на то, что в наборе разрешений обнаружен дубликат пользовательского ИД, либо по умолчанию, либо анонимный, либо имеются дублирующиеся SID или получатели.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Эта ошибка возникает при попытке запроса создать или обновить параметры поиска папки поиска. Например, это может произойти, когда папка поиска создается в почтовом ящике, но папка поиска направлена на поиск в другом почтовом ящике.  <br/> |
|ErrorEventNotFound  <br/> |Эта ошибка возникает, когда событие, связанное с водяным знаком, удаляется перед возвращением события. Когда эта ошибка возвращается, подписка также удаляется.  <br/> |
|ErrorExceededConnectionCount  <br/> |Эта ошибка - iIndicates, что существует больше одновременно запросов к серверу, чем разрешено политикой пользователя.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Эта ошибка указывает на превышение максимального максимального абонентского счета политики регулирования для пользователя.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Эта ошибка указывает на то, что вызов операции поиска превысил общее число возвращаемого элементов.  <br/> |
|ErrorExpiredSubscription  <br/> |Эта ошибка возникает, если операция [GetEvents](getevents-operation.md) называется как подписка удаляется из-за истечения срока действия.  <br/> |
|ErrorExtensionNotFound  <br/> |Указывает, что расширение не найдено.  <br/> |
|ErrorFolderCorrupt  <br/> |Эта ошибка возникает, когда папка повреждена и не может быть сохранена.  <br/> |
|ErrorFolderExists  <br/> |Эта ошибка возникает при попытке создать папку с тем же именем, что и другая папка в том же родительском. Дублировать имена папок запрещено.  <br/> |
|ErrorFolderNotFound  <br/> |Эта ошибка указывает, что указанный ID папки не соответствует допустимой папке или что у делегата нет разрешения на доступ к папке.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Эта ошибка указывает на то, что запрашиваемую свойство не удалось получить. Это не указывает на то, что свойство не существует, но свойство было повреждено каким-то образом, чтобы не удалось найти.  <br/> |
|ErrorFolderSave  <br/> |Эта ошибка указывает на то, что папку нельзя создать или обновить из-за недействительного состояния.  <br/> |
|ErrorFolderSaveFailed  <br/> |Эта ошибка указывает на то, что папку нельзя создать или обновить из-за недействительного состояния.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Эта ошибка указывает на то, что папка не может быть создана или обновлена из-за недействительных значений свойств. Код ответа перечисляет, какие свойства привели к проблеме.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Эта ошибка указывает на то, что максимальное количество участников группы было достигнуто для получения сведений о свободной или загруженной занятости для списка рассылки.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Эта ошибка возвращается, когда из-за сбоя не удается получить бесплатные/загруженные сведения.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorImContactLimitReached  <br/> |Эта ошибка возвращается, когда новые контакты обмена мгновенными сообщениями не могут быть добавлены, так как достигнуто максимальное количество контактов. Эта ошибка была введена Exchange Server 2013 году.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Эта ошибка возвращается при попытке добавить имя отображения группы, когда существующая группа уже имеет одно и то же имя отображения. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorImGroupLimitReached  <br/> |Эта ошибка возвращается, когда новые группы мгновенных данных не могут быть добавлены, так как достигнуто максимальное число групп. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorImpersonateUserDenied  <br/> |Ошибка возвращается в случае авторизации от сервера к серверу для Exchange, когда вызываемая не имеет надлежащих прав на то, чтобы выдать себя за конкретного пользователя, о чем идет речь. Эта ошибка сопопоает с расширенным правом Active Directory на ms-Exch-EPI-May-Impersonate.  <br/> |
|ErrorImpersonationDenied  <br/> |Эта ошибка возвращается в авторизации от сервера к серверу для Exchange, когда вызываемая не имеет надлежащих прав на то, чтобы выдать себя через сервер клиентского доступа, на который он делает запрос. Это карта для ms-Exch-EPI-Impersonation расширенного права Active Directory.  <br/> |
|ErrorImpersonationFailed  <br/> |Эта ошибка указывает на неожиданную ошибку при попытке выполнить проверку подлинности от сервера к серверу. В этом коде ответа обычно указывается, что учетная запись службы, которая работает в пуле приложений Exchange веб-служб, настроена неправильно, что Exchange веб-службы не могут общаться с каталогом, или что доверие между лесами не настроено правильно.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Эта ошибка указывает, что запрос был действителен для текущей версии Exchange Server, но был недействительным для указанной версии сервера запроса.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Эта ошибка указывает, что каждое описание изменений в [элементах UpdateItem](updateitem.md) или [UpdateFolder](updatefolder.md) должно указывать только одно свойство для обновления.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Эта ошибка возникает, когда запрос содержит слишком много участников для решения. По умолчанию максимальное число участников для решения составляет 100.  <br/> |
|ErrorInsufficientResources  <br/> |Эта ошибка возникает при перегрузке сервера почтовых ящиков. Попробуйте свой запрос еще раз позже.  <br/> |
|ErrorInternalServerError  <br/> |Эта ошибка указывает, что Exchange веб-службы столкнулись с ошибкой, из которой она не могла восстановиться, а более конкретного кода ответа, связанного с ошибкой, которая произошла, не существует.  <br/> |
|ErrorInternalServerTransientError  <br/> |Эта ошибка указывает на то, что произошла внутренняя ошибка сервера и что вы должны попробовать свой запрос еще раз позже.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Эта ошибка указывает на то, что уровень доступа, который имеет вызываемая на бесплатных и загруженных данных, является недействительным.  <br/> |
|ErrorInvalidArgument  <br/> |Эта ошибка указывает на ошибку, вызванную всеми недействительными аргументами, переданными в операцию [GetMessageTrackingReport.](getmessagetrackingreport-operation.md)<br/><br/> Эта ошибка возвращается в следующих сценариях: <br/><br/>— Пользователь, указанный в параметре  _sending-as,_ не существует в каталоге. <br/>— Пользователь, указанный в  _параметре sending-as,_ не является уникальным в каталоге. <br/>-  _Адрес отправки как_ пуст.<br/>-  _Адрес отправки не_ является допустимым адресом электронной почты.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Эта ошибка возвращается операцией [GetAttachment](getattachment-operation.md) или [операцией DeleteAttachment,](deleteattachment-operation.md) когда вложение, соответствующее указанному ID, не найдено.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Эта ошибка возникает при попытке привязки к существующей папке поиска с помощью сложного ограничения таблицы вложений. Exchange Веб-службы поддерживают только простые фильтры для таблицы вложений. Если вы попытаетесь связаться с существующей папкой поиска, имеющей более сложное ограничение таблицы вложений (подфильтратор), Exchange веб-службы не могут отрисовывать XML для этого фильтра и возвращают этот код отклика. <br/><br/>Обратите внимание, что вы по-прежнему можете вызвать операцию GetFolder в папке, но не запрашивать элемент [SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Эта ошибка возникает при попытке привязки к существующей папке поиска с помощью сложного ограничения таблицы вложений. Exchange Веб-службы поддерживают только простые фильтры для таблицы вложений. <br/><br/>Если вы пытаетесь связаться с существующей папкой поиска с более сложным ограничением таблицы вложений, Exchange веб-службы не могут отрисовывать XML для этого фильтра. В этом случае подфильтр вложения содержит текстовый фильтр, но не смотрит на имя отображения вложения.<br/><br/> Обратите внимание, что вы по-прежнему можете вызвать операцию GetFolder в папке, но не запрашивать элемент [SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Эта ошибка указывает на сбой процедуры авторизации запросителя.  <br/> |
|ErrorInvalidChangeKey  <br/> |Эта ошибка возникает, когда потребитель передает в папку или идентификатор элемента с ключом изменения, который не может быть размазнут. Например, это может быть недействительный контент base64 или пустая строка.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Эта ошибка указывает на то, что при попытке устранить удостоверение вызывающего пользователя была допущена внутренняя ошибка.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Эта ошибка возвращается при попытке установить значение [элемента CompleteDate](completedate.md) задачи на время в будущем. При преобразовании в локальное время сервера клиентского доступа значение [CompleteDate](completedate.md) задачи не может быть установлено к значению, которое превышает местное время на сервере клиентского доступа.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Эта ошибка указывает на то, что для контакта был предоставлен недействительный адрес электронной почты.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Эта ошибка указывает, что для записи электронной почты было предоставлено значение недействительных индексов электронной почты.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Эта ошибка возникает, когда учетные данные, используемые для прокси-запроса в лес службы каталогов, не удается проверить подлинность.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Эта ошибка указывает на то, что указанные разрешения папок являются недействительными.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Эта ошибка указывает, что указанный пользовательский ID делегата является недействительным.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Эта ошибка возникает во время Exchange, когда вызываемая не указывает upN, адрес электронной почты или пользовательский SID. Это также произойдет, если звонячий указывает одно или несколько из них, а значения пусты.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Эта ошибка возникает, когда битмаска, которая была передана в ограничение элемента [Excludes,](excludes.md) не может быть разрезана.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Эта ошибка возникает при следующих событиях: <br/> <br/>- Вызываемая служба пытается использовать расширенное свойство, которое не поддерживается Exchange веб-службами.  <br/>- Вызываемая передается в недействительное сочетание значений атрибута для расширенного свойства. Это также происходит, если атрибуты не передаются. Разрешены только определенные комбинации.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Эта ошибка возникает, когда раздел значения расширенного свойства не соответствует типу свойства. <br/><br/>Например, при настройке расширенного свойства, которое имеет PropertyType="String" для массива integers, это приведет к этой ошибке. Любое представление строки, не принудительное к типу, указанному для расширенного свойства, даст эту ошибку.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Эта ошибка указывает на то, что отправитель приглашений общего доступа не создал метаданные приглашения общего доступа.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Эта ошибка указывает, что сообщение общего доступа не предназначено для вызываемой.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Эта ошибка указывает на то, что объекты федерации организации запросителя не настроены правильно.  <br/> |
|ErrorInvalidFolderId  <br/> |Эта ошибка возникает при поврежденном ID папки.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Эта ошибка указывает, что указанный тип папки является недействительным для текущей операции. Например, нельзя создать папку Поиска в общедоступных папках.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Эта ошибка возникает при дробной прогонах, когда пользователь указал один из следующих ниже. <br/> <br/>— числитель, который больше, чем знаменатель  <br/>— числитель, который меньше нуля  <br/>- Знаменатель, который меньше или равен нулю  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Эта ошибка указывает, что элементы [DataType](datatype.md) и ShareFolderId присутствуют в запросе.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Эта ошибка возникает, когда [операция GetUserAvailability](getuseravailability-operation.md) вызвана [с помощью FreeBusyViewType](freebusyviewtype.md) none.  <br/> |
|ErrorInvalidId  <br/> |Эта ошибка указывает на то, что ключ ID и(или) изменения имеет неправильное значение.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Эта ошибка возникает, когда вызываемая указывает пустой атрибут **Id.**  <br/> |
|ErrorInvalidLikeRequest  <br/> |Эта ошибка возникает, когда элемент не может понравиться. Версии Exchange со сборкой 15.00.0913.09 включают это значение.  <br/> |
|ErrorInvalidMalformed  <br/> |Эта ошибка возникает при указании недооформленного атрибута **Id** вызываемого вызываемого.  <br/> |
|ErrorInvalidMalformedEwsLegacyIdFormat  <br/> |Эта ошибка указывает на то, что папка или ID элемента, использующий формат 2007 Exchange 2007, была указана для запроса с версией Exchange 2007 sp1 или более поздней версии. Вы не можете использовать Exchange 2007 в запросах Exchange 2007 sp1 или более поздних. Для их преобразования сначала необходимо использовать операцию [ConvertId.](convertid-operation.md)  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Эта ошибка возникает, когда звонячий указывает слишком длинный атрибут **Id.**  <br/> |
|ErrorInvalidNotAnItemAttachmentId  <br/> |Эта ошибка возвращается всякий раз, когда ID, который не является ИД вложения элементов, передается методу веб-службы, который ожидает ИД вложения.  <br/> |
|ErrorInvalidReturnedByResolveNames  <br/> |Эта ошибка возникает при поврежденном контакте в почтовом ящике.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Эта ошибка возникает, когда звонячий указывает слишком длинный атрибут **Id.**  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Эта ошибка возвращается, когда иерархия вложений на элементе превышает максимум 255 уровней глубиной.  <br/> |
|ErrorInvalidIdXml  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidImContactId  <br/> |Эта ошибка возвращается, когда указанный идентификатор контакта с мгновенными данными не представляет допустимого идентификатора. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Эта ошибка возвращается, когда указанный идентификатор адреса SMTP группы рассылки im не представляет допустимого идентификатора. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidImGroupId  <br/> |Эта ошибка возвращается, когда указанный идентификатор группы im не представляет допустимого идентификатора. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Эта ошибка возникает, если смещение для индексации пробок является отрицательным.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Указывает, что элемент недействителен для **операции ArchiveItem.**  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Эта ошибка возникает при попытке использования объекта ответа AcceptItem для типа элемента, кроме запроса собрания или элемента календаря, или при попытке принять возникновение элементов календаря, который находится в папке "Удаленные элементы".  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Эта ошибка возникает при попытке использования объекта ответа CancelItem в типе элемента, кроме элемента календаря.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Эта ошибка возвращается при попытке создания вложения элемента неподтвердимого типа.  <br/><br/>  Поддерживаемые типы элементов для вложений элементов включают следующие объекты:  <br/><br/>- [Item](item.md) <br/>- [Сообщение](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Задача](task.md) <br/>- [Контакт](contact.md) <br/> <br/> Например, при попытке создания вложения [MeetingMessage](meetingmessage.md) вы столкнетесь с этим кодом ответа.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Эта ошибка возвращается из операции [CreateItem,](createitem-operation.md) если запрос содержит неподтвердимый тип элемента. <br/><br/>Поддерживаемые элементы включают следующие объекты:<br/>  <br/>- [Item](item.md) <br/>- [Сообщение](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Задача](task.md) <br/>- [Контакт](contact.md) <br/><br/>  Некоторые типы создаются как побочный эффект от действия чего-то другого. Например, сообщения собраний создаются при отправке элемента календаря участникам; они явно не создаются.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Эта ошибка возникает при попытке использования объекта ответа DeclineItem для типа элемента, кроме запроса собрания или элемента календаря, или при попытке отклонит возникновение элементов календаря, который находится в папке "Удаленные элементы".  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Эта ошибка указывает, что операция [ExpandDL](expanddl-operation.md) действительна только для частных списков рассылки.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Эта ошибка возвращается из объекта ответа RemoveItem, если в запросе указан элемент, который не является элементом отмены собрания.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Эта ошибка возвращается из операции [SendItem,](senditem-operation.md) если в запросе указан элемент, который не является элементом сообщения.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Эта ошибка возникает при попытке использования [ПредварительноAcceptItem](tentativelyacceptitem.md) для типа элемента, кроме запроса собрания или элемента календаря, или при попытке предварительно принять появление элементов календаря, который находится в папке "Удаленные элементы".  <br/> |
|ErrorInvalidLogonType  <br/> |Эта ошибка используется только для внутреннего использования. Эта ошибка не возвращается.  <br/> |
|ErrorInvalidMailbox  <br/> |Эта ошибка указывает на сбой операции [CreateItem](createitem-operation.md) или [операции UpdateItem](updateitem-operation.md) при создании или обновлении личного списка рассылки.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Эта ошибка возникает, когда структура управляемой папки повреждена и не может быть отрисовка.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Эта ошибка возникает, когда квота, установленная в управляемой папке, меньше нуля, что указывает на поврежденную управляемой папку.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Эта ошибка возникает, когда размер, заданной в управляемой папке, меньше нуля, что указывает на поврежденную управляемой папку.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Эта ошибка возникает, когда поставляемая слитая свободная/занятая внутренняя ценность является недействительной. Минимальное значение по умолчанию — 5 минут. Максимальное значение по умолчанию — 1440 минут.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Эта ошибка возникает, когда имя является недействительным для [операции ResolveNames.](resolvenames-operation.md) Например, строка нулевой длины, одно пространство, запятая и тире — это все недействительные имена.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Эта ошибка указывает на ошибку в учетной записи сетевой службы на сервере клиентского доступа.  <br/> |
|ErrorInvalidOofParameter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidOperation  <br/> | Это общая ошибка, которая используется, когда запрашиваемая операция недействительна. <br/><br/>Например, вы не можете сделать следующее: <br/> <br/>- Выполните "глубокий" обход с помощью операции [FindFolder](findfolder-operation.md) в общедоступных папках.  <br/>- Перемещение или копирование корневой папки общего государственного.  <br/>- Удалите связанный элемент с помощью любого режима, кроме "Hard" delete.  <br/>- Перемещение или копирование связанного элемента.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Эта ошибка указывает на то, что вызываемая пользователь запрашивает бесплатные или занятые сведения для пользователя в другой организации, но в организационных отношениях не включено бесплатное/занятое.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Эта ошибка возникает, когда потребитель передает в ноль или отрицательное значение для возвращаемой максимальной строки.  <br/> |
|ErrorInvalidParentFolder  <br/> |Эта ошибка возникает, когда потребитель передает недействительные родительские папки для операции. Например, эта ошибка возвращается при попытке создания папки в папке поиска.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Эта ошибка возвращается при попытке установить процент завершения задачи до недействительных значений. Значение должно быть от 0 до 100 (включительно).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Эта ошибка указывает на то, что уровень разрешений не соответствует настройкам разрешений.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Эта ошибка указывает на то, что идентификатор вызываемой связи не действителен.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Эта ошибка указывает на то, что номер телефона не соответствует правилам набора номера.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Эта ошибка возникает, когда свойство, к которое вы пытаетесь приметь, не поддерживает приложение. <br/><br/>Ниже приводится только одно из свойств, поддерживаюющих приложение: <br/> <br/>- Коллекции получателей (ToRecipients, CcRecipients, BccRecipients)  <br/>- Коллекции участников (RequiredAttendees, OptionalAttendees, Resources)  <br/>- Body  <br/>- ReplyTo  <br/><br/>  Кроме того, эта ошибка возникает при добавлении тела сообщения, если указанный в запросе формат не соответствует формату элемента в магазине.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Эта ошибка возникает, если операция удаления указана в операции [UpdateItem](updateitem-operation.md) или вызове операции [UpdateFolder](updatefolder-operation.md) для свойства, которое не поддерживает операцию удаления. Например, нельзя удалить элемент [ItemId](itemid.md) объекта [Item.](item.md)  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Эта ошибка возникает, если потребитель проходит в одном из свойств флага в [фильтре Существует.](exists.md) Например, эта ошибка возникает, если [флаги IsRead](isread.md) или [IsFromMe](isfromme.md) указаны в [элементе Exists.](exists.md) Вместо этого в запросе должен быть элемент [IsEqualTo,](isequalto.md) так как они являются флагами и, следовательно, частью одного свойства.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Эта ошибка возникает, когда свойство, которое вы пытаетесь манипулировать, не поддерживает выполняемую на нем операцию.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Эта ошибка возникает, если свойство, указанное в запросе, не доступно для типа элемента. Например, эта ошибка возвращается, если свойство, доступное только для элементов календаря, запрашивается в вызове операции [GetItem](getitem-operation.md) для сообщения или обновляется в вызове операции [UpdateItem](updateitem-operation.md) для сообщения. <br/> <br/>  Это происходит в следующих операциях: <br/> <br/>- [Операция GetItem](getitem-operation.md) <br/>- [Операция GetFolder](getfolder-operation.md) <br/>- [Операция UpdateItem](updateitem-operation.md) <br/>- [Операция UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Эта ошибка указывает на то, что свойство, которое вы пытаетесь манипулировать, не поддерживает выполняемую на нем операцию. Например, эта ошибка возвращается, если свойство, которое вы пытаетесь установить, является только для чтения.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Эта ошибка возникает во время [операции UpdateItem,](updateitem-operation.md) когда клиент пытается обновить определенные свойства уже отправленного сообщения.<br/><br/> Например, следующие свойства не могут быть обновлены в отправленном сообщении: <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Эта ошибка возникает при вызове операции [GetEvents](getevents-operation.md) или операции отписки с помощью push-имени подписки. [](unsubscribe-operation.md) Чтобы отписаться от push-подписки, необходимо ответить на запрос push с отписавным ответом или отключить веб-службу и дождаться времени ожидания push-уведомлений.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Эта ошибка возвращается операцией [Подписка,](subscribe-operation.md) когда создается подписка "push" и указывает, что URL-адрес, включенный в запрос, является недействительным.<br/><br/>Чтобы принять URL-адрес, Exchange веб-службы должны быть выполнены следующие условия. <br/> <br/>- Длина \> строки 0 и \< 2083.  <br/> протокол https или https.  <br/>- URL-адрес может быть разрисовыт классом microsoft платформа .NET Framework URI.  <br/> |
|ErrorInvalidRecipients  <br/> |Эта ошибка указывает, что коллекция получателей в вашем сообщении или коллекция участников в элементе календаря недействительна. Например, эта ошибка возвращается при попытке отправки элемента без получателей.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Эта ошибка указывает на то, что в папке поиска имеется фильтр таблицы получателей, Exchange веб-службы не могут представлять. Чтобы обойти эту ошибку, извлекать папку без запроса параметров поиска.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Эта ошибка указывает на то, что в папке поиска имеется фильтр таблицы получателей, Exchange веб-службы не могут представлять. Чтобы обойти эту ошибку, извлекать папку без запроса параметров поиска.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Эта ошибка указывает на то, что в папке поиска имеется фильтр таблицы получателей, Exchange веб-службы не могут представлять. Чтобы обойти эту ошибку, извлекать папку без запроса параметров поиска.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Эта ошибка указывает на то, что в папке поиска имеется фильтр таблицы получателей, Exchange веб-службы не могут представлять. Чтобы обойти эту ошибку, извлекать папку без запроса параметров поиска.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Эта ошибка возвращается из операции [CreateItem](createitem-operation.md) для объектов ответа forward и Response в следующих сценариях:<br/>  <br/>- Идентификатор ссылаемого элемента не является [сообщением,](message-ex15websvcsotherref.md) [calendarItem](calendaritem.md)или потомком **сообщения** или **CalendarItem.**  <br/>— идентификатор эталонного элемента для **CalendarItem,** и организатор пытается ответить или ответить на него самому.  <br/>- Сообщение является черновиком и выбирается Ответ или ReplyAll.  <br/>- Эталонный элемент [для SuppressReadReceipt](suppressreadreceipt.md)не является сообщением или потомком **сообщения.**   <br/> |
|ErrorInvalidRequest  <br/> |Эта ошибка возникает, когда в запросе SOAP есть заголовка действий SOAP, но ничего в теле SOAP. Обратите внимание, что заголовка soap Action не требуется, так как Exchange веб-службы могут определить способ вызова из локального имени корневого элемента в теле SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Эта ошибка возвращается, когда указанный тег хранения имеет неправильное действие, связанное с ним. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Эта ошибка возвращается при попытке установить несущестуционный или невидимый тег в **свойстве PolicyTag.** Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Эта ошибка возвращается при попытке установить неявный тег в **свойстве PolicyTag.** Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Указывает, что GUID тега хранения был недействительным.  <br/> |
|ErrorInvalidRoutingType  <br/> |Эта ошибка возникает, если тип маршрутирования, переданный для элемента [RoutingType (EmailAddressType),](routingtype-emailaddresstype.md) является недействительным. Как правило, тип маршрутивки за набором простого протокола передачи почты (SMTP).  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Эта ошибка возникает, если указанное время окончания продолжительности не превышает время начала или не произойдет в будущем.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Эта ошибка указывает на то, что прокси-запрос, отправленный на другой сервер, не может обслужить запрос из-за несоответствия версии.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Эта ошибка указывает на то Exchange дескриптор безопасности в папке Calendar в магазине поврежден.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Эта ошибка возникает при попытке отправить элемент, в котором в запросе [указана сохраненнаяItemFolderId,](saveditemfolderid.md) но свойство **SaveItemToFolder** задано как **ложное.**  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Эта ошибка указывает на то, что маркер, переданный в загоне, имеет неправильное образование, не ссылается на допустимую учетную запись в каталоге или отсутствует основная группа **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Эта ошибка указывает на то, что метаданные общего доступа не допустимы. Это может быть вызвано недействительным XML.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Эта ошибка указывает на то, что сообщение общего доступа не является допустимым. Это может быть вызвано отсутствием свойства.  <br/> |
|ErrorInvalidSid  <br/> |Эта ошибка возникает, когда недействительный SID передается в запросе.  <br/> |
|ErrorInvalidSIPUri  <br/> |Эта ошибка указывает, что имя SIP, телефонный план или номер телефона являются недействительными URL-адресами SIP.  <br/> |
|ErrorInvalidServerVersion  <br/> |Эта ошибка указывает на то, что в запросе указана недействительный версия сервера запроса.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Эта ошибка возникает, когда адрес SMTP не может быть размыт.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidSubscription  <br/> |Эта ошибка указывает на то, что подписка больше не действительна. Это может быть из-за перезапуска сервера клиентского доступа или из-за истечения срока действия подписки.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Эта ошибка указывает, что запрос на подписку включал несколько общедоступных папок. Подписка может включать несколько папок из одного почтового ящика или одного общего ИД папок.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Эта ошибка возвращается [SyncFolderItems](syncfolderitems.md) или [SyncFolderHierarchy,](syncfolderhierarchy.md) если переданные данные [SyncState](syncstate-ex15websvcsotherref.md) недействительны. Чтобы устранить эту ошибку, необходимо повторно ресинхронизироваться без состояния синхронизации. Убедитесь, что при сохраняющихся BLOBs состояния синхронизации не случайно усечена BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Эта ошибка указывает, что указанный интервал времени является недействительным. Время начала должно быть больше или равно конечному времени.  <br/> |
|ErrorInvalidUserInfo  <br/> |Эта ошибка указывает на то, что для операции разрешений был указан внутренний несогласованный [UserId.](userid.md) Например, если указан отличительный пользовательский ID (по умолчанию или анонимный), эта ошибка возвращается, если вы также пытаетесь указать SID, или основной SMTP-адрес или отображать имя этого пользователя.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Эта ошибка указывает на то, что параметры Office (OOF) недействительны из-за отсутствующих внутренних или внешних ответов.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Эта ошибка возникает во время Exchange обезличения. Вызываемая в недействительном upN в загон SOAP, которая была недоступна в каталоге.  <br/> |
|ErrorInvalidUserSid  <br/> |Эта ошибка возникает, когда недействительный SID передается в запросе.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Этот код ответа не используется.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Эта ошибка указывает, что значение сравнения в ограничении является недействительным для свойства, которое вы сравниваете.<br/><br/> Например, значение сравнения [True DateTimeCreated](datetimecreated.md)  >   возвращает этот код ответа. <br/><br/>Этот код ответа также возвращается, если в сопоставлении указывается свойство переумеления, но значение, которое вы сравниваете, не является допустимым значением для этого переумерия.  <br/> |
|ErrorInvalidWatermark  <br/> |Эта ошибка вызвана недействительным водяным знаком.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Эта ошибка указывает на то, что допустимый шлюз VoIP не доступен.  <br/> |
|ErrorIrresolvableConflict  <br/> |Эта ошибка указывает на то, что разрешение конфликтов не удалось разрешить изменения свойств. Элементы в магазине, возможно, были изменены и должны быть обновлены. Извлечение обновленного ключа изменения и попробуйте еще раз.  <br/> |
|ErrorItemCorrupt  <br/> |Эта ошибка указывает на то, что состояние объекта повреждено и не может быть извлечено. При обнаружении элемента в этом состоянии будут только определенные элементы, такие как [Body](body.md) и [MimeContent.](mimecontent.md) Опустить эти элементы и повторить операцию.  <br/> |
|ErrorItemNotFound  <br/> |Эта ошибка возникает, когда элемент не найден или у вас нет разрешения на доступ к элементу.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Эта ошибка возникает в случае с ошибкой запроса свойства на элемент. Свойство может существовать, но его не удалось получить.  <br/> |
|ErrorItemSave  <br/> |Эта ошибка возникает, когда попытки сохранить элемент или папку сбой.  <br/> |
|ErrorItemSavePropertyError  <br/> |Эта ошибка возникает при срыве попыток сохранить элемент или папку из-за недействительных значений свойств. Код ответа включает путь недействительных свойств.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Этот код ответа не используется.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Этот код ответа не используется.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Эта ошибка указывает на то, что служба доступности не смогла войти в систему в качестве сетевой службы для прокси-запросов на соответствующие сайты или леса. Этот ответ обычно указывает на ошибку конфигурации.  <br/> |
|ErrorMailboxConfiguration  <br/> |Эта ошибка указывает, что сведения о почтовых ящиках в AD DS настроены неправильно.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Эта ошибка указывает, что элемент [MailboxDataArray](mailboxdataarray.md) в запросе пуст. Необходимо предоставить по крайней мере один идентификатор почтового ящика.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Эта ошибка возникает при поставке более 100 записей в [элементе MailboxDataArray.](mailboxdataarray.md)  <br/> |
|ErrorMailboxFailover  <br/> |Эта ошибка указывает на то, что попытка доступа к почтовому ящику не удалась, так как почтовый ящик находится в процессе сбоя.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Указывает, что удержание почтового ящика не найдено.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Эта ошибка возникает при сбое подключения к почтовому ящику для получения сведений о представлении календаря.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Эта ошибка указывает на то, что почтовый ящик перемещается в другой магазин почтовых ящиков или сервер. Эта ошибка также может указывать на то, что почтовый ящик находится на другом сервере или базе данных почтовых ящиков.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Эта ошибка указывает на то, что произошло одно из следующих условий ошибки:  <br/><br/>- Магазин почтовых ящиков поврежден.  <br/>- Хранилище почтовых ящиков остановлено.  <br/>- Магазин почтовых ящиков находится в автономном режиме.  <br/>— Ошибка сети произошла при попытке доступа к магазину почтовых ящиков.  <br/>- Хранилище почтовых ящиков перегружено и не может принимать больше подключений.  <br/>— Приостановка хранения почтовых ящиков.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Эта ошибка возникает, если данные элемента [MailboxData](mailboxdata.md) не могут быть соотданы с допустимой учетной записью почтового ящика.  <br/> |
|ErrorMailTipsDisabled  <br/> |Эта ошибка указывает на отключение советов почты.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Эта ошибка возникает, если управляемой папки, которую вы пытаетесь создать, уже существует в почтовом ящике.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Эта ошибка возникает, когда имя папки, указанное в запросе, не сооперна с определением управляемой папки в AD DS. Можно создавать экземпляры управляемых папок только для папок, определенных в AD DS. Проверьте имя и попробуйте еще раз.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Эта ошибка указывает, что корень управляемых папок был удален из почтового ящика или что папка существует в одной родительской папке с именем корневой папки управляемых папок. Это также произойдет, если попытка создания корневой управляемой папки не удалась.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Эта ошибка указывает на то, что при попытке создания предложений у двигателя предложений возникла проблема.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Эта ошибка возникает, если атрибут **MessageDisposition** не заданной.<br/><br/> Этот атрибут необходим для следующих: <br/> <br/>- Операция [CreateItem и](createitem-operation.md) [операция UpdateItem](updateitem-operation.md) при создании или обновлении элемента [является сообщением.](message-ex15websvcsotherref.md)  <br/>- [CancelCalendarItem,](cancelcalendaritem.md) [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)или [TentativelyAcceptItem](tentativelyacceptitem.md) response objects.  <br/> |
|ErrorMessageSizeExceeded  <br/> |Эта ошибка указывает, что сообщение, которое вы пытаетесь отправить, превышает допустимые ограничения.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Эта ошибка указывает, что данный домен не может быть найден.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Эта ошибка указывает на то, что служба отслеживания сообщений не может отслеживать сообщение.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Эта ошибка указывает на то, что служба отслеживания сообщений либо не загружена, либо занята. Этот код ошибки указывает на переходную ошибку. Клиенты могут повторно подключиться к серверу при получении этой ошибки.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Эта ошибка возникает, когда содержимое MIME не является допустимым iCal для [операции CreateItem.](createitem-operation.md) Для операции [GetItem](getitem-operation.md)этот ответ указывает на то, что контент MIME не может быть создан.  <br/> |
|ErrorMimeContentInvalid  <br/> |Эта ошибка возникает, когда содержимое MIME является недействительным.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Эта ошибка возникает, когда содержимое MIME в запросе не является допустимой строкой 64.  <br/> |
|ErrorMissingArgument  <br/> |Эта ошибка указывает, что в запросе отсутствует необходимый аргумент. В тексте сообщения ответа указывается, какой аргумент следует проверить.  <br/> |
|ErrorMissingEmailAddress  <br/> |Эта ошибка указывает на то, что в запросе указан отличительный ИД папки, но учетная запись, которая сделала запрос, не имеет почтового ящика в системе. В этом случае необходимо предоставить под элемент [почтовых](mailbox.md) ящиков в [соответствии с DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Эта ошибка указывает на то, что в запросе указан отличительный ИД папки, но учетная запись, которая сделала запрос, не имеет почтового ящика в системе. В этом случае необходимо предоставить под элемент [почтовых](mailbox.md) ящиков в [соответствии с DistinguishedFolderId](distinguishedfolderid.md). Этот ответ возвращается из [операции CreateManagedFolder.](createmanagedfolder-operation.md)  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Эта ошибка возникает, если элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) отсутствует.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Эта ошибка возникает, если [отсутствует ReferenceItemId.](referenceitemid.md)  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Этот код ошибки никогда не возвращается.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Эта ошибка возвращается при попытке не включать элемент элемента в элемент **ItemAttachment** запроса на операцию [CreateAttachment.](createattachment-operation.md)  <br/> |
|ErrorMissingManagedFolderId  <br/> |Эта ошибка возникает, когда свойство IDs политики, тег свойства 0x6732, для папки отсутствует. Вы должны считать это поврежденной папкой.  <br/> |
|ErrorMissingRecipients  <br/> |Эта ошибка указывает на то, что вы пытались отправить элемент без использования получателей. Обратите внимание, что при вызове операции [CreateItem](createitem-operation.md) с диспозицией сообщения, которая вызывает отправление сообщения, вы получите следующий код ответа: **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Эта ошибка указывает на то, что [userId](userid.md) не был полностью указан в наборе разрешений.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Эта ошибка указывает, что в запросе указано несколько значений элемента [ExchangeImpersonation.](exchangeimpersonation.md)  <br/> |
|ErrorMoveCopyFailed  <br/> |Эта ошибка указывает на сбой операции перемещения или копирования. Перемещение происходит в операции [CreateItem](createitem-operation.md) при приеме запроса на собрание, который находится в папке "Удаленные элементы". Кроме того, при отклонении запроса на собрание, отмене элемента календаря или удалении собрания из календаря он перемещается в папку "Удаленные элементы".  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Эта ошибка возникает, если вы пытаетесь переместить отличимую папку.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Эта ошибка возникает, когда запрос пытается получить доступ к нескольким серверам почтовых ящиков. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Эта ошибка возникает, если операция [ResolveNames](resolvenames-operation.md) возвращает несколько результатов или неоднозначное имя, указанное вами, соответствует более чем одному объекту в каталоге. Код ответа содержит совпадают имена в данных отклика.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Эта ошибка указывает на то, что у вызываемой в системе нет почтового ящика. Операция [ResolveNames или](resolvenames-operation.md) [Операция ExpandDL](expanddl-operation.md) недействительна для подключения пользователя без почтового ящика.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Эта ошибка указывает на то, что операция [ResolveNames](resolvenames-operation.md) не возвращает результатов.  <br/> |
|ErrorNoApplicableProxyCASErversAvailable  <br/> |Этот код ошибки должен быть возвращен, если веб-служба не может найти сервер для обработки запроса.  <br/> |
|ErrorNoCalendar  <br/> |Эта ошибка возникает, если для почтового ящика нет папки Calendar.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Эта ошибка указывает на то, что запрос ссылается на почтовый ящик на другом сайте Active Directory, но серверы клиентского доступа на сайте назначения не были настроены для Windows проверки подлинности, и поэтому запрос не может быть заявляем.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Эта ошибка указывает на то, что запрос ссылается на почтовый ящик на другом сайте Active Directory, но серверы клиентского доступа на сайте назначения не были настроены для подключений SSL, и поэтому запрос не мог быть подключен.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Эта ошибка указывает на то, что запрос ссылается на почтовый ящик на другом сайте Active Directory, но никакие серверы клиентского доступа на сайте назначения не были приемлемой версией продукта для получения запроса, и поэтому запрос не мог быть прокси-сервером.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Эта ошибка возникает, если вы установите элемент [FolderClass](folderclass.md) при создании элемента, кроме общей папки. Для впечатаемых папок, таких как [CalendarFolder](calendarfolder.md) и [TasksFolder,](tasksfolder.md)подразумевается класс папок. Настройка класса папки для другого типа папок с помощью операции [UpdateFolder](updatefolder-operation.md) приводит к **ответу ErrorObjectTypeChanged.** Вместо этого используйте тип общих папок, но установите класс папки до требуемого значения. Exchange Веб-службы создадут правильную папку строго введите.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Эта ошибка указывает на то, что вызываемая не имеет прав на просмотр в папке Календарь.  <br/> |
|ErrorNonExistentMailbox  <br/> | Эта ошибка возникает в следующих сценариях: <br/> <br/>- Адрес электронной почты пуст в [CreateManagedFolder](createmanagedfolder.md).  <br/>- Адрес электронной почты не относится к допустимой учетной записи в запросе, который принимает адрес электронной почты в теле или в заголовке SOAP, например в вызове Exchange impersonation.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Эта ошибка возникает при переходе вызываемого в адрес SMTP, который не является основным. Ответ включает правильный smTP-адрес для использования.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Эта ошибка указывает на то, что свойства MAPI в настраиваемом диапазоне, 0x8000 и больше, не могут ссылаться на теги свойств. Необходимо использовать свойство EWS Managed API [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)или элемент EWS [ExtendedFieldURI](extendedfielduri.md) с атрибутом PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Этот код ответа не используется.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Этот код ошибки должен быть возвращен, если не доступен сервер общедоступных папок или если у вызываемой не имеется домашнего общего сервера.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Эта ошибка указывает на то, что запрос ссылается на почтовый ящик на другом сайте Active Directory, но ни один из серверов клиентского доступа на этом сайте не ответил, и поэтому запрос не мог быть прокси-сервером.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Эта ошибка указывает на то, что звонивка пыталась предоставить разрешения в календаре или папке контактов пользователю в другой организации, и попытка не удалась.  <br/> |
|ErrorNotDelegate  <br/> |Эта ошибка указывает, что пользователь не является делегатом для почтового ящика. Он возвращается операцией [GetDelegate,](getdelegate-operation.md)операцией [RemoveDelegate](removedelegate-operation.md)и операцией [UpdateDelegate,](updatedelegate-operation.md) когда указанный пользователь делегата не найден в списке делегатов.  <br/> |
|ErrorNotEnoughMemory  <br/> |Эта ошибка указывает на то, что операция не может быть выполнена из-за недостаточной памяти.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Эта ошибка указывает на то, что сообщение общего доступа не поддерживается.  <br/> |
|ErrorObjectTypeChanged  <br/> |Эта ошибка возникает, если тип объекта изменился.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Эта ошибка возникает, [](start.md) когда [](end-ex15websvcsotherref.md) обновляется время начала или окончания возникновения, так что это событие должно произойти раньше или позже соответствующего предыдущего или следующего возникновения.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Эта ошибка указывает на то, что время, предоставленное для данного события, совпадает с другим возникновением одного и того же повторяющегося элемента. Этот ответ также возникает, когда длина в минутах заданного события больше, чем Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Эта ошибка указывает на то, что текущая операция не является допустимой для корневой папки общего государственного.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Эта ошибка указывает на то, что организация запрашиваемой организации не является федераированной, поэтому запрашиватель не может создавать сообщения общего доступа для отправки внешнему пользователю или не может принимать сообщения, полученные от внешнего пользователя.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Этот код ответа не используется.  <br/> |
|ErrorParentFolderNotFound  <br/> |Эта ошибка возникает в операции [CreateFolder,](createfolder-operation.md) когда родительская папка не найдена.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Эта ошибка указывает на то, что перед доступом к этому почтовому ящику необходимо изменить пароль. Это происходит, когда была создана новая учетная запись, и администратор указал, что пользователь должен изменить пароль при первом логоном. Вы не можете обновить пароль с помощью Exchange веб-служб. Чтобы изменить пароль, необходимо использовать Microsoft Office Outlook веб-приложение.  <br/> |
|ErrorPasswordExpired  <br/> |Эта ошибка указывает на то, что срок действия пароля истек. Вы не можете изменить пароль с помощью Exchange веб-служб. Для изменения пароля необходимо использовать Outlook Web App средства.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Эта ошибка указывает на то, что запрашиватель пытался предоставить разрешения в календаре или папке контактов внешнему пользователю, но политика общего доступа, назначенная запрашиваемой запрашиваемой стороне, указывает на то, что запрашиваемая степень разрешения превышает допустимую политику общего доступа.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Эта ошибка указывает на то, что номер телефона не был в правильной форме.  <br/> |
|ErrorPropertyUpdate  <br/> |Эта ошибка указывает на сбой обновления из-за недействительных значений свойств. Сообщение ответа включает пути недействительных свойств.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Этот код ответа не используется.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Эта ошибка указывает на то, что запрос ссылается на подписку, которая существует на другом сервере клиентского доступа, но попытка прокси-сервера клиентского доступа не удалась.  <br/> |
|ErrorProxyCallFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Эта ошибка указывает на то, что запрос ссылается на почтовый ящик на другом сайте Active Directory, а первоначальный звонив является членом более 3000 групп.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Эта ошибка указывает на то, что запрос, Exchange веб-службы, отправленные на другой сервер клиентского доступа при выполнении [запроса GetUserAvailabilityRequest,](getuseravailabilityrequest.md) был недействительным. Этот код ответа обычно указывает, что произошла ошибка конфигурации или прав, или что кто-то безуспешно пытался имитировать запрос прокси-сервера доступности.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Эта ошибка указывает, Exchange веб-службы пытались прокси-запрос на доступность на другой сервер клиентского доступа для выполнения, но запрос не удалось. Этот ответ может быть вызван из-за проблем с подключением к сети или из-за проблем с периодичностью запроса.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Этот код ошибки должен быть возвращен, если веб-служба не может определить, следует ли выполнить запрос на целевом сервере или будет закавлиться на другой сервер.  <br/> |
|ErrorProxyTokenExpired  <br/> |Этот код ответа не используется.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Эта ошибка возникает, когда НЕВОЗМОЖНО найти URL-адрес почтового ящика общедоступных папок. Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Эта ошибка возникает при попытке доступа к общедоступным папкам, и попытка не выполнена. Эта ошибка была введена в Exchange 2013Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Эта ошибка возникает, когда получатель, переданный в операцию [GetUserAvailability,](getuseravailability-operation.md) находится на компьютере с версией Exchange Server, которая является более ранней Exchange 2007 г., и запрос на извлечение бесплатных и загруженных сведений для получателя с сервера общедоступных папок не удалось.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Эта ошибка возникает, когда получатель, переданный в операцию [GetUserAvailability,](getuseravailability-operation.md) находится на компьютере с версией Exchange Server, что является более ранним Exchange 2007 г., а запрос на извлечение бесплатных и загруженных сведений для получателя с сервера общедоступных папок не удалось, так как в организационном подразделении не было связанного сервера общедоступных папок.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Эта ошибка возникает, когда операция синхронизации успешно работает с основным почтовым ящиком общедоступных папок, но не удается в отношении вторичного почтового ящика общедоступных папок. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Эта ошибка указывает на то, что ограничение папки поиска может быть допустимым, но оно не поддерживается EWS. Exchange Веб-службы ограничивают ограничения, содержащие не более 255 выражений фильтра. При попытке привязки к существующей папке поиска, которая превышает 255, возвращается код ответа.  <br/> |
|ErrorQuotaExceeded  <br/> |Эта ошибка возникает при превышении квоты почтовых ящиков.  <br/> |
|ErrorReadEventsFailed  <br/> |Эта ошибка возвращается операцией [GetEvents](getevents-operation.md) или push-уведомлениями при сбое при идентвации сведений о событиях. Когда эта ошибка возвращается, подписка удаляется. Повторно создайте синхронизацию событий на основе последнего известного водяного знака.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Эта ошибка возвращается операцией [CreateItem,](createitem-operation.md) если была предпринята попытка подавить получение чтения, когда отправитель сообщения не запрашивал квитанцию на чтение в сообщении или если сообщение находится в папке нежелательной почты.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Эта ошибка возникает, когда дата окончания повторения после 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Эта ошибка возникает, когда указанное повторение не имеет экземпляров возникновения в указанном диапазоне.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Эта ошибка указывает на то, что список делегатов не удалось сохранить после удаления делегатов.  <br/> |
|ErrorRequestAborted  <br/> |Этот код ответа не используется.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Эта ошибка возникает, когда поток запросов превышает 400 КБ.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Эта ошибка возвращается, когда необходимое свойство отсутствует в запросе [операции CreateAttachment.](createattachment-operation.md) Недостающее свойство URI включено в ответ.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Эта ошибка указывает на то, что звонячий указал папку, которая не является папкой контактов для операции [ResolveNames.](resolvenames-operation.md)  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Эта ошибка указывает на то, что звонячий указал несколько папок контактов для операции [ResolveNames.](resolvenames-operation.md)  <br/> |
|ErrorResponseSchemaValidation  <br/> |Этот код ответа не используется.  <br/> |
|ErrorRestrictionTooLong  <br/> |Эта ошибка возникает, если ограничение содержит более 255 узлов.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Эта ошибка возникает, когда ограничение не может быть оценено Exchange веб-службами.  <br/> |
|ErrorResultSetTooBig  <br/> |Эта ошибка указывает на то, что количество записей календаря для данного получателя превышает допустимый предел в 1000. Уменьшите окно и попробуйте еще раз.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Эта ошибка возникает, когда [savedItemFolderId](saveditemfolderid.md) не найден.  <br/> |
|ErrorSchemaValidation  <br/> | Эта ошибка возникает, когда запрос не может быть проверен в схеме.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Эта ошибка указывает на то, что папка поиска была создана, но критерии поиска никогда не устанавливались в папке. Это происходит только при доступе к поврежденным папкам поиска, созданным с помощью другого API или клиента. Чтобы устранить эту ошибку, используйте операцию [UpdateFolder,](updatefolder-operation.md) чтобы установить элемент [SearchParameters,](searchparameters.md) чтобы включить ограничение, которое должно быть в папке.  <br/> |
|ErrorSendAsDenied  <br/> | Эта ошибка возникает при обоих следующих условиях: <br/> <br/>- Пользователю были предоставлены разрешения CanActAsOwner, но не предоставлены права делегата на почтовом ящике директора.  <br/>- Тот же пользователь пытается создать и отправить сообщение электронной почты в почтовом ящике директора с помощью параметра SendAndSaveCopy.<br/>  <br/>  В результате ошибка ErrorSendAsDenied и создание сообщения электронной почты в папке Черновики директора.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Эта ошибка возвращается операцией [DeleteItem,](deleteitem-operation.md) если атрибут **SendMeetingCancellations** отсутствует в запросе, а элемент для удаления — элемент календаря.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Эта ошибка возвращается операцией [UpdateItem,](updateitem-operation.md) если атрибут **SendMeetingInvitationsOrCancellations** отсутствует в запросе, а элемент обновления — элемент календаря.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Эта ошибка возвращается операцией [CreateItem,](createitem-operation.md) если атрибут **SendMeetingInvitations** отсутствует в запросе, а элемент для создания — элемент календаря.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Эта ошибка указывает на то, что после отправки организатором запроса собрания запрос не может быть обновлен. Чтобы изменить собрание, измените элемент календаря, а не запрос собрания.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Эта ошибка указывает на то, что после отправки запроса задачи инициатором задачи этот запрос не может быть обновлен.  <br/> |
|ErrorServerBusy  <br/> |Эта ошибка возникает, когда сервер занят.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Эта ошибка указывает, что Exchange веб-службы пытались прокси-сервер запроса доступности пользователя в соответствующий лес для получателя, но она не могла определить, куда отправить запрос из-за сбоя обнаружения службы.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Эта ошибка указывает на то, что внешнее свойство URL-адреса не было заданной в базе данных Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Эта ошибка указывает на сбой попытки синхронизации папки общего доступа. <br/><br/>Этот код ошибки возвращается, когда происходит следующее:<br/><br/>Подписка на папку общего доступа не найдена.<br/>— папка общего доступа не найдена.<br/>- Соответствующий пользователь каталога не найден.<br/>— Пользователь больше не существует.<br/>- Назначение является недействительным.<br/>— элемент контакта является недействительным.<br/>- Сбой связи с удаленным сервером.  <br/> |
|ErrorStaleObject  <br/> |Эта ошибка возникает в операции [UpdateItem](updateitem-operation.md) или в операции [SendItem,](senditem-operation.md) когда клавиша изменения не обновлена или не была поставлена. Вызов операции [GetItem,](getitem-operation.md) чтобы получить обновленный ключ изменения, а затем снова попробовать операцию.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Эта ошибка указывает на то, что пользователь не может немедленно отправлять больше запросов, так как квота отправки достигнута.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Эта ошибка возникает при попытке получить доступ к подписке с помощью учетной записи, которая не создает эту подписку. Доступ к каждой подписке может получить только создатель подписки.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Эта ошибка указывает, что вы не можете создать подписку, если вы не владелец или не имеете доступа владельца к почтовому ящику.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Эта ошибка возникает, если подписка, соответствующая указанной [SubscriptionId (GetEvents),](subscriptionid-getevents.md) не найдена. Возможно, срок действия подписки истек, процесс Exchange веб-служб может быть перезапущен или была передана недействительный подписка. Если подписка действительна, повторно создайте подписку с помощью последнего водяного знака. Это возвращается операцией [отписки](unsubscribe-operation.md) или ответами на операции [GetEvents.](getevents-operation.md)  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Этот код ошибки должен быть возвращен при запросе на подписку, которая была отписана.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Эта ошибка возвращается операцией [SyncFolderItems,](syncfolderitems-operation.md) если указанная родительская папка не может быть найдена.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Эта ошибка указывает на то, что почтовый ящик группы не найден. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Эта ошибка указывает на то, что почтовый ящик группы был найден, но он не связан с SharePoint Server. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Эта ошибка указывает на то, что почтовый ящик группы найден, но ссылка на сервер SharePoint не действительна. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Этот код ошибки не используется. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Этот код ошибки не используется. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Эта ошибка указывает на то, что попытка отправить уведомление владельцам почтовых ящиков группы не увенчалась успехом. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Эта ошибка указывает на общую ошибку, которая может возникнуть при попытке получить доступ к почтовому ящику группы. Попробуйте отправку запроса позже. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Эта ошибка указывает на то, что указанное время превышает допустимое ограничение. По умолчанию допустимый предел — 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Эта ошибка возникает, когда недостаточно времени для завершения обработки запроса.  <br/> |
|ErrorTimeZone  <br/> |Эта ошибка указывает на ошибку часовой пояс.  <br/> |
|ErrorToFolderNotFound  <br/> |Эта ошибка указывает на то, что папка назначения не существует.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Эта ошибка возникает, если звонячий пытается сделать запрос на сериализацию маркеров, но не имеет права ms-Exch-EPI-TokenSerialization на сервере клиентского доступа.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Эта ошибка возникает при превышении внутреннего ограничения на открытые объекты.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Эта ошибка указывает на то, что телефонная шкала пользователя недоступна.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Эта ошибка указывает на то, что пользователя не удалось найти.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Эта ошибка указывает, что для обработки запроса можно найти допустимый сервер для набора номера.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Эта ошибка возникает при неудачной попытке удалить контакт с мгновенными данными из группы. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorUnsupportedCulture  <br/> |Эта ошибка возникает, когда вы пытаетесь установить свойство **Culture** к значению, которое не может быть размыкаемо классом **System.Globalization.CultureInfo.**  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Эта ошибка возникает, когда звонячий пытается использовать расширенные свойства объектов типов, массива объектов, ошибок или null.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Эта ошибка возникает при попытке получить или установить контент MIME для элемента, помимо [объекта PostItem,](postitem.md) [Message](message-ex15websvcsotherref.md)или [CalendarItem.](calendaritem.md)  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Эта ошибка возникает, когда вызывающий передает свойство, которое является недействительным для запроса. Это может произойти при расчете свойств.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Эта ошибка возникает, когда вызываемая группа передает свойство, которое является недействительным для типа или группы по свойству. Это может произойти при расчете свойств.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Эта ошибка указывает на то, что ограничение папки поиска может быть допустимым, но оно не поддерживается EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Эта ошибка указывает на то, что указанное повторение не поддерживается для задач.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Этот код ответа не используется.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Эта ошибка указывает, Exchange веб-службы нашли тип свойства в магазине, но не могут создавать XML для типа свойства.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Эта ошибка указывает на то, что список делегатов не удалось сохранить после обновления делегатов.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Эта ошибка возникает, когда один путь свойства, указанный в описании изменений, не соответствует одному свойству, заданной в объекте [Item](item.md) или [Folder.](folder.md)  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Эта ошибка указывает на то, что запрашиватель не включен.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Эта ошибка указывает на то, что запрашиватель пытался предоставить разрешения в календаре или папке контактов внешнему пользователю, но политика общего доступа, назначенная запрашиваемой стороне, указывает на то, что домен внешнего пользователя не указан в политике.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Указывает, что в организации запрашиваемого запроса имеется набор федераированных доменов, но в организации запроса нет прокси-адресов SMTP с одним из федерадных доменов.  <br/> |
|ErrorValueOutOfRange  <br/> |Эта ошибка указывает, что дата начала или окончания представления календаря была назначена на 1/1/0001 12:00:00 или 12.31.9999 11:59:59.  <br/> |
|ErrorVirusDetected  <br/> |Эта ошибка указывает, что Exchange хранилище обнаружило вирус в сообщении.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Эта ошибка указывает, что Exchange обнаружил вирус в сообщении и удалил его.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWin32InteropError  <br/> |Эта ошибка указывает на то, что во время связи с неугодным кодом был допущен внутренний сбой.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Этот код ответа не используется.  <br/> |
|ErrorWrongServerVersion  <br/> |Эта ошибка указывает на то, что запрос может быть выполнен только на сервере, который является той же версией, что и сервер почтовых ящиков.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Эта ошибка указывает, что запрос был сделан делегатом, который имеет другую версию сервера, чем сервер почтовых ящиков директора.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Этот код ошибки никогда не возвращается.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Указывает, что имеются дублирующиеся заготавлители SOAP.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Указывает, что попытка синхронизации папки общего доступа не удалась.<br/><br/> Этот код ошибки должен быть возвращен, когда:<br/><br/>Подписка на папку общего доступа не найдена.  <br/>— папка общего доступа не найдена.  <br/>— Соответствующий пользователь каталога не найден.  <br/>— Пользователь больше не существует.  <br/>- Назначение является недействительным.  <br/>— элемент контакта является недействительным.  <br/>- Сбой связи с удаленным сервером.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Указывает, что внешнее свойство URL-адреса не задано в базе данных Active Directory. Этот код ошибки должен быть возвращен, если внешнее свойство URL-адреса не установлено в базе данных Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Указывает, что максимальное количество участников группы было достигнуто для получения сведений о свободной или загруженной занятости для списка рассылки. Эта ошибка должна быть возвращена, если максимальное количество участников группы достигнуто для получения сведений о свободной или загруженной занятости для списка рассылки.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Указывает, что элемент DataType и ShareFolderId присутствуют в запросе. Этот код ошибки должен быть возвращен, если элемент DataType и ShareFolderId присутствуют в запросе.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Указывает, что звонивка попыталась предоставить разрешения в календаре или папке контактов пользователю в другой организации, и попытка не удалась. Этот код ошибки должен быть возвращен, когда политика общего доступа отключена для вызываемого или когда политика общего доступа, назначенная для общего доступа к вызываемой папке, не передается для запрашиваемого уровня или типа запрашиваемой папки.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Указывает, что запросчик пытался предоставить разрешения в календаре или папке контактов внешнему пользователю, но политика общего доступа, назначенная запросчику, указывает, что домен внешнего пользователя не указан в политике.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Указывает, что запрашиватель пытался предоставить разрешения в своей папке календаря или контактов внешнему пользователю, но политика общего доступа, назначенная запрашиваемой запрашиваемой стороне, указывает, что уровень запрашиваемого разрешения выше, чем позволяет политика общего доступа.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Указывает, что организация запросителя не является федераторской, поэтому он не может создавать сообщения общего доступа для отправки внешнему пользователю или не может принимать сообщения, полученные от внешнего пользователя. Этот код ошибки должен быть возвращен, если организация запросителя не является федераторской.  <br/> |
|ErrorMailboxFailover  <br/> |Указывает, что попытка доступа к почтовому ящику не удалась, так как почтовый ящик находится в процессе сбоя.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Указывает, что отправитель приглашения общего доступа не создал метаданные приглашения общего доступа. Этот код ошибки должен быть возвращен, если отправитель приглашения общего доступа не создал метаданные приглашения общего доступа.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Указывает, что служба отслеживания сообщений не может отслеживать сообщение.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Указывает, что либо служба отслеживания сообщений не установлена, либо занята. Этот код ошибки указывает переходную ошибку. Клиенты могут повторно подключиться к серверу при получении этой ошибки.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Указывает, что данный домен не может быть найден.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Указывает, что у организации запросителя есть набор федераированных доменов, но у организации запросителя нет прокси-адресов SMTP с одним из федерадных доменов.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Указывает, что звонячий запрашивал бесплатные или занятые сведения для пользователя в другой организации, но в организационных отношениях не включено бесплатное/занятое.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Указывает, что объекты федерации организации запросителя не настроены должным образом.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Указывает, что сообщение общего доступа не предназначено для вызываемого.  <br/> |
|ErrorInvalidSharingData  <br/> |Указывает, что метаданные общего доступа не допустимы. Это может быть вызвано недействительным XML.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Указывает, что сообщение общего доступа не допустимо. Это может быть вызвано отсутствием свойства.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Указывает, что сообщение общего доступа не поддерживается.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Эта ошибка должна быть возвращена, если действие не может быть применено к одному или более элементов в беседе.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Эта ошибка должна быть возвращена, если любое правило не проверяется.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Эта ошибка должна быть возвращена, когда попытка управлять правилами "Входящие" возникает после того, как другой клиент получил доступ к правилам "Входящие".  <br/> |
|ErrorRulesOverQuota  <br/> |Эта ошибка должна быть возвращена при превышении квоты правил пользователя.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Эта ошибка должна быть возвращена первому подключению к подписке, если открыта вторая подписка.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Эта ошибка должна быть возвращена при пропущенных уведомлениях о событиях.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Эта ошибка возвращается, когда в службе доменных служб Active Directory (AD DS) имеются дублирующиеся устаревшие имена. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Эта ошибка указывает на то, что запрос на токен клиентского доступа был не действителен. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorNoSpeechDetected  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorUMServerUnavailable  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorRecipientNotFound  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorSpeechGrammarError  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Эта ошибка возвращается, если заглавная система [ManagementRole](managementrole.md) в загонах SOAP неверна. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Эта ошибка предназначена только для внутреннего использования. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Эта ошибка возвращается, когда выполняется масштабная попытка поиска без использования элемента [QueryString (String)](querystring-string.md) для поиска индексирования контента. Это применимо к операциям **SearchMailboxes** и **FindConversation.** Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Эта ошибка возвращается при неудачном поиске архивных почтовых ящиков. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Эта ошибка возвращается, когда URL-адрес архивного почтового ящика не обнаружен. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Эта ошибка возникает при сбое операции по удалённой папке почтовых ящиков архива.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Эта ошибка возникает при сбое операции по поиску папки удаленного почтового ящика архива.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Эта ошибка возникает, когда не удалось получить элемент удаленного почтового ящика архива.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Эта ошибка возникает при сбое операции по экспорту элементов удаленного архивного почтового ящика.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Эта ошибка возвращается, если с сервера запрашивается недействительный размер фотографии. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Эта ошибка возвращается, когда в запросе операции **GetUserPhoto** запрашивается неожиданный размер фотографии. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Эта ошибка возвращается, когда запрос на операцию **SearchMailboxes** содержит слишком много почтовых ящиков для поиска. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Эта ошибка указывает на отсутствие тегов хранения для этого пользователя. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Эта ошибка возвращается при отключении поиска обнаружения на клиенте или сервере. Эта ошибка была введена в Exchange 2013 г.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Эта ошибка возникает при попытке вызвать операцию [FindItem](finditem-operation.md) с [помощью SeekToConditionPageItemView](seektoconditionpageitemview.md) для получения элементов календаря, которые не поддерживаются.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Эта ошибка предназначена только для внутреннего использования.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |Клиент помечен для удаления.  <br/> |
|ErrorInvalidLicense  <br/> |У пользователя нет допустимой лицензии.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Квота получения сообщения на одну папку превышена.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент не требуется и не входит во все ответы. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

