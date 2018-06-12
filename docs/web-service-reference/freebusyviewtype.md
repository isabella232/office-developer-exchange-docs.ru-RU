---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: Элемент FreeBusyViewType представляет тип сведений о доступности, возвращаемого в ответе.
ms.openlocfilehash: fe965d062f72d99dff7148f4d00b12fd8c4e1366
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762675"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

Элемент **FreeBusyViewType** представляет тип сведений о доступности, возвращаемого в ответе. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
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
|[FreeBusyView](freebusyview.md) <br/> |Содержит сведения о доступности для конкретного пользователя.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Это значение не является допустимым для запросов. Это значение является допустимым для ответов.  <br/> |
|MergedOnly  <br/> |Представляет поток объединенные обмен сведениями о доступности. В сценариях между лесами, в которых конечного пользователя в одном лесу не использовать службу доступности настроен службу доступности, запрашивающего извлекает сведения о доступности конечного пользователя из занятости общих папок. Так как общие папки только хранятся сведения о доступности в объединенном формы, **MergedOnly** , доступны только сведения.  <br/> |
|FreeBusy  <br/> |Представляет сведения о состоянии прежних версий: бесплатная, «занят», под вопросом и об отсутствии на работе. Это также включает в себя времени начала или окончания встречи. В этом представлении функционального предоставляются не прежних версий занятости представления, так как отдельные собрания начала и окончания раз вместо поток объединенные обмен сведениями о доступности.  <br/> |
|FreeBusyMerged  <br/> |Представляет все свойства **занятости** с потока данных объединенные доступность сведений о доступности.  <br/> |
|Detailed  <br/> |Представляет сведения о состоянии прежних версий: бесплатная, «занят», под вопросом и OOF; время начала и окончания встречи; различные свойства и встречи, такие как тему, местоположение и важности. В этом требуемого представления возвращает максимальный объем сведений, для которого является привилегированной запрашивающего пользователя. Если объединенные сведения о доступности только, как с запросом информации для пользователей в лесу, Microsoft Exchange Server 2003, **MergedOnly** будут возвращены. В противном случае будут возвращены **занятости** или **Detailed** .  <br/> Если **Detailed** указан для списка рассылки, объединенные сведения о доступности для участников списка, и возвращается **MergedOnly** .  <br/> |
|DetailedMerged  <br/> |Представляет все свойства **Detailed** с потока данных объединенные доступность сведений о доступности. Если объединенные сведения о доступности доступен только, например, если почтовый ящик существует на компьютере под управлением Exchange 2003, будут возвращены **MergedOnly** . В противном случае будут возвращены **FreeBusyMerged** или **DetailedMerged** .  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является обязательным, если используется элемент [FreeBusyView](freebusyview.md) . Тип возвращаемых сведений о доступности определенных в элементе [RequestedView](requestedview.md) . Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
В следующей таблице перечислены элементы, возвращаемые для различных типов представлений и соответствующего свойства MAPI. Каждый тип представления основан на тип прежний режим.
  
|**FreeBusyViewType**|**Свойства**|**Свойство Calendar MAPI**|
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
|**Подробное описание** <br/> |Сообщения об отсутствии (при необходимости)  <br/> ||
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
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

