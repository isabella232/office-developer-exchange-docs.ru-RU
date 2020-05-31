---
title: мессажетекст
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageText
api_type:
- schema
ms.assetid: 59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1
description: Элемент Мессажетекст предоставляет текстовое описание состояния отклика.
ms.openlocfilehash: e90313c1b8616658932de4b394d4a2b3ed0fd054
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834462"
---
# <a name="messagetext"></a>мессажетекст

Элемент **мессажетекст** предоставляет текстовое описание состояния отклика. 
  
```XML
<MessageText/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессаже](responsemessage.md) <br/> | Предоставляет описательные сведения о состоянии отклика.  <br/> <br/> Ниже приведены некоторые из возможных выражений XPath для этого элемента: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[делетеитемреспонсемессаже](deleteitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteItem.  <br/> |
|[сендитемреспонсемессаже](senditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendItem.  <br/> |
|[делетефолдерреспонсемессаже](deletefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteFolder.  <br/> |
|[делетеаттачментреспонсемессаже](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса DeleteAttachment.  <br/> |
|[унсубскрибереспонсемессаже](unsubscriberesponsemessage.md) <br/> |Содержит состояние и результат одного запроса отказа от подписки.  <br/> |
|[креатефолдерреспонсемессаже](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateFolder.  <br/> |
|[жетфолдерреспонсемессаже](getfolderresponsemessage.md) <br/> |Содержит сведения о состоянии и результатах одного запроса на получение вложенной папки.  <br/> |
|[упдатефолдерреспонсемессаже](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса операцию UpdateFolder.  <br/> |
|[мовефолдерреспонсемессаже](movefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveFolder.  <br/> |
|[копифолдерреспонсемессаже](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyFolder.  <br/> |
|[креатеманажедфолдерреспонсемессаже](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateManagedFolder.  <br/> |
|[финдфолдерреспонсемессаже](findfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindFolder.  <br/> |
|[креатеитемреспонсемессаже](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateItem.  <br/> |
|[жетитемреспонсемессаже](getitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetItem.  <br/> |
|[упдатеитемреспонсемессаже](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса UpdateItem.  <br/> |
|[мовеитемреспонсемессаже](moveitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса MoveItem.  <br/> |
|[копитемреспонсемессаже](copyitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CopyItem.  <br/> |
|[креатеаттачментреспонсемессаже](createattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса CreateAttachment.  <br/> |
|[жетаттачментреспонсемессаже](getattachmentresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetAttachment.  <br/> |
|[финдитемреспонсемессаже](finditemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса FindItem.  <br/> |
|[ресолвенамесреспонсемессаже](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса ResolveNames.  <br/> |
|[експанддлреспонсемессаже](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса ExpandDL.  <br/> |
|[субскрибереспонсемессаже](subscriberesponsemessage.md) <br/> |Содержит состояние и результат запроса одиночной подписки.  <br/> |
|[жетевентсреспонсемессаже](geteventsresponsemessage.md) <br/> |Содержит состояние и результат запроса на единичные события.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса Сенднотификатион.  <br/> |
|[синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderHierarchy.  <br/> |
|[синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderItems.  <br/> |
|[конвертидреспонсемессаже](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса ConvertId.  <br/> |
|[аддделегатереспонсе](adddelegateresponse.md) <br/> |Содержит состояние и результат запроса AddDelegate.  <br/> |
|[жетсервертимезонесреспонсемессаже](getservertimezonesresponsemessage.md) <br/> |Содержит состояние и результат запроса GetServerTimeZones.  <br/> |
|[жетшарингфолдерреспонсемессаже](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса GetSharingFolder.  <br/> |
|[жетшарингфолдерреспонсе](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос GetSharingFolder.  <br/> |
|[жетшарингметадатареспонсемессаже](getsharingmetadataresponsemessage.md) <br/> |Содержит состояние и результат запроса GetSharingMetadata.  <br/> |
|[жетшарингметадатареспонсе](getsharingmetadataresponse.md) <br/> |Определяет ответ на запрос GetSharingMetadata.  <br/> |
|[рефрешшарингфолдерреспонсемессаже](refreshsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса RefreshSharingFolder.  <br/> |
|[рефрешшарингфолдерреспонсе](refreshsharingfolderresponse.md) <br/> |Определяет ответ на запрос RefreshSharingFolder.  <br/> |
|[инвалидреЦипиент](invalidrecipient.md) <br/> |Представляет недопустимого получателя для запроса GetSharingMetadata.  <br/> |
|[финдконверсатионреспонсе](findconversationresponse.md) <br/> |Содержит сведения о состоянии и результатах ответа **FindConversation** .  <br/> |
|[емптифолдерреспонсемессаже](emptyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса **EmptyFolder** .  <br/> |
|[упдатеинбоксрулесреспонсе](updateinboxrulesresponse.md) <br/> |Содержит ответ на запрос **UpdateInboxRules** .  <br/> |
|[жетинбоксрулесреспонсе](getinboxrulesresponse.md) <br/> |Содержит ответ на запрос **GetInboxRules** .  <br/> |
|[жетсервицеконфигуратионреспонсе](getserviceconfigurationresponse.md) <br/> |Содержит ответ на запрос **GetServiceConfiguration** .  <br/> |
|[сервицеконфигуратионреспонсемессажетипе](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент не является обязательным и не включается во все ответы. Этот элемент включается при возвращении сообщений об ошибках. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

