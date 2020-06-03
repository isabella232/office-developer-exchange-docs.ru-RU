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
description: Элемент TimeZone содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460276"
---
# <a name="timezone-availability"></a>Часовой пояс (доступность)

Элемент **TimeZone** содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе со стандартного времени на летнее время. 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **сериализаблетимезоне**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сдвиг (UTC)](bias-utc.md) <br/> |Представляет общее смещение от времени в формате UTC. Это значение представлено в минутах.  <br/> |
|[StandardTime](standardtime.md) <br/> |Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетусераваилабилитирекуест](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователя. Это корневой элемент.  <br/> Элемент **TimeZone** в сообщении жетусераваилабилитирекуест представляет часовой пояс, в котором указаны значения DateTime в запросе. Значения даты и времени, возвращаемые службой доступности, также находятся в этом часовом поясе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[воркингхаурс](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.  <br/> Элемент **TimeZone** в сообщении жетусераваилабилитиреспонсе представляет параметры часового пояса запрошенного пользователя почтового ящика.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент является обязательным для элемента [жетусераваилабилитирекуест](getuseravailabilityrequest.md) . Этот элемент происходит не более одного раза или по крайней мере ноль раз, когда родительский элемент является элементом [воркингхаурс](workinghours-ex15websvcsotherref.md) . 
  
## <a name="example"></a>Пример

В приведенном ниже примере показана часть XML-запроса, которая определяет смещение относительно времени в формате UTC 8 часов в клиентском приложении.
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

