---
title: Time
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: Элемент времени представляет время перехода между зимнего и летнего времени.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840164"
---
# <a name="time"></a>Время

Элемент **времени** представляет время перехода между зимнего и летнего времени. 
  
```xml
<Time>...</Time>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.  <br/><br/>  Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) . <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени. Этот элемент также содержит сведения о когда происходит переход на летнее время.  <br/><br/>  Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет часов, минут и секунд в следующем формате: ЧЧ.
  
## <a name="remarks"></a>Замечания

При появлении элемента **времени** в элемент [DaylightTime](daylighttime.md) представляет время дня, осуществляется переход на летнее время происходит. При появлении элемента [времени](time.md) в элемент [StandardTime](standardtime.md) представляет время дня, происходит переход на летнее время. 
  
Этот элемент имеет минимальные вхождения нулевой и максимальное одно вхождение.
  
## <a name="example"></a>Пример

Следующие части запроса, представляющий время перехода от 2: 00. из стандартного времени на летнее время.
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

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

