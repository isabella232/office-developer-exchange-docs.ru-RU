---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: Элемент RequestedView определяет тип данных календаря, для которого запрашивается клиента.
ms.openlocfilehash: 7710227720264432c325f95da894cbbbd4748dc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835145"
---
# <a name="requestedview"></a>RequestedView

Элемент **RequestedView** определяет тип данных календаря, для которого запрашивается клиента. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[RequestedView](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 **FreeBusyViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Указывает тип сведений о доступности, возвращаемого в ответе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Это значение не является допустимым для запросов. Это значение является допустимым для ответов.  <br/> |
|MergedOnly  <br/> |Представляет поток объединенные обмен сведениями о доступности. В сценариях между лесами, в которых конечного пользователя в одном лесу не использовать службу доступности настроен службу доступности, запрашивающего извлекает сведения о доступности конечного пользователя из занятости общих папок. Так как общие папки только хранятся сведения о доступности в объединенном формы, **MergedOnly** , доступны только сведения.  <br/> |
|FreeBusy  <br/> |Представляет сведения о состоянии прежних версий: бесплатная, «занят», под вопросом и об отсутствии на работе. Это также включает в себя времени начала или окончания встречи. В этом представлении функционального предоставляются не прежних версий занятости представления, так как отдельные собрания начала и окончания раз вместо поток объединенные обмен сведениями о доступности.  <br/> |
|FreeBusyMerged  <br/> |Представляет все свойства **занятости** с потоком объединенные сведения о доступности.  <br/> |
|Detailed  <br/> |Представляет сведения о состоянии прежних версий: бесплатная, «занят», под вопросом и OOF; время начала и окончания встречи; различные свойства и встречи, такие как тему, местоположение и важности. В этом требуемого представления возвращает максимальный объем сведений, для которого является привилегированной запрашивающего пользователя. Если объединенные сведения о доступности только, как с запросом информации для пользователей в лесу, Microsoft Exchange Server 2003, **MergedOnly** будут возвращены. В противном случае будут возвращены **занятости** или **Detailed** .  <br/> |
|DetailedMerged  <br/> |Представляет все свойства **Detailed** с потоком объединенные сведения о доступности. Если объединенные сведения о доступности только недоступны, будут возвращены **MergedOnly** . В противном случае будут возвращены **FreeBusyMerged** или **DetailedMerged** .  <br/> |
   
## <a name="remarks"></a>Замечания

Значение, установленное этот элемент возвращается с элемент [FreeBusyViewType](freebusyviewtype.md) в ответе. 
  
В следующей таблице перечислены элементы, возвращаемые для различных типов представлений и соответствующего свойства MAPI. Каждый тип представления основан на тип прежний режим.
  
|**Тип представления сведений о занятости**|**Свойства**|**Свойство Calendar MAPI**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |Классическая состояния  <br/> |Важный параметр PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Рабочее время  <br/> ||
|**FreeBusy** <br/> |Время начала  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |Время окончания  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |Классическая состояния  <br/> |Важный параметр PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Рабочее время  <br/> ||
|**FreeBusyMerged** <br/> |Время начала  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |Время окончания  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Подробное описание** <br/> |Классическая состояния  <br/> |Важный параметр PropTag (0x80860003)  <br/> |
|**Подробное описание** <br/> |Рабочее время  <br/> ||
|**Подробное описание** <br/> |Время начала  <br/> |PR_START_DATE  <br/> |
|**Подробное описание** <br/> |Время окончания  <br/> |PR_END_DATE  <br/> |
|**Подробное описание** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**Подробное описание** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**Подробное описание** <br/> |Запись Id(unless private)  <br/> ||
|**Подробное описание** <br/> |Флаг Private  <br/> ||
|**Подробное описание** <br/> |IsMeeting  <br/> ||
|**Подробное описание** <br/> |IsRecurring  <br/> ||
|**Подробное описание** <br/> |IsException  <br/> ||
|**Подробное описание** <br/> |IsReminderSet  <br/> ||
|**DetailedMerged** <br/> |Классическая состояния  <br/> |Важный параметр PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Рабочее время  <br/> ||
|**DetailedMerged** <br/> |Время начала  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Время окончания  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Запись Id(unless private)  <br/> ||
|**DetailedMerged** <br/> |Флаг Private  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
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

