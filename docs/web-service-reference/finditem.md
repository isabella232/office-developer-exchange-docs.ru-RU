---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: Элемент FindItem определяет запрос для поиска элементов в почтовом ящике.
ms.openlocfilehash: 9831b034be7deb0cf6e756bb585bdbe34b370afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762577"
---
# <a name="finditem"></a>FindItem

Элемент **FindItem** определяет запрос для поиска элементов в почтовом ящике. 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

 **FindItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Обход** <br/> |Определяет, будет ли поиск элементов в папках или папки корзины. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

|**Значение**|**Описание**|
|:-----|:-----|
|Неполная  <br/> |Возвращает только идентификаторы элементов в папке.  <br/> |
|SoftDeleted  <br/> |Возвращает только идентификаторы элементов, находящихся в папке корзины. Обратите внимание, что удаленные обхода, в сочетании с ограничения поиска приведет к нулю, найденном даже в том случае, если существуют элементы, соответствующие условиям поиска.  <br/> |
|Связанные  <br/> |Возвращает только идентификаторы связанных элементов в папке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Определяет свойства элемента и содержимого для включения в [операции FindItem](finditem-operation.md) ответа.  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Описывает, как выгружаемый элемента сведения возвращаются для запроса **FindItem** . Этот элемент является необязательным.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Описывает, где начала страничного представления и максимальное число элементов, возвращаемых в запросе **FindItem** . Смещение страничного представления от начала набора найденных элементов описывается функцией. Этот элемент является необязательным.  <br/> |
|[Представления календаря](calendarview.md) <br/> |Содержит время охватывать ограничения для определения критериев поиска для элементов календаря. Этот элемент является необязательным.  <br/> |
|[ContactsView](contactsview.md) <br/> |Определяет поиска на основе алфавитном отображения имен контактов. Этот элемент является необязательным.  <br/> |
|[GroupBy](groupby.md) <br/> |Указывает произвольное группирование для запросов **FindItem** . Этот элемент является необязательным.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Содержит стандартные группы для запросов **FindItem** . Этот элемент является необязательным.  <br/> |
|[Ограничения](restriction.md) <br/> |Задает ограничение или запрос, используемый для фильтрации элементов или папок в **FindItem**/ **FindFolder** и папки операций поиска. Этот элемент является необязательным.  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет способ сортировки в запросе FindItem элементов. Этот элемент является необязательным.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Идентифицирует папок для поиска для операций FindItem и FindFolder.  <br/> |
|[Строка запроса (QueryStringType)](querystring-querystringtype.md) <br/> |Содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Только один из [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [представления календаря](calendarview.md)или элементы [ContactsView](contactsview.md) может быть включен в запросе **FindItem** . Только один из элементов [GroupBy](groupby.md) или [DistinguishedGroupBy](distinguishedgroupby.md) может быть включен в запросе **FindItem** . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindItem Operation](finditem-operation.md)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

