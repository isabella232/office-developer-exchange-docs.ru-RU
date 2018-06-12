---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: Элемент StandardTime представляет смещение от времени относительно времени в формате UTC, представленный в элемент Bias (UTC). Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835546"
---
# <a name="standardtime"></a>StandardTime

Элемент **StandardTime** представляет смещение от времени относительно времени в формате UTC, представленный в элемент [Bias (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени. 
  
- [Часовой пояс (доступность)](timezone-availability.md)
- [StandardTime](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 **SerializableTimeZoneTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уровень защиты](bias.md) <br/> |Представляет смещение из времени UTC, который идентифицируется средством элемент [Bias (UTC)](bias-utc.md) для зимнего и летнего времени. Это значение представлено в минутах.  <br/> |
|[Time](time.md) <br/> |Представляет время перехода между зимнего и летнего времени.  <br/> |
|[DayOrder](dayorder.md) <br/> |Представляет _n_th вхождения день, указанный в элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который представляет дату перехода и зимнего и летнего времени.  <br/> |
|[Месяц](month.md) <br/> |Представляет перехода месяц года между зимнего и летнего времени.  <br/> |
|[DayOfWeek (часовой пояс)](dayofweek-timezone.md) <br/> |Представляет день недели, когда происходит переход на и с зимнего и летнего времени.  <br/> |
|[Год](year.md) <br/> |Определяет часовой пояс, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Часовой пояс (доступность)](timezone-availability.md) <br/> | Содержит элементы, чтобы указать часовой пояс сведения. Этот элемент также содержит сведения о переходе между зимнего и летнего времени. <br/><br/>Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **StandardTime** представляет смещения времени, которая представляется элемент [Bias (UTC)](bias-utc.md) . Если дочерний элемент [Bias](bias.md) равно 0, стандартное время равно некоторым смещением от времени UTC, представленный в элемент [Bias (UTC)](bias-utc.md) . 
  
## <a name="example"></a>Пример

В следующем примере показано область, где наблюдается летнего времени. Наблюдаемое осуществляется переход на летнее время в 2: 00. на пятом воскресенье десятой месяца.
  
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

