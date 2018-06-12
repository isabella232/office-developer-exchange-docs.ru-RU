---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: Элемент CalendarEvent представляет вхождение элемента уникальный календаря.
ms.openlocfilehash: f7fff7ba511ca12813dd4c2d694e89c97589ba31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761637"
---
# <a name="calendarevent"></a>CalendarEvent

Элемент **CalendarEvent** представляет вхождение элемента уникальный календаря. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 **CalendarEvent**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Время начала](starttime.md) <br/> |Представляет начало события календаря. Это обязательный дочерний элемент.  <br/> |
|[Время окончания](endtime.md) <br/> |Представляет конец события календаря. Это обязательный дочерний элемент.  <br/> |
|[BusyType](busytype.md) <br/> |Представляет состояние сведений о доступности для события календаря. Это обязательный дочерний элемент.  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |Дополнительные сведения для события календаря. Это необязательный дочерний элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |Содержит набор вхождений элемента уникальный календаря, которые представляют доступности запрошенного пользователя.  <br/> Ниже приведен выражение XPath 2.0 для этого элемента.  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>Замечания

Время встречи и собрания возвращается в часовом поясе клиента. Все дочерние элементы, перечислены в последовательности, в котором они изложены. Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

