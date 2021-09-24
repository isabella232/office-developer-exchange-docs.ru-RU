---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: Элемент DayOfWeek представляет день недели, в который происходит переход часового пояса.
ms.openlocfilehash: 5b51a3692a1836d2d2448df88b0ec07ccf1d79a5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519900"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (TimeZone)

Элемент **DayOfWeek** представляет день недели, в который происходит переход часового пояса. 
  
```xml
<DayOfWeek>...</DayOfWeek>
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
|[StandardTime](standardtime.md) <br/> | Представляет смещение времени по отношению к координированному универсальному времени (UTC), представленного элементом [Bias (UTC).](bias-utc.md)<br/><br/>Этот элемент также содержит сведения о переходе на стандартное время с летнего времени в регионах, где наблюдается летнее время.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.<br/><br/>Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часовой зоны, который происходит каждый год в один и тот же день.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представлено переумежением, которое имеет следующие возможные значения:
  
- Воскресенье    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота    
- Day    
- День недели   
- WeekendDay
    
## <a name="remarks"></a>Заметки

Элемент [StandardTime,](standardtime.md) содержащий элемент [DayOrder](dayorder.md) со значением 5, элемент Месяц со значением 10, а элемент **DayOfWeek** со значением воскресенья означает, что переход от стандартного времени к летнему времени происходит в пятое воскресенье десятого месяца. [](month.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

