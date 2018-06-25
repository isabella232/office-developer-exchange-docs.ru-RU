---
title: Месяц
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: Элемент Month представляет перехода месяц года между зимнего и летнего времени.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834476"
---
# <a name="month"></a>Месяц

Элемент **Month** представляет перехода месяц года между зимнего и летнего времени. 
  
```xml
<Month>...</Month>
```

 **Короткие**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) . Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени. <br/> <br/>  Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) . <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени. Этот элемент также содержит сведения о когда происходит переход на летнее время.  <br/><br/>  Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Значение представляет порядковый номер ранг месяца появления и должно быть числом между 1 и 12. Это тип данных короткое целое число.
  
## <a name="remarks"></a>Замечания

Элемент [StandardTime](standardtime.md) , который содержит элемент [DayOrder](dayorder.md) , который имеет значение 5, **месяц** , который имеет значение 10 и элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который имеет значение воскресенье означает, что переход к летнее время выполняется на пятом воскресенье десятой месяца. 
  
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

