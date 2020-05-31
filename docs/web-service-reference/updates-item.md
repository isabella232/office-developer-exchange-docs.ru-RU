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
description: Элемент Updates содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента.
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840378"
---
# <a name="updates-item"></a>Обновления (элемент)

Элемент **Updates** содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств элемента. 
  
- [UpdateItem](updateitem.md)
  
- [итемчанжес](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Обновления (элемент)](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

**нонемптяррайофитемчанжедескриптионстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аппендтоитемфиелд](appendtoitemfield.md) <br/> |Представляет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[сетитемфиелд](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).  <br/> |
|[делетеитемфиелд](deleteitemfield.md) <br/> |Представляет операцию удаления данного свойства из элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления, применяемые к элементу.  <br/> Ниже приведено выражение XPath для этого элемента:`/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>Примечания

Обновления, определенные этим элементом, выполняются над элементом, идентифицируемым элементами [ItemId](itemid.md), [оккурренцеитемид](occurrenceitemid.md)или [рекуррингмастеритемид](recurringmasteritemid.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateItem](updateitem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

