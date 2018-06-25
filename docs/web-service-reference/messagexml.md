---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: Элемент MessageXml предоставляет дополнительные сведения об ошибке ответа.
ms.openlocfilehash: 8b6d201fe35c99a65f920ed7f60c33a2271fbd2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834470"
---
# <a name="messagexml"></a>MessageXml

Элемент **MessageXml** предоставляет дополнительные сведения об ошибке ответа. 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **xs: любой**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Содержит описательные сведения о состоянии ответа. <br/> <br/>  Ниже приведены некоторые возможные выражения XPath для этого элемента. <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса отказа от подписки.  <br/> |
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
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса подписаться.  <br/> |
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
|[FindConversationResponse](findconversationresponse.md) <br/> |Содержит состояние и результаты **FindConversation** ответа.  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса **EmptyFolder** .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Содержит состояние и результат запроса **UpdateInboxRules** .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Содержит состояние и результат запроса **UploadItemsResponse** .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Содержит ответ на запрос **GetInboxRules** .  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Содержит ответ на запрос **GetServiceConfiguration** .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент не является обязательным и не добавляется во все ответы. Она включена для сообщения об ошибках. В запросах, в которых используются папки или элементов, элемент **MessageXML** будет содержать один или несколько элементов, содержащих URI для свойства, вызвавшей ошибку. В качестве примера является элементом [FieldURI](fielduri.md) . 
  
Элемент **MessageXML** имеет тип **xs: любой**, который означает, что любые правильности XML-кода допустимое содержимое для этого элемента.
  
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

