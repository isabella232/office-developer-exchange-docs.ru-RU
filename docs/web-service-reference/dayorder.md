---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: Элемент DayOrder представляет nth возникновение дня, указанного в элементе DayOfWeek (TimeZone), который представляет дату перехода от стандартного времени и летнего времени.
ms.openlocfilehash: bc216984a92fef58ac6f46dc4646a0deca837563
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543445"
---
# <a name="dayorder"></a>DayOrder

Элемент **DayOrder** представляет _n_th дня, указанного в элементе [DayOfWeek (TimeZone),](dayofweek-timezone.md) который представляет дату перехода от стандартного и летнего времени. 
  
```xml
<DayOrder>...</DayOrder>
```

**short**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение времени по отношению к координированному универсальному времени (UTC), представленного элементом [Bias (UTC).](bias-utc.md)<br/><br/>Этот элемент также содержит сведения о переходе на стандартное время с летнего времени в регионах, где наблюдается летнее время.<br/><br/>Ниже приводится выражение XPath к [элементу StandardTime:](standardtime.md)<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.<br/><br/>Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.<br/><br/>Ниже приводится выражение XPath к [элементу DaylightTime:](daylighttime.md)<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Значение элемента **DayOrder** может быть от 1 до 5. Максимальное значение для этого элемента может быть 4 или 5 в зависимости от месяца и года. 
  
## <a name="remarks"></a>Заметки

Элемент [StandardTime,](standardtime.md) содержащий элемент **DayOrder** со значением 5, элемент Месяц со значением 10, и элемент [DayOfWeek (TimeZone),](dayofweek-timezone.md) который имеет значение воскресенье, означает, что переход от стандартного времени к летнему времени происходит в пятое воскресенье десятого месяца. [](month.md) 
  
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

