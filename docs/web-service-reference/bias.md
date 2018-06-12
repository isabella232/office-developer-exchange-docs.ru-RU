---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: Элемент Bias представляет смещение из смещения по Гринвичу (UTC), определяемую средством элемент Bias (UTC) для зимнего и летнего времени. Это значение представлено в минутах.
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761563"
---
# <a name="bias"></a>Bias

Элемент **Bias** представляет смещение из смещения по Гринвичу (UTC), определяемую средством элемент [Bias (UTC)](bias-utc.md) для зимнего и летнего времени. Это значение представлено в минутах. 
  
```xml
<Bias>...</Bias>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение от времени относительно UTC, представленный в элемент [Bias (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.<br/><br/>Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) .<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени. Этот элемент также содержит сведения о когда происходит переход на летнее время.  <br/><br/>Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет собой целое число.
  
## <a name="remarks"></a>Замечания

Смещение используется для определения местного времени может предоставить только с помощью одного из элементов **Bias** . Сумма значений элемент Bias предоставлено элемент [DaylightTime](daylighttime.md) или элемент [StandardTime](standardtime.md) , а также элемент [Bias (UTC)](bias-utc.md) идентифицирует местного времени. 
  
## <a name="example"></a>Пример

Следующий пример показывает часть запроса XML, который идентифицирует пользователя, должно соответствовать летнего времени, настраивая смещение от времени UTC,-60 минут. Это фактически делает сдвиг 420 минут времени в формате UTC.
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
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

