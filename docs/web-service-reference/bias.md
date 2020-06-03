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
description: Элемент offset представляет смещение от смещения относительно всеобщего скоординированного времени (UTC), определенного элементом смещения (UTC) для стандартного времени и летнего времени. Это значение представлено в минутах.
ms.openlocfilehash: 6c9dce88f3eece9c793fb018114f07a85c7cb89b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460241"
---
# <a name="bias"></a>Bias

Элемент **offset** представляет смещение от смещения относительно всеобщего скоординированного времени (UTC), определенного элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени. Это значение представлено в минутах. 
  
```xml
<Bias>...</Bias>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.<br/><br/>Ниже приведены выражения XPath для элемента [StandardTime](standardtime.md) :<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.  <br/><br/>Ниже приведены выражения XPath для элемента [DaylightTime](daylighttime.md) :<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение представляет целое число.
  
## <a name="remarks"></a>Примечания

Смещение, используемое для определения локального времени, может быть предоставлено только одним из элементов **смещения** . Сумма значений элемента сдвига, предоставляемого элементом [DaylightTime](daylighttime.md) или элементом [StandardTime](standardtime.md) , кроме элемента [смещения (UTC)](bias-utc.md) , определяет местное время. 
  
## <a name="example"></a>Пример

В приведенном ниже примере показана часть XML-запроса, определяющая пользователя, который следит за переходом на летнее время, путем корректировки смещения относительно времени в формате UTC на-60 минут. Это позволяет эффективно отменять смещение 420 минут от времени в формате UTC.
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

