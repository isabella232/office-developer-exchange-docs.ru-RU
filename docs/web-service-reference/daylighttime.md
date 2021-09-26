---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: Элемент DaylightTime представляет смещение времени по отношению к координированному универсальному времени (UTC), которое представлено элементом Bias (UTC) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.
ms.openlocfilehash: 95d09fe01602f2d55d1a39dc7164a3f60a328f2a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543435"
---
# <a name="daylighttime"></a>DaylightTime

Элемент **DaylightTime** представляет смещение времени по отношению к координированному универсальному времени (UTC), которое представлено элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени. 
  
- [TimeZone (доступность)](timezone-availability.md) 
- [DaylightTime](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

**SerializableTimeZoneTime**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Представляет смещение от смещения UTC, которое определено элементом [Bias (UTC)](bias-utc.md) для стандартного времени и летнего времени. Это значение представлено в минутах.  <br/> |
|[Time](time.md) <br/> |Представляет время перехода от дня к обычному времени и времени летнего времени.  <br/> |
|[DayOrder](dayorder.md) <br/> |Представляет _n_th дня, указанного в элементе [DayOfWeek (TimeZone),](dayofweek-timezone.md) который представляет дату перехода от стандартного и летнего времени.  <br/> |
|[Month](month.md) <br/> |Представляет собой переходный месяц года к обычному времени и летнему времени.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Представляет день недели, когда происходит переход к обычному времени и летнему времени.  <br/> |
|[Год](year.md) <br/> |Используется для определения часовой пояс, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZone (доступность)](timezone-availability.md) <br/> | Содержит элементы, определяющие сведения о часовом поясе.<br/><br/>Этот элемент также содержит сведения о переходе между стандартным временем и летнее время.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>Пример

Следующий частичный запрос GetUserAvailability представляет клиентскую заявку в расположении, которое распознает летнее время.
  
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

