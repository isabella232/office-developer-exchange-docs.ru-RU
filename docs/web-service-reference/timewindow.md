---
title: Значение TimeWindow
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
description: Элемент значение TimeWindow указывает промежуток времени, запрос пользователя сведений о доступности.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840189"
---
# <a name="timewindow"></a>Значение TimeWindow

Элемент **значение TimeWindow** указывает промежуток времени, запрос пользователя сведений о доступности. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[Значение TimeWindow](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Срок действия**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Время начала](starttime.md) <br/> |Представляет начало промежуток времени, запрос пользователя сведений о доступности.  <br/> |
|[Время окончания](endtime.md) <br/> |Представляет конец промежуток времени, запрос пользователя сведений о доступности.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Указывает тип сведений о доступности, возвращаемого в ответе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Замечания

Максимальное значение для этого периода времени — 42 дня. Это максимальное значение может быть изменено. Все запросы на сведения о доступности пользователя за пределы максимальное значение возвращает ошибку. Если встречи, частично в промежуток времени, определенные в элементы [StartTime](starttime.md) и [EndTime](endtime.md) встречи включается целиком. 
  
> [!NOTE]
> Схема, описывающая этот элемент находится в каталоге /EWS/ компьютера, на котором выполняется Microsoft® Exchange Server 2007 с установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

