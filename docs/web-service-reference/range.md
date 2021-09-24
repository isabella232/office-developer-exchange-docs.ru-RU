---
title: Диапазон
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Элемент Range указывает диапазон событий элементов календаря для повторяют элемент календаря.
ms.openlocfilehash: 0d16dad24dda48f084b3011d7b96eb719431d9da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519102"
---
# <a name="range"></a>Диапазон

Элемент **Range** указывает диапазон событий элементов календаря для повторяют элемент календаря. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Start** <br/> |Текстовое значение атрибута **Начните** — это дата начала повторяющегося диапазона элементов. Это значение **dateTime.**  <br/> |
|**End** <br/> |Текстовое значение атрибута **End** — это дата окончания диапазона повторяющихся элементов. Это значение **dateTime.**  <br/> |
|**Count** <br/> |Текстовое значение **атрибута Count** — это количество вхождений повторяющегося элемента. Это значение **в несколько раз.**  <br/> |
|**CompareOriginalStartTime** <br/> |Текстовое значение **true** для атрибута **CompareOriginalStartTime** указывает на то, что клиент должен сравнить исходное время начала с новым временем начала. Значение false **указывает** на то, что клиенту не нужно сравнивать исходное время начала с новым временем начала.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Ranges](ranges.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

