---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: Элемент DateTimePrecision указывает точность для значений, возвращаемых даты и времени.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761976"
---
# <a name="datetimeprecision"></a>DateTimePrecision

Элемент **DateTimePrecision** указывает точность для значений, возвращаемых даты и времени. 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

Элемент **DateTimePrecision** находится в заголовке SOAP. 
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Ниже перечислены возможные значения.
  
- Секунд
    
- Мс
    
## <a name="remarks"></a>Замечания

Дата и время, когда используется заголовок SOAP с элементом **DateTimePrecision** , задайте значение «Секунд», возвращаемые значения ближайшего секунд (00: 00:00). При использовании «Миллисекундах» Дата/время значения возвращаются до ближайшей миллисекунды (00:00:00.0000). 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

