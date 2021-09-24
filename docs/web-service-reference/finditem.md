---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: Элемент FindItem определяет запрос на поиск элементов в почтовом ящике.
ms.openlocfilehash: 7005b4a837c61ffa00a49b687e729de7ed769bcf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541317"
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


**FindItemType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Traversal** <br/> |Определяет, находятся ли в поиске элементы в папках или в контейнерах папок. Этот атрибут является обязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибута Traversal

|**Значение**|**Описание**|
|:-----|:-----|
|Shallow  <br/> |Возвращает только удостоверения элементов в папке.  <br/> |
|SoftDeleted  <br/> |Возвращает только удостоверения элементов, которые находятся в контейнере папки. Обратите внимание, что переход с мягким удалением в сочетании с ограничением поиска приведет к возвращению нулевых элементов, даже если существуют элементы, которые соответствуют критериям поиска.  <br/> |
|Связанные  <br/> |Возвращает только удостоверения связанных элементов в папке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Определяет свойства и содержимое элемента, которые необходимо включить в ответ на операцию [FindItem.](finditem-operation.md)  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Описывает, как возвращается информация о странице для запроса **FindItem.** Этот элемент является необязательным.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Описывает, где начинается просмотр страницы и максимальное количество элементов, возвращаемых в **запросе FindItem.** Представление страницы, смещенное с начала набора найденных элементов, описывается фракцией. Этот элемент является необязательным.  <br/> |
|[CalendarView](calendarview.md) <br/> |Предоставляет ограничения по времени для определения поиска элементов календаря. Этот элемент является необязательным.  <br/> |
|[ContactsView](contactsview.md) <br/> |Определяет поиск контактных элементов на основе алфавитных имен отображения. Этот элемент является необязательным.  <br/> |
|[GroupBy](groupby.md) <br/> |Указывает произвольные группировки для **запросов FindItem.** Этот элемент является необязательным.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Предоставляет стандартные группировки для **запросов FindItem.** Этот элемент является необязательным.  <br/> |
|[Restriction](restriction.md) <br/> |Определяет ограничение или запрос, используемый для фильтрации элементов или папок в **операциях FindItem** /  **FindFolder** и папки поиска. Этот элемент является необязательным.  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет сортировку элементов в запросе FindItem. Этот элемент является необязательным.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Определяет папки для поиска операций FindItem и FindFolder.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Содержит строку запроса почтовых ящиков на основе синтаксиса расширенных запросов (AQS).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Только один из элементов [IndexedPageItemView,](indexedpageitemview.md) [FractionalPageItemView,](fractionalpageitemview.md) [CalendarView](calendarview.md)или [ContactsView](contactsview.md) может быть включен в **запрос FindItem.** Только один из [элементов GroupBy](groupby.md) или [DistinguishedGroupBy](distinguishedgroupby.md) может быть включен в запрос **FindItem.** 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

