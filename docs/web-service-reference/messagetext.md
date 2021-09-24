---
title: MessageText
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageText
api_type:
- schema
ms.assetid: 59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1
description: Элемент MessageText предоставляет текстовое описание состояния ответа.
ms.openlocfilehash: 1503bbf211544797f56e7da661f38824a87a1196
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523855"
---
# <a name="messagetext"></a>MessageText

Элемент **MessageText** предоставляет текстовое описание состояния ответа. 
  
```XML
<MessageText/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Предоставляет описательные сведения о состоянии ответа.  <br/> <br/> Ниже приводится несколько возможных выражений XPath к этому элементу: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса deleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса отписки.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateFolder.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetFolder.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса UpdateFolder.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveFolder.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyFolder.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateManagedFolder.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateItem.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetItem.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса UpdateItem.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveItem.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyItem.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetAttachment.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса ResolveNames.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса ExpandDL.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса подписки.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderItems.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса ConvertId.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Содержит состояние и результат запроса AddDelegate.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Содержит состояние и результат запроса GetServerTimeZones.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса GetSharingFolder.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос GetSharingFolder.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Содержит состояние и результат запроса GetSharingMetadata.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Определяет ответ на запрос GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса RefreshSharingFolder.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Определяет ответ на запрос RefreshSharingFolder.  <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Представляет недействительный получатель для запроса GetSharingMetadata.  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Содержит состояние и результаты ответа **FindConversation.**  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного **запроса EmptyFolder.**  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Содержит ответ на **запрос UpdateInboxRules.**  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Содержит ответ на запрос **GetInboxRules.**  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Содержит ответ на запрос **GetServiceConfiguration.**  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент не требуется и не входит во все ответы. Этот элемент включается при возвращении сообщений об ошибках. 
  
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

