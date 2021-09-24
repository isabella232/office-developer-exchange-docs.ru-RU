---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: Элемент CalendarEventDetails предоставляет дополнительные сведения о событии календаря.
ms.openlocfilehash: c332d17b1bb630b9635e64c484b4c5fd989f9845
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516092"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

Элемент **CalendarEventDetails предоставляет** дополнительные сведения о событии календаря. 
  
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
|[ID](id.md) <br/> |Представляет ID записи элемента календаря.  <br/> |
|[Subject (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |Представляет субъект элемента календаря.  <br/> |
|[Location (CalendarEventDetails)](location-calendareventdetails.md) <br/> |Представляет поле расположения элемента календаря.  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |Указывает, является ли событие календаря собранием или встречей.  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |Указывает, является ли событие календаря экземпляром повторяющегося элемента календаря или одним элементом календаря.  <br/> |
|[IsException](isexception.md) <br/> |Указывает, изменен ли экземпляр повторяющегося элемента календаря из мастера.  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |Указывает, установлено ли напоминание для события календаря.  <br/> |
|[IsPrivate](isprivate.md) <br/> |Указывает, является ли элемент календаря закрытым.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |Представляет уникальный случай элементов календаря.  <br/> Ниже приводится выражение XPath 2.0 к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Заметки

Все элементы ребенка перечислены в последовательности, в которой они происходят. 
  
Если элемент [IsPrivate](isprivate.md) является **верным,** все остальные элементы элемента [CalendarEventDetails](calendareventdetails.md) не возвращаются в ответ. 
  
Операция GetUserAvailability не возвращает подробные сведения об вызываемом пользователе, если только он не прочитает доступ в календаре целевого пользователя. Разрешения доступа можно установить с помощью Exchange.
  
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

