---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: Элемент AssociatedCalendarItemId представляет элемента календаря, который связан с MeetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation или ReminderMessageData.
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761506"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

Элемент **AssociatedCalendarItemId** представляет элемента календаря, который связан с [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)или [ReminderMessageData](remindermessagedata.md).
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Определяет элемент календаря, который связан с собрания.  <br/> |
|**ChangeKey** <br/> |Идентифицирует определенной версии элемента календаря, который связан с собрания.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>Замечания

Версии Exchange, начиная с номер сборки 15.00.0913.09 может включать элемент **AssociatedCalendarItemId** как дочерний элемент элемента **ReminderMessageData** . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

