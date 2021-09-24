---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: Элемент CalendarEvent представляет уникальный элемент календаря.
ms.openlocfilehash: fd57517595659f2081c82fe9f4665ce2c39059fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514825"
---
# <a name="calendarevent"></a>CalendarEvent

Элемент **CalendarEvent** представляет уникальный элемент календаря. 
  
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
|[StartTime](starttime.md) <br/> |Представляет начало события календаря. Это необходимый детский элемент.  <br/> |
|[EndTime](endtime.md) <br/> |Представляет собой конец события календаря. Это необходимый детский элемент.  <br/> |
|[BusyType](busytype.md) <br/> |Представляет набор состояния free/busy для события календаря. Это необходимый детский элемент.  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |Предоставляет дополнительные сведения для события календаря. Это необязательный детский элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |Содержит набор уникальных событий элементов календаря, которые представляют доступность запрашиваемого пользователя.  <br/> Ниже приводится выражение XPath 2.0 к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>Заметки

Время встречи и собрания возвращается в часовом поясе клиента. Все элементы ребенка перечислены в последовательности, в которой они происходят. Уровень детализации, предоставляемой этим элементом, зависит от разрешений, предоставленных запросчику.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

