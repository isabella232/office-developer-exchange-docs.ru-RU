---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: Элемент GroupBy задает произвольную группировки для запросов FindItem.
ms.openlocfilehash: cdf9b9906025bc91768bb4a14acb2573801c4e12
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353219"
---
# <a name="groupby"></a>GroupBy

Элемент **GroupBy** задает произвольную группировки для запросов FindItem. 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

**GroupByType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Порядок** <br/> | Определяет порядок групп в массиве сгруппированных элементов, возвращаемого в ответе. Этот атрибут имеет тип SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Значения атрибутов заказа

|**Значение**|**Описание**|
|:-----|:-----|
|По возрастанию  <br/> |Группы упорядочены в порядке возрастания.  <br/> |
|Descending  <br/> |Группы упорядочены по убыванию.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает расширенные свойства MAPI для получения, установки или создать.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Представляет поле, которое используется для определения порядка групп в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.  <br/><br/> Ниже приведен выражение XPath для этого элемента.`/FindItem` <br/> |
   
## <a name="remarks"></a>Замечания

Ответ FindItem будет содержать коллекцию групп. Каждой группе будет содержать все элементы, которым пришлось совпадающие значения для свойства **GroupBy** . Свойство, которое определяет группирование идентифицируется в элементе [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI](extendedfielduri.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

