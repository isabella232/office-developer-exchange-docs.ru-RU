---
title: Time
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: Элемент Time представляет время перехода от дня к обычному времени и времени летнего времени.
ms.openlocfilehash: d9cd83a7dcb0a296693e3daa1874b12294de5857
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513271"
---
# <a name="time"></a>Time

Элемент **Time** представляет время перехода от дня к обычному времени и времени летнего времени. 
  
```xml
<Time>...</Time>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение времени по отношению к координированному универсальному времени (UTC), представленного элементом [Bias (UTC).](bias-utc.md) Этот элемент также содержит сведения о переходе на стандартное время с летнего времени в регионах, где наблюдается летнее время.  <br/><br/>  Ниже приводится выражение XPath к [элементу StandardTime:](standardtime.md) <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.  <br/><br/>  Ниже приводится выражение XPath к [элементу DaylightTime:](daylighttime.md)  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет часы, минуты и секунды в следующем формате: hh:mm:ss.
  
## <a name="remarks"></a>Заметки

Когда элемент **Time** возникает в [элементе DaylightTime,](daylighttime.md) он представляет время суток, когда происходит переход от летнего времени к обычному. Когда элемент [Time](time.md) возникает в [элементе StandardTime,](standardtime.md) он представляет время суток, когда происходит переход от стандартного времени к летнему времени. 
  
Этот элемент имеет минимальное значение нуль и максимальное число случаев.
  
## <a name="example"></a>Пример

Следующая часть запроса представляет собой время перехода в 2 часа. от стандартного времени до летнего времени.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

