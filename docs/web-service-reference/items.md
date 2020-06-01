---
title: Элементы
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
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Элемент Items содержит массив элементов.
ms.openlocfilehash: 489e34ad0e4bcc2520febb3c213db970fa496051
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458133"
---
# <a name="items"></a>Элементы

Элемент **Items** содержит массив элементов. 
  
```xml
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
   <PostItem/>
</Items>
```

 **аррайофреалитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент POST в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[копитемреспонсемессаже](copyitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции CopyItem](copyitem-operation.md) .  <br/> |
|[креатеитемреспонсемессаже](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateItem](createitem-operation.md) .  <br/> |
|[жетитемреспонсемессаже](getitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции GetItem](getitem-operation.md) .  <br/> |
|[граупедитемс](groupeditems.md) <br/> |Представляет коллекцию элементов, которая является результатом сгруппированного вызова [операции FindItem](finditem-operation.md) .  <br/> |
|[мовеитемреспонсемессаже](moveitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции MoveItem](moveitem-operation.md) .  <br/> |
|[Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md) <br/> |Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).  <br/> |
|[упдатеитемреспонсемессаже](updateitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции UpdateItem](updateitem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Сведения о наборе элементов в запросе на [операцию CreateItem](createitem-operation.md) см. в статье [Items (нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md).
  
Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS). Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов **Message** . Версии Exchange, начиная с Exchange Server 2010, не возвращают элемент базового [элемента](item.md) в ответах. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором запущен Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

