---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: Элемент DaylightTime представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом смещения (UTC) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.
ms.openlocfilehash: 350fcb4ce278f423c62fcc5ecaa160eda71e4a2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455655"
---
# <a name="daylighttime"></a>DaylightTime

Элемент **DaylightTime** представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (](bias-utc.md) UTC) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени. 
  
- [Часовой пояс (доступность)](timezone-availability.md) 
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

**сериализаблетимезонетиме**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Представляет смещение относительно времени в формате UTC, которое определено элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени. Это значение представлено в минутах.  <br/> |
|[Time](time.md) <br/> |Представляет время перехода на зимнее и зимнее время и обратно.  <br/> |
|[дайордер](dayorder.md) <br/> |Представляет _n_th день недели, указанный в элементе [DayOfWeek (TimeZone)](dayofweek-timezone.md) , который представляет дату перехода со стандартного и летнего времени.  <br/> |
|[Month](month.md) <br/> |Представляет переходный месяц года от стандартного и летнего времени.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Представляет день недели, когда происходит переход на зимнее и зимнее время и на летнее время.  <br/> |
|[Год](year.md) <br/> |Используется для определения часового пояса, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Часовой пояс (доступность)](timezone-availability.md) <br/> | Содержит элементы, определяющие сведения о часовом поясе.<br/><br/>Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>Пример

Следующий частичный запрос GetUserAvailability представляет клиентское приложение в расположении, которое распознает летнее время.
  
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

