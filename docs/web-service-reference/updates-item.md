---
title: Обновления (элемент)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: Элемент Updates содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента.
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840378"
---
# <a name="updates-item"></a>Обновления (элемент)

Элемент **Updates** содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента. 
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Обновления (элемент)](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

**NonEmptyArrayOfItemChangeDescriptionsType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToItemField](appendtoitemfield.md) <br/> |Представляет данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Представляет операцию для удаления заданного свойства из элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления для применения к элементу.  <br/> Ниже приведен выражение XPath для этого элемента.`/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>Замечания

Обновления, определенные в этот элемент выполняются для элемента, который идентифицируется средством [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)или [RecurringMasterItemId](recurringmasteritemid.md) элементы. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |типы схемы  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [UpdateItem Operation](updateitem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

