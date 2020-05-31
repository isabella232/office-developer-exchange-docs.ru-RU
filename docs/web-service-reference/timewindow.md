---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: Элемент TimeWindow определяет интервал времени, запрошенный для сведений о доступности пользователя.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840189"
---
# <a name="timewindow"></a>TimeWindow

Элемент **TimeWindow** определяет интервал времени, запрошенный для сведений о доступности пользователя. 
  
[жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
[фрибусивиевоптионс](freebusyviewoptions.md)
  
[TimeWindow](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Представляет начало интервала времени, запрошенного для сведений о доступности пользователя.  <br/> |
|[EndTime](endtime.md) <br/> |Представляет конец интервала времени, запрошенного для сведений о доступности пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусивиевоптионс](freebusyviewoptions.md) <br/> |Указывает тип сведений о доступности, возвращаемых в ответе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Примечания

Максимальное значение для этого периода времени составляет 42 дней. Это максимальное значение можно изменить. Все запросы сведений о доступности пользователей за пределами максимального значения будут возвращать ошибку. Если какие-либо встречи частично указаны в диапазоне времени, определенном элементами [StartTime](starttime.md) и [EndTime](endtime.md) , эта встреча включается целиком. 
  
> [!NOTE]
> Схема, описывающая этот элемент, находится в каталоге/ЕВС/компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

