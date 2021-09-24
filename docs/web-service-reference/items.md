---
title: Элементы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Элемент Items содержит массив элементов.
ms.openlocfilehash: b6e9db6524640098a902f431393fccd6bd4e8868
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540889"
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
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания в Exchange магазине.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции CopyItem.](copyitem-operation.md)  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateItem.](createitem-operation.md)  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [на операцию GetItem.](getitem-operation.md)  <br/> |
|[GroupedItems](groupeditems.md) <br/> |Представляет коллекцию элементов, которые являются результатом группового вызова [операции FindItem.](finditem-operation.md)  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [на операцию MoveItem.](moveitem-operation.md)  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Содержит результаты поиска одной корневой папки во время операции [FindItem.](finditem-operation.md)  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции UpdateItem.](updateitem-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Сведения о наборе элементов в запросе [операции CreateItem](createitem-operation.md) см. в статьи [Items (NonEmptyArrayOfAllItemsType).](items-nonemptyarrayofallitemstype.md)
  
[Элементы](message-ex15websvcsotherref.md) сообщений представляют сообщения электронной почты и все другие элементы, которые не сильно впечатлены схемой Exchange веб-служб (EWS). Такие элементы, как IPM. Общий доступ и IPM.InfoPath возвращаются в качестве **элементов сообщения.** Версии Exchange начиная с 2010 Exchange Server не возвращают базовый элемент [Item](item.md) в ответах. 
  
Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Exchange который установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

