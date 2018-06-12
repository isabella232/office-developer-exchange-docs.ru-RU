---
title: DayOfWeek (часовой пояс)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: Элемент DayOfWeek представляет день недели, на котором происходит переход часового пояса.
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761993"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (часовой пояс)

Элемент **DayOfWeek** представляет день недели, на котором происходит переход часового пояса. 
  
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
|[StandardTime](standardtime.md) <br/> | Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .<br/><br/>Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.<br/><br/>Этот элемент также содержит сведения о когда происходит переход на летнее время.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часового пояса, что происходит в тот же день каждый год.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представлено перечислением, который имеет следующие возможные значения:
  
- Воскресенье    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота    
- День    
- День недели   
- WeekendDay
    
## <a name="remarks"></a>Замечания

Элемент [StandardTime](standardtime.md) , который содержит элемент [DayOrder](dayorder.md) , который имеет значение 5, [месяц](month.md) , который имеет значение 10 и элемент **DayOfWeek** , который имеет значение воскресенье означает, что переход на летнее экономии времени происходящее в пятый воскресенье десятой месяца. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

