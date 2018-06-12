---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: Элемент CancelCalendarItem представляет объект ответа, которая используется для отмены собрания.
ms.openlocfilehash: 262f60db33abac36156b069dc85e1fccb3522d5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761664"
---
# <a name="cancelcalendaritem"></a>CancelCalendarItem

Элемент **CancelCalendarItem** представляет объект ответа, которая используется для отмены собрания. 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 **CancelCalendarItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Subject](subject.md) <br/> |Представляет свойство subject элементов хранилища Exchange.  <br/> |
|[Body](body.md) <br/> |Не используется с **CancelCalendarItem**. Свойство [NewBodyContent](newbodycontent.md) используется для установки содержимое текста запроса.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит набор получателей элемента. Далее представлены основные получателей элемента.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копии сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Указывает, будет ли отправителя элемента о прочтении.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Указывает, требует ли отправитель элемента уведомление о доставке.  <br/> |
|[ReferenceItemId](referenceitemid.md) <br/> |Определяет элемент, к которому относится объект ответа.  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |Представляет новое содержимое текста сообщения.  <br/> |
|[Получил](receivedby.md) <br/> |Определяет делегат в сценарии доступа делегата. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Идентифицирует участника в сценарии доступа делегата. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> | Описание всех элементов, расположенных во время собрания.<br/><br/> Ниже приведены некоторые из выражения XPath для этого элемента.<br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> | Описание всех элементов, конфликтующие с время собрания.<br/><br/>Ниже приведены некоторые из выражения XPath для этого элемента.<br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.  <br/> |
|[Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папку, указанную в элементе [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **CancelCalendarItem** только просматривать организатором. Применяется только для организатора элемента календаря. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

