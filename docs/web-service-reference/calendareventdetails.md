---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: Дополнительные сведения о событии календаря элемент CalendarEventDetails.
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761639"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

Дополнительные сведения о событии календаря элемент **CalendarEventDetails** . 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 **CalendarEventDetails**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ИД](id.md) <br/> |Представляет идентификатор записи элемента календаря.  <br/> |
|[Тема (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Представляет Тема элемента календаря.  <br/> |
|[Расположение (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Представляет поле расположение элемента календаря.  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Указывает, является ли событие календаря собрания или встречи.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Указывает, является ли событие календаря экземпляр повторяющегося элемента календаря или элемента одного календаря.  <br/> |
|[IsException](isexception.md) <br/> |Указывает, изменяется ли экземпляр повторяющегося элемента календаря из образца.  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |Указывает, установил ли напоминания для событий календаря.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Указывает, является ли закрытый элемента календаря.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Представляет вхождение элемента уникальный календаря.  <br/> Ниже приведен выражение XPath 2.0 для этого элемента.  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Замечания

Все дочерние элементы, перечислены в последовательности, в котором они изложены. 
  
Если элемент [IsPrivate](isprivate.md) имеет **значение true**, в элементе [CalendarEventDetails](calendareventdetails.md) элементы не возвращаются в ответе. 
  
Операция GetUserAvailability не возвращает подробные сведения о нем только при наличии вызывающего доступ на чтение в календаре конечного пользователя. Можно задавать разрешения доступа с помощью командной консоли Exchange.
  
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

