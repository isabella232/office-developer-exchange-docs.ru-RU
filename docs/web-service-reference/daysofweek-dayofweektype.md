---
title: DaysOfWeek (DayOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: ba8f990d-d37d-403d-b31f-55e5208c8ad5
description: Элемент DaysOfWeek описывает дни недели, используемые в шаблонах повторения элементов.
ms.openlocfilehash: f30184755117c7561b66e93491cbd68534064eeb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525108"
---
# <a name="daysofweek-dayofweektype"></a>DaysOfWeek (DayOfWeekType)

Элемент **DaysOfWeek** описывает дни недели, используемые в шаблонах повторения элементов. 
  
```xml
<DaysOfWeek/>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительное ежегодное повторение.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Описывает относительную ежемесячную схему повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ниже перечислены возможные значения.
  
- Воскресенье    
- Понедельник    
- Вторник   
- Среда    
- Четверг    
- Пятница    
- Суббота    
- Day (не используется в TimeChangePatternTypes)    
- Будний день (не используется в TimeChangePatternTypes)    
- WeekendDay (не используется в TimeChangePatternTypes)
    
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

