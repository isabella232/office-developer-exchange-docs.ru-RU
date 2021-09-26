---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: Элемент AggregationRestriction указывает значение, которое применяется к набору свойств Persona в результате запроса FindPeople и фильтрует результат в соответствии с указанным ограничением.
ms.openlocfilehash: 6a00035f87e0f365f4551df1a6ff570e01761770
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546793"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

Элемент **AggregationRestriction** указывает значение, которое применяется к набору свойств Persona в результате запроса FindPeople и фильтрует результат в соответствии с указанным ограничением. 
  
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
  
## <a name="remarks"></a>Заметки

Элемент **AggregationRestriction** может содержать любой детский элемент, использующий группу **замены SearchExpression.** Элементы, которые являются частью группы замены **SearchExpression** [являются:](contains.md) [](exists.md)Содержит [,](excludes.md)Исключает [](and.md), Существует , [Не](not.md) [,](or.md)Или , и , [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), IsGreaterThan , [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThanThan](islessthan.md)и [](isgreaterthan.md) [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

