---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: Элемент AssociatedCalendarItemId представляет элемент календаря, связанный с meetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation или ReminderMessageData.
ms.openlocfilehash: 5a51c5e3e43a25ebe676bc85e80c2a6ab3705c4d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543690"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

Элемент **AssociatedCalendarItemId** представляет элемент календаря, связанный с [meetingMessage,](meetingmessage.md) [MeetingRequest,](meetingrequest.md) [MeetingResponse,](meetingresponse.md) [MeetingCancellation](meetingcancellation.md)или [ReminderMessageData.](remindermessagedata.md)
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет элемент календаря, связанный с собранием.  <br/> |
|**ChangeKey** <br/> |Определяет определенную версию элемента календаря, связанного с собранием.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>Заметки

Версии Exchange со сборкой 15.00.0913.09 могут включать элемент **AssociatedCalendarItemId** в качестве детского элемента элемента **ReminderMessageData.** 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

