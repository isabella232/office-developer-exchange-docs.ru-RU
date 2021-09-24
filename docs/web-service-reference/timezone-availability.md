---
title: TimeZone (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: Элемент TimeZone содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе между стандартным временем и летнее время.
ms.openlocfilehash: 7ca6f0f2d9950770055d19c04adab9b76b95c295
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538844"
---
# <a name="timezone-availability"></a>TimeZone (доступность)

Элемент **TimeZone** содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе между стандартным временем и летнее время. 
  
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
|[Bias (UTC)](bias-utc.md) <br/> |Представляет общий смещение от скоординированного универсального времени (UTC). Это значение представлено в минутах.  <br/> |
|[StandardTime](standardtime.md) <br/> |Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC).](bias-utc.md) Этот элемент также содержит сведения о переходе на стандартное время с летнего времени в регионах, где наблюдается летнее время.  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Представляет смещение времени по отношению к UTC, представленного элементом [Bias (UTC)](bias-utc.md) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время со стандартного времени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Содержит аргументы, используемые для получения сведений о доступности пользователей. Это корневой элемент.  <br/> Элемент **TimeZone** в сообщении GetUserAvailabilityRequest представляет часовой пояс, в котором заданы значения DateTime в запросе. Значения DateTime, возвращенные службой доступности, также находятся в этом часовом поясе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часовой зоны и рабочие часы для запрашиваемой пользователя почтового ящика.  <br/> Элемент **TimeZone** в сообщении GetUserAvailabilityResponse представляет параметры часового пояса запрашиваемого пользователя почтового ящика.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент необходим в [элементе GetUserAvailabilityRequest.](getuseravailabilityrequest.md) Этот элемент возникает не чаще одного или хотя бы нулевого времени, когда родительский элемент является [элементом WorkingHours.](workinghours-ex15websvcsotherref.md) 
  
## <a name="example"></a>Пример

В следующем примере показана часть XML-запроса, который определяет смещение от UTC в клиентское приложение в течение 8 часов.
  
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
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[Bias](bias.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

