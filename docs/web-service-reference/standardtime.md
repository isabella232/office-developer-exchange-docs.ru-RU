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
description: Элемент StandardTime представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом смещения (UTC). Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835546"
---
# <a name="standardtime"></a>StandardTime

Элемент **StandardTime** представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время. 
  
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

 **сериализаблетимезонетиме**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Bias](bias.md) <br/> |Представляет смещение относительно времени в формате UTC, которое определено элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени. Это значение представлено в минутах.  <br/> |
|[Time](time.md) <br/> |Представляет время перехода на зимнее и зимнее время и обратно.  <br/> |
|[дайордер](dayorder.md) <br/> |Представляет _n_th день недели, указанный в элементе [DayOfWeek (TimeZone)](dayofweek-timezone.md) , который представляет дату перехода со стандартного и летнего времени.  <br/> |
|[Month](month.md) <br/> |Представляет переходный месяц года от стандартного и летнего времени.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Представляет день недели, когда происходит переход на зимнее и зимнее время и на летнее время.  <br/> |
|[Год](year.md) <br/> |Определяет часовой пояс, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Часовой пояс (доступность)](timezone-availability.md) <br/> | Содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе со стандартного времени на летнее время. <br/><br/>Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **StandardTime** представляет время смещения, представленное элементом [смещения (UTC)](bias-utc.md) . Если дочерний элемент [сдвига](bias.md) равен 0, стандартное время равно смещению смещения относительно времени в формате UTC, которое представлено элементом [смещения (UTC)](bias-utc.md) . 
  
## <a name="example"></a>Пример

В следующем примере показан регион, в котором наблюдается летнее время. Переход с летнего на зимнее время выполняется в 2 часа утра. в пятом воскресенье десятого месяца.
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

