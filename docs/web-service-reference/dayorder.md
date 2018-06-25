---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: Элемент DayOrder представляет n-й вхождения день, заданный в элемент DayOfWeek (часовой пояс), который представляет дату перехода и зимнего и летнего времени.
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761998"
---
# <a name="dayorder"></a>DayOrder

Элемент **DayOrder** представляет вхождение _n_th день, заданный в элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который представляет дату перехода и зимнего и летнего времени. 
  
```xml
<DayOrder>...</DayOrder>
```

**короткие**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .<br/><br/>Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.<br/><br/>Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) .<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.<br/><br/>Этот элемент также содержит сведения о когда происходит переход на летнее время.<br/><br/>Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Значение для элемента **DayOrder** может быть от 1 до 5. Максимальное значение для этого элемента может быть 4 и 5, в зависимости от того, месяц и год. 
  
## <a name="remarks"></a>Замечания

Элемент [StandardTime](standardtime.md) , который содержит элемент **DayOrder** , который имеет значение 5, [месяц](month.md) , который имеет значение 10 и элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который имеет значение воскресенье означает, что переход к летнее время выполняется на пятом воскресенье десятой месяца. 
  
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

