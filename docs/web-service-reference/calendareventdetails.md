---
title: календаревентдетаилс
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
description: Элемент Календаревентдетаилс предоставляет дополнительные сведения о событии календаря.
ms.openlocfilehash: 3e1dbba00bce4a1fdc53f3330527764c516890ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459071"
---
# <a name="calendareventdetails"></a>календаревентдетаилс

Элемент **календаревентдетаилс** предоставляет дополнительные сведения о событии календаря. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
[календаревентаррай](calendareventarray.md)
  
[календаревент](calendarevent.md)
  
[календаревентдетаилс](calendareventdetails.md)
  
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

 **календаревентдетаилс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ID](id.md) <br/> |Представляет идентификатор записи элемента календаря.  <br/> |
|[Subject (Календаревентдетаилс)](subject-calendareventdetails.md) <br/> |Представляет тему элемента календаря.  <br/> |
|[Местоположение (Календаревентдетаилс)](location-calendareventdetails.md) <br/> |Представляет поле расположения элемента календаря.  <br/> |
|[Проведенное собрание (Календаревентдетаилс)](ismeeting-calendareventdetails.md) <br/> |Указывает, является ли событие календаря собранием или встречей.  <br/> |
|[IsRecurring (Календаревентдетаилс)](isrecurring-calendareventdetails.md) <br/> |Указывает, является ли событие Calendar экземпляром повторяющегося элемента календаря или одним элементом календаря.  <br/> |
|[Исключение](isexception.md) <br/> |Указывает, изменяется ли экземпляр повторяющегося элемента календаря с основного.  <br/> |
|[Попамятка](isreminderset.md) <br/> |Указывает, задано ли напоминание для события календаря.  <br/> |
|[Частный](isprivate.md) <br/> |Указывает, является ли элемент календаря частным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаревент](calendarevent.md) <br/> |Представляет уникальное вхождение элемента календаря.  <br/> Ниже приведено выражение XPath 2,0 для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>Примечания

Все дочерние элементы перечислены в той последовательности, в которой они выполняются. 
  
Если элемент с параметром- [Private](isprivate.md) имеет **значение true**, все остальные элементы в элементе [календаревентдетаилс](calendareventdetails.md) не возвращаются в ответе. 
  
Операция GetUserAvailability не возвращает подробные сведения о вызывающем абоненте, если у вызывающего абонента нет прав на чтение в календаре целевого пользователя. Для настройки разрешений доступа можно использовать командную консоль Exchange.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

