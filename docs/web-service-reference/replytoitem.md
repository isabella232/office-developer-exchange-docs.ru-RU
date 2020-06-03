---
title: реплитоитем
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyToItem
api_type:
- schema
ms.assetid: 35ee751a-41c0-4216-ad8b-78f7ada43a2f
description: Элемент Реплитоитем содержит ответ отправителю элемента в хранилище Exchange.
ms.openlocfilehash: fc40335dc73327820c0b39cafa07168d1f27851d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529856"
---
# <a name="replytoitem"></a>реплитоитем

Элемент **реплитоитем** содержит ответ отправителю элемента в хранилище Exchange. 
  
```xml
<ReplyToItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <From/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</ReplyToItem>
```

**реплитоитемтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тема](subject.md) <br/> |Представляет свойство Subject элементов хранилища Exchange.  <br/> |
|[Body](body.md) <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит массив получателей элемента. Далее представлены основные получателей элемента.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения скрытой копии (BCC) сообщения электронной почты.  <br/> |
|[исреадрецеиптрекуестед](isreadreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента уведомление о прочтении.  <br/> |
|[исделиверирецеиптрекуестед](isdeliveryreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента уведомление о доставке.  <br/> |
|[From](from.md) <br/> |Представляет адрес, с которого было отправлено сообщение.  <br/> |
|[референцеитемид](referenceitemid.md) <br/> |Определяет элемент, на который ссылается объект Response.  <br/> |
|[невбодиконтент](newbodycontent.md) <br/> |Представляет новое содержимое основного текста сообщения.  <br/> |
|[рецеиведби](receivedby.md) <br/> |Определяет делегат в сценарии доступа делегата. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[рецеиведрепресентинг](receivedrepresenting.md) <br/> |Определяет участника в сценарии доступа делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аджацентмитингс](adjacentmeetings.md) <br/> | Описывает все элементы, смежные с временем собрания. <br/> <br/>  Ниже приведены некоторые выражения XPath для этого элемента. <br/> <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> | Описывает все элементы, которые конфликтуют с временем собрания. <br/> <br/>  Ниже приведены некоторые выражения XPath для этого элемента. <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[респонсеобжектс](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.  <br/> |
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент [from](from.md) должен быть установлен на адрес электронной почты субъекта, если элемент является ответом делегата. Если делегат не задает свойство [from](from.md) , элемент будет отправлен непосредственно из почтового ящика представителя. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

