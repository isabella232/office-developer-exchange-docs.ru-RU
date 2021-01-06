---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: Элемент ResponseMessages содержит сообщения ответа для запроса веб-служб Exchange.
ms.openlocfilehash: 93d83fbba3ea4bfe33f574eea7991157a4f10b88
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465403"
---
# <a name="responsemessages"></a>ResponseMessages

Элемент **ResponseMessages** содержит сообщения ответа для запроса веб-служб Exchange. 
  
```XML
<ResponseMessages>
   <CreateItemResponseMessage/>
</ResponseMessages>
```

```xml
<ResponseMessages>
   <DeleteItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <EmptyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UploadItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExportItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ResolveNamesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExpandDLResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetServerTimeZonesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetStreamingEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UnsubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendNotificationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderHierarchyResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateManagedFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ConvertIdResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingMetadataResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <RefreshSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomListsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRemindersResponse/>
</ResponseMessages
```

```xml 
<ResponseMessages>
   <PerformReminderActionResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ApplyConversationActionResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetPasswordExpirationDateResponse />
</ResponseMessages>
```


**ArrayOfResponseMessagesType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyFolder.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyItem.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateAttachment.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateItem.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteAttachment.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteFolder.  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteItem.  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [EmptyFolder.](emptyfolder.md)  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса ExpandDL.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindFolder.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindItem.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetAttachment.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Содержит состояние и результаты одного запроса UploadItems.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Содержит состояние и результаты одного запроса ExportItems.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetEvents.  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetStreamingEvents.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetFolder.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetItem.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveFolder.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса ResolveNames.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendItem.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendNotification.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса на подписку.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderItems.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса на отписки.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса UpdateFolder.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса UpdateItem.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса ConvertId.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Содержит состояние и результаты запроса GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Содержит состояние и результаты запроса RefreshSharingFolder.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результаты запроса GetSharingFolder.  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |Содержит состояние и результаты запроса CreateUserConfiguration.  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |Содержит состояние и результаты запроса DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Содержит состояние и результаты запроса GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |Содержит состояние и результаты запроса UpdateUserConfiguration.  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Содержит состояние и результаты запроса GetRoomLists.  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |Содержит состояние и результаты запроса GetRooms.  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |Содержит состояние и результаты запроса GetReminders.  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |Содержит состояние и результаты запроса PerformReminderAction.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetServerTimeZones.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Содержит состояние и результаты запроса на операцию [ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyFolderResponse](copyfolderresponse.md) <br/> |Определяет ответ на запрос CopyFolder.  <br/> |
|[CopyItemResponse](copyitemresponse.md) <br/> |Определяет ответ на запрос CopyItem.  <br/> |
|[CreateAttachmentResponse](createattachmentresponse.md) <br/> |Определяет ответ на запрос CreateAttachment.  <br/> |
|[CreateFolderResponse](createfolderresponse.md) <br/> |Определяет ответ на запрос CreateFolder.  <br/> |
|[CreateItemResponse](createitemresponse.md) <br/> |Определяет ответ на запрос CreateItem.  <br/> |
|[CreateManagedFolderResponse](createmanagedfolderresponse.md) <br/> |Определяет ответ на запрос CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponse](deleteattachmentresponse.md) <br/> |Определяет ответ на запрос DeleteAttachment.  <br/> |
|[DeleteFolderResponse](deletefolderresponse.md) <br/> |Определяет ответ на запрос DeleteFolder.  <br/> |
|[DeleteItemResponse](deleteitemresponse.md) <br/> |Определяет ответ на запрос DeleteItem.  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |Определяет ответ на запрос EmptyFolder.  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |Определяет ответ на запрос ExpandDL.  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |Представляет ответ на один запрос ExportItems.  <br/> |
|[FindFolderResponse](findfolderresponse.md) <br/> |Определяет ответ на запрос FindFolder.  <br/> |
|[FindItemResponse](finditemresponse.md) <br/> |Определяет ответ на запрос FindItem.  <br/> |
|[GetAttachmentResponse](getattachmentresponse.md) <br/> |Определяет ответ на запрос GetAttachment.  <br/> |
|[GetEventsResponse](geteventsresponse.md) <br/> |Определяет ответ на запрос GetEvents.  <br/> |
|[GetStreamingEventsResponse](getstreamingeventsresponse.md) <br/> |Определяет ответ на запрос GetStreamingEvents.  <br/> |
|[GetFolderResponse](getfolderresponse.md) <br/> |Определяет ответ на запрос GetFolder.  <br/> |
|[GetItemResponse](getitemresponse.md) <br/> |Определяет ответ на запрос GetItem.  <br/> |
|[MoveFolderResponse](movefolderresponse.md) <br/> |Определяет ответ на запрос MoveFolder.  <br/> |
|[MoveItemResponse](moveitemresponse.md) <br/> |Определяет ответ на запрос MoveItem.  <br/> |
|[ResolveNamesResponse](resolvenamesresponse.md) <br/> |Определяет ответ на запрос ResolveNames.  <br/> |
|[SendItemResponse](senditemresponse.md) <br/> |Определяет ответ на запрос SendItem.  <br/> |
|[SendNotificationResult](sendnotificationresult.md) <br/> |Определяет ответ на запрос SendNotification.  <br/> |
|[SubscribeResponse](subscriberesponse.md) <br/> |Определяет ответ на запрос на подписку.  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |Определяет ответ на запрос SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |Определяет ответ на запрос SyncFolderItems.  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |Определяет ответ на запрос отписаться.  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |Определяет ответ на запрос UpdateFolder.  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |Определяет ответ на запрос UpdateItem.  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |Содержит ответ на запрос ConvertId.  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |Определяет ответ на запрос GetServerTimeZones.  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |Определяет ответ на запрос CreateUserConfiuration.  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |Определяет ответ на запрос DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |Определяет ответ на запрос GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |Определяет ответ на запрос UpdateUserConfiguration.  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |Определяет ответ на запрос [операции ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |Определяет ответ на запрос [операции GetPasswordExpirationDate.](getpasswordexpirationdate-operation.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExportItems](exportitems-operation.md) 
- [Операция UploadItems](uploaditems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

