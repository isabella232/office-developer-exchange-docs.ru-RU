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
description: Элемент FindItem определяет запрос на поиск элементов в почтовом ящике.
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460997"
---
# <a name="finditem"></a>FindItem

Элемент **FindItem** определяет запрос на поиск элементов в почтовом ящике. 
  
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

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


**финдитемтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Обход** <br/> |Определяет, ищет ли поиск элементы в папках или корзинах папок. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

|**Значение**|**Описание**|
|:-----|:-----|
|Поверхност  <br/> |Возвращает только удостоверения элементов в папке.  <br/> |
|SoftDeleted  <br/> |Возвращает только удостоверения элементов в корзине папки. Обратите внимание на то, что обратимо удаленный обход с ограничением поиска приведет к возвращению нулевых элементов, даже если имеются элементы, которые удовлетворяют условиям поиска.  <br/> |
|Соответствующую  <br/> |Возвращает только удостоверения связанных элементов в папке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемшапе](itemshape.md) <br/> |Определяет свойства и содержимое элемента, включаемые в ответ [операции FindItem](finditem-operation.md) .  <br/> |
|[индекседпажеитемвиев](indexedpageitemview.md) <br/> |Описывает, как возвращаются сведения о страничном элементе для запроса **FindItem** . Этот элемент является необязательным.  <br/> |
|[фрактионалпажеитемвиев](fractionalpageitemview.md) <br/> |Описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе **FindItem** . Смещение страничного представления от начала набора найденных элементов описывается с помощью дробной части. Этот элемент является необязательным.  <br/> |
|[CalendarView](calendarview.md) <br/> |Предоставляет ограниченные интервалы времени для определения поиска элементов календаря. Этот элемент является необязательным.  <br/> |
|[контактсвиев](contactsview.md) <br/> |Определяет Поиск элементов контактов на основе отображаемых имен в алфавитном порядке. Этот элемент является необязательным.  <br/> |
|[GroupBy](groupby.md) <br/> |Задает произвольное группирование для запросов **FindItem** . Этот элемент является необязательным.  <br/> |
|[дистингуишедграупби](distinguishedgroupby.md) <br/> |Предоставляет стандартные группирования для запросов **FindItem** . Этот элемент является необязательным.  <br/> |
|[Restriction](restriction.md) <br/> |Определяет ограничение или запрос, используемый для фильтрации элементов или папок в операциях **FindItem** /  **FindFolder** и папок поиска. Этот элемент является необязательным.  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет порядок сортировки элементов в запросе FindItem. Этот элемент является необязательным.  <br/> |
|[парентфолдеридс](parentfolderids.md) <br/> |Определяет папки для поиска операций FindItem и FindFolder.  <br/> |
|[Строка запроса (Куеристрингтипе)](querystring-querystringtype.md) <br/> |Содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

В запрос **FindItem** можно включить только один из элементов [индекседпажеитемвиев](indexedpageitemview.md), [фрактионалпажеитемвиев](fractionalpageitemview.md), [CalendarView](calendarview.md)или [контактсвиев](contactsview.md) . В запрос **FindItem** можно включить только один из элементов [GroupBy](groupby.md) или [дистингуишедграупби](distinguishedgroupby.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

