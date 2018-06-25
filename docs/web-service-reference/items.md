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
description: Элемент элементов содержит массив элементов.
ms.openlocfilehash: 241a56ee23e87d6a4320b93cc65b1f5aa1f60120
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834163"
---
# <a name="items"></a>Элементы

Элемент **элементов** содержит массив элементов. 
  
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

 **ArrayOfRealItemsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент post в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат [операции CopyItem](copyitem-operation.md) запроса.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат один запрос [CreateItem операции](createitem-operation.md) .  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат [операции GetItem](getitem-operation.md) запроса.  <br/> |
|[GroupedItems](groupeditems.md) <br/> |Представляет коллекцию элементов, которые являются результатом сгруппированных [операции FindItem](finditem-operation.md) вызова.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат [операции MoveItem](moveitem-operation.md) запроса.  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат [операции UpdateItem](updateitem-operation.md) запроса.  <br/> |
   
## <a name="remarks"></a>Замечания

Сведения о наборе элементов в запрос [CreateItem операции](createitem-operation.md) отображаются [элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).
  
Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange (EWS). Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы **сообщения** . Версии Exchange, начиная с Exchange Server 2010 не возвращает [базовый элемент](item.md) в ответы. 
  
Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

