---
title: Элементы (Нонемптяррайофаллитемстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: d61ef1cc-ddfc-480a-9625-7b436cb33ae0
description: Элемент Items содержит набор элементов, которые необходимо создать.
ms.openlocfilehash: 0f70f1fe4348b5b74cef6be6414618af1e3de260
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459856"
---
# <a name="items-nonemptyarrayofallitemstype"></a>Элементы (Нонемптяррайофаллитемстипе)

Элемент **Items** содержит набор элементов, которые необходимо создать. 
  
```XML
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</Items>
```

 **нонемптяррайофаллитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[реплитоитем](replytoitem.md) <br/> |Содержит ответ отправителю элемента в хранилище Exchange.  <br/> |
|[форвардитем](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[репляллтоитем](replyalltoitem.md) <br/> |Содержит ответ на отправителя и всех идентифицированных получателей элемента в хранилище Exchange.  <br/> |
|[акцептитем](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[тентативелякцептитем](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
|[деклинеитем](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[канцелкалендаритем](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Представляет объект Response, который используется для удаления элемента собрания при получении сообщения Митингканцеллатион.  <br/> |
|[постреплитем](postreplyitem.md) <br/> |Содержит ответ на элемент POST.  <br/> |
|[суппрессреадрецеипт](suppressreadreceipt.md) <br/> |Используется для отключения уведомлений о прочтении.  <br/> |
|[акцептшарингинвитатион](acceptsharinginvitation.md) <br/> |Используется для принятия приглашения, позволяющего получить доступ к данным календаря или контактов другого пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Определяет запрос на создание элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/CreateItem` <br/> |
|[конверсатионноде](conversationnode.md) <br/> |Определяет один узел в беседе.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateFolder](createfolder-operation.md)
  
[Операция CreateItem](createitem-operation.md)


[Создание папок (веб-службы Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

