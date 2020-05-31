---
title: ассоЦиатедкалендаритемид
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
description: Элемент АссоЦиатедкалендаритемид представляет элемент календаря, связанный с Митингмессаже, свойство meetingrequest, Митингреспонсе, Митингканцеллатион или Реминдермессажедата.
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761506"
---
# <a name="associatedcalendaritemid"></a>ассоЦиатедкалендаритемид

Элемент **ассоЦиатедкалендаритемид** представляет элемент календаря, связанный с [митингмессаже](meetingmessage.md), [свойство meetingrequest](meetingrequest.md), [митингреспонсе](meetingresponse.md), [митингканцеллатион](meetingcancellation.md)или [реминдермессажедата](remindermessagedata.md).
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **итемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет элемент календаря, связанный с собранием.  <br/> |
|**чанжекэй** <br/> |Определяет конкретную версию элемента календаря, связанную с собранием.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Митингмессаже](meetingmessage.md) | [свойство meetingrequest](meetingrequest.md) | [ReminderMessageData](remindermessagedata.md) [MeetingCancellation](meetingcancellation.md)[MeetingResponse](meetingresponse.md)митингреспонсе митингканцеллатион реминдермессажедата |  | 
  
## <a name="remarks"></a>Примечания

Версии Exchange, начинающиеся с номера сборки 15.00.0913.09, могут включать элемент **ассоЦиатедкалендаритемид** в качестве дочернего элемента элемента **реминдермессажедата** . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

