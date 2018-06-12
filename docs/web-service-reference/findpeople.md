---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'Элемент FindPeople определяет набор данных, используемые в запросе FindPeople. Данные включают 0 или более из следующих элементов: фигуры пользователя (необязательно), индексируемых элементов страниц, ограничение (необязательно), объединение ограничение (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762589"
---
# <a name="findpeople"></a>FindPeople

Элемент **FindPeople** определяет набор данных, используемые в запросе FindPeople. Данные включают 0 или более из следующих элементов: фигуры пользователя (необязательно), индексируемых элементов страниц, ограничение (необязательно), объединение ограничение (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно). 
  
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

 **FindPeopleType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [ограничение](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [ Строка запроса (QueryStringType)](querystring-querystringtype.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

