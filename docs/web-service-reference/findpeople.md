---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'Элемент FindPeople указывает набор данных, используемых в запросе FindPeople. Данные включают ноль или более следующих элементов: фигуру пользователя (необязательно), представление элемента индексированной страницы, ограничение (необязательно), ограничение объединения (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).'
ms.openlocfilehash: 4777601b7146ec857b5c79fa9d4ced59a7247889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462903"
---
# <a name="findpeople"></a>FindPeople

Элемент **FindPeople** указывает набор данных, используемых в запросе FindPeople. Данные включают ноль или более следующих элементов: фигуру пользователя (необязательно), представление элемента индексированной страницы, ограничение (необязательно), ограничение объединения (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно). 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 **финдпеоплетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Персонашапе](personashape.md)  |  [Индекседпажеитемвиев](indexedpageitemview.md)  |  [Ограничение](restriction.md)  |  [Аггрегатионрестриктион](aggregationrestriction.md)  |  [SortOrder](sortorder.md)  |  [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md)  |  [Строка запроса (куеристрингтипе)](querystring-querystringtype.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

