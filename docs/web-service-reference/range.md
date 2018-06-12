---
title: Range
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Элемент Range указывает диапазон вхождения элемента календаря для повторяющегося элемента календаря.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834946"
---
# <a name="range"></a>Range

Элемент **Range** указывает диапазон вхождения элемента календаря для повторяющегося элемента календаря. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Start** <br/> |Текстовое значение атрибута **Начать** — это дата начала диапазона повторяющегося элемента. Это значение **даты и времени** .  <br/> |
|**End** <br/> |Текстовое значение атрибута **окончания** — это дата окончания диапазона повторяющегося элемента. Это значение **даты и времени** .  <br/> |
|**Count** <br/> |Текстовое значение атрибута **счетчика** — это число вхождений повторяющегося элемента. Это значение типа **integer** .  <br/> |
|**CompareOriginalStartTime** <br/> |Текстовое значение **true** для атрибута **CompareOriginalStartTime** указывает, что клиент должен сравнить исходное время начала с новое время начала. Значение **false** указывает, что клиент не нужно сравнить исходное время начала с новое время начала.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Диапазоны](ranges.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

