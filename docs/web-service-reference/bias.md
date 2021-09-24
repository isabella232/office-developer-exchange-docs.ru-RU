---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: Элемент Bias представляет смещение смещения от смещения согласованного универсального времени (UTC), установленного элементом Bias (UTC) для стандартного времени и летнего времени. Это значение представлено в минутах.
ms.openlocfilehash: 557605380dbda8c980272edcf445bb8099e14ada
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516099"
---
# <a name="bias"></a>Bias

Элемент **Bias** представляет смещение смещения от смещения согласованного универсального времени (UTC), установленного элементом [Bias (UTC)](bias-utc.md) для стандартного времени и летнего времени. Это значение представлено в минутах. 
  
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
|[StandardTime](standardtime.md) <br/> | Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC).](bias-utc.md) Этот элемент также содержит сведения о переходе на стандартное время с летнего времени в регионах, где наблюдается летнее время.<br/><br/>Ниже приводится выражение XPath к [элементу StandardTime:](standardtime.md)<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.  <br/><br/>Ниже приводится выражение XPath к [элементу DaylightTime:](daylighttime.md)<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет собой integer.
  
## <a name="remarks"></a>Заметки

Смещение, используемого для определения местного времени, может быть предоставлено только одним из элементов **Bias.** Сумма значений элемента Bias, предоставляемого элементом [DaylightTime](daylighttime.md) или элементом [StandardTime](standardtime.md) плюс элемент [Bias (UTC),](bias-utc.md) определяет местное время. 
  
## <a name="example"></a>Пример

В следующем примере показана часть XML-запроса, который определяет пользователя, который соблюдает летнее время, корректирует смещение от UTC на -60 минут. Это эффективно делает смещение в 420 минутах от UTC.
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

