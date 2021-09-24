---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: Элемент GroupBy указывает произвольную группировку для запросов FindItem.
ms.openlocfilehash: 15e2d818ceae81f08ad0c52d9bdc881f7c3e2579
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539804"
---
# <a name="groupby"></a>GroupBy

Элемент **GroupBy** указывает произвольную группировку для запросов FindItem. 
  
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
|**Order** <br/> | Определяет порядок групп в массиве сгрупповых элементов, возвращаемом в ответе. Этот атрибут имеет тип SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Значения атрибута заказа

|**Значение**|**Описание**|
|:-----|:-----|
|По возрастанию  <br/> |Группы заказываться в порядке восходящей.  <br/> |
|Убывка  <br/> |Группы упорядочены в порядке убывания.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Определяет часто ссылаясь свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Определяет отдельных членов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI для получения, набора или создания.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Представляет поле, которое используется для определения порядка групп в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/><br/> Ниже приводится выражение XPath к этому элементу:  `/FindItem` <br/> |
   
## <a name="remarks"></a>Заметки

Ответ FindItem будет содержать коллекцию групп. Каждая группа будет содержать все элементы, которые имели совпадающие значения для свойства **GroupBy.** Свойство, определяющий группировку, определяется в [элементе FieldURI,](fielduri.md) [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI.](extendedfielduri.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

