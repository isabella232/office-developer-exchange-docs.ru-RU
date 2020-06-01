---
title: аггрегатионрестриктион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: Элемент Аггрегатионрестриктион указывает значение, которое применяется к набору свойств пользователя, полученному при запросе FindPeople, и фильтрует результат в соответствии с указанным ограничением.
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463526"
---
# <a name="aggregationrestriction"></a>аггрегатионрестриктион

Элемент **аггрегатионрестриктион** указывает значение, которое применяется к набору свойств пользователя, полученному при запросе FindPeople, и фильтрует результат в соответствии с указанным ограничением. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **рестриктионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[сеарчекспрессион](searchexpression.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Примечания

Элемент **аггрегатионрестриктион** может содержать любой дочерний элемент, в котором используется группа подстановки **сеарчекспрессион** . Элементами, которые являются частью группы подстановки **сеарчекспрессион** : [Contains](contains.md), [Exclude](excludes.md), [Exists](exists.md), [Not](not.md), [or](or.md) [и](and.md), [исекуалто](isequalto.md), [иснотекуалто](isnotequalto.md), [исгреатерсан](isgreaterthan.md), [исгреатерсанорекуалто](isgreaterthanorequalto.md), [ислесссан](islessthan.md)и [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

