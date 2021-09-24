---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: Элемент FreeBusyViewType представляет тип свободной и занятой информации, возвращаемой в ответе.
ms.openlocfilehash: 6eec490b39ccb9c02e7a16c8da7cfdd57f9b92c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509926"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

Элемент **FreeBusyViewType** представляет тип свободной и занятой информации, возвращаемой в ответе. 
  
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
|[FreeBusyView](freebusyview.md) <br/> |Содержит сведения о доступности для определенного пользователя.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Это значение не допустимо для запросов. Это значение допустимо для ответов.  <br/> |
|MergedOnly  <br/> |Представляет агрегированные потоки свободного и загруженного. В межлесных сценариях, в которых целевому пользователю в одном лесу не настроена служба доступности, служба доступности запрашиваемого запроса извлекает бесплатные и загруженные сведения целевого пользователя из свободной/занятой публичной папки. Так как общедоступные папки хранят только сведения о свободном или загруженном доступе в объединенной форме, **только MergedOnly** является доступной информацией.  <br/> |
|FreeBusy  <br/> |Представляет устаревшие сведения о состоянии: бесплатные, занятые, предварительные и OOF. Это также включает время начала и окончания встреч. Это представление богаче, чем устаревшее бесплатное и занятое представление, так как вместо агрегированного свободного/загруженного потока предоставляются отдельные время начала и окончания собрания.  <br/> |
|FreeBusyMerged  <br/> |Представляет все свойства **в FreeBusy** с потоком объединенных сведений о доступности бесплатной и загруженной.  <br/> |
|Подробные сведения  <br/> |Представляет устаревшие сведения о состоянии: бесплатные, занятые, предварительные и OOF; время начала и окончания встреч; и различные свойства встречи, такие как тема, расположение и значение. Это запрашиваемая точка зрения возвращает максимальное количество сведений, для которых запрашивающий пользователь имеет привилегии. Если будет доступна только информация о свободном или загруженном доступе, как и при запросе сведений для пользователей в лесу 2003 Microsoft Exchange Server 2003 года, **MergedOnly** будет возвращена. В противном **случае возвращается FreeBusy** или **Detailed.**  <br/> Если **подробные** сведения указаны для списка рассылки, сведения о свободном/занятом доступе для участников списка сливаются, и **возвращается MergedOnly.**  <br/> |
|DetailedMerged  <br/> |Представляет все свойства в **Detailed** с потоком объединенных сведений о доступности свободной и загруженной работы. Если доступна только информация о свободном или загружении, например, если почтовый ящик существует на компьютере Exchange 2003 г., **MergedOnly** будет возвращена. В противном **случае будет возвращено freeBusyMerged** или **DetailedMerged.**  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент необходим, если используется элемент [FreeBusyView.](freebusyview.md) Тип возвращаемой бесплатной и занятой информации обозначен в [элементе RequestedView.](requestedview.md) Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
В следующей таблице показано, что возвращается для различных типов представлений и соответствующего свойства MAPI. Каждый тип представления строится на прежнем типе представления.
  
|**FreeBusyViewType**|**Свойства**|**Свойство MAPI Calendar**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |Классический статус  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Рабочие часы  <br/> ||
|**FreeBusy** <br/> |Время запуска  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |время окончания.  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |Классический статус  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Рабочие часы  <br/> ||
|**FreeBusyMerged** <br/> |Время запуска  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |время окончания.  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Подробные сведения** <br/> |Классический статус  <br/> |PropTag (0x80860003)  <br/> |
|**Подробные сведения** <br/> |Рабочие часы  <br/> ||
|**Подробные сведения** <br/> |Время запуска  <br/> |PR_START_DATE  <br/> |
|**Подробные сведения** <br/> |время окончания.  <br/> |PR_END_DATE  <br/> |
|**Подробные сведения** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**Подробные сведения** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**Подробные сведения** <br/> |Entry-Id (если только не частное)  <br/> ||
|**Подробные сведения** <br/> |Частный флаг  <br/> ||
|**Подробные сведения** <br/> |IsMeeting  <br/> ||
|**Подробные сведения** <br/> |IsRecurring  <br/> ||
|**Подробные сведения** <br/> |IsException  <br/> ||
|**Подробные сведения** <br/> |IsReminderSet  <br/> ||
|**Подробные сведения** <br/> |Из сообщения Office (при запросе)  <br/> ||
|**DetailedMerged** <br/> |Классический статус  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Рабочие часы  <br/> ||
|**DetailedMerged** <br/> |Время запуска  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |время окончания.  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Location  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Entry-Id (если только не частное)  <br/> ||
|**DetailedMerged** <br/> |Частный флаг  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
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

