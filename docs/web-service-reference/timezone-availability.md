---
title: Часовой пояс (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: Элемент TimeZone содержит элементы, чтобы указать часовой пояс сведения. Этот элемент также содержит сведения о переходе между зимнего и летнего времени.
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840205"
---
# <a name="timezone-availability"></a>Часовой пояс (доступность)

Элемент **TimeZone** содержит элементы, чтобы указать часовой пояс сведения. Этот элемент также содержит сведения о переходе между зимнего и летнего времени. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Смещение (UTC)](bias-utc.md) <br/> |Представляет общие смещение в формате UTC. Это значение представлено в минутах.  <br/> |
|[StandardTime](standardtime.md) <br/> |Представляет смещение от времени относительно UTC, представленный в элемент [Bias (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени. Этот элемент также содержит сведения о когда происходит переход на летнее время.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователя. Это корневой элемент.  <br/> Элемент **TimeZone** в сообщении GetUserAvailabilityRequest представляет часовой пояс, в котором указаны значения даты и времени в запросе. Значения даты и времени, возвращаемые службы доступности могут также в данном часовом поясе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.  <br/> Элемент **TimeZone** в сообщении GetUserAvailabilityResponse представляет параметры часового пояса запрошенные почтового ящика пользователя.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является обязательным в элементе [GetUserAvailabilityRequest](getuseravailabilityrequest.md) . Этот элемент возникает только один раз или по крайней мере ноль раз при родительский элемент представляет собой элемент [WorkingHours](workinghours-ex15websvcsotherref.md) . 
  
## <a name="example"></a>Пример

Следующий пример показывает часть запроса XML, который определяет смещение времени в формате UTC 8 часов в клиентском приложении.
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
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



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[Уровень защиты](bias.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

