---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: Элемент AggregationRestriction указывает значение, которое применяется к набор свойств пользователя, связанные с FindPeople запроса и фильтрует result согласно указанным ограничениям.
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761367"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

Элемент **AggregationRestriction** указывает значение, которое применяется к набор свойств пользователя, связанные с FindPeople запроса и фильтрует result согласно указанным ограничениям. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Замечания

Элемент **AggregationRestriction** может содержать любые дочерний элемент, который использует **SearchExpression** группы подстановки. Элементы, которые входят в состав группы подстановки **SearchExpression** : [содержит](contains.md), [Excludes](excludes.md), [Exists](exists.md), [не](not.md), [или](or.md) [и](and.md), [выражение IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md) [IsGreaterThan ](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)и [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

