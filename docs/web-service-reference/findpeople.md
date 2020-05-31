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
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762589"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Персонашапе](personashape.md) | [индекседпажеитемвиев](indexedpageitemview.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md)[Restriction](restriction.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)[QueryString (QueryStringType)](querystring-querystringtype.md) ограничение аггрегатионрестриктион | SortOrder ParentFolderId (таржетфолдеридтипе) QueryString (куеристрингтипе) | 
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

