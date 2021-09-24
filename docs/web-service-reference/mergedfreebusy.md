---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: Элемент MergedFreeBusy содержит объединенный свободный и загруженный поток данных.
ms.openlocfilehash: db451d6b2e67313836771604fae57b14b6b3db10
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511032"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

Элемент **MergedFreeBusy содержит** объединенный свободный и загруженный поток данных. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **строка**
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

Текстовое значение предоставляется сервером, если значение элемента [FreeBusyViewType](freebusyviewtype.md) является одним из следующих: 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
Текстовое значение — это поток бесплатных и загруженных сведений. 
  
## <a name="remarks"></a>Заметки

Поток данных, предоставляемый этим элементом, определяется элементами [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) и [TimeWindow.](timewindow.md) Элемент [TimeWindow](timewindow.md) определяет период времени, задаваемый для доступности. Элемент [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) определяет, как время от элемента [TimeWindow](timewindow.md) разбивается на интервалы, возвращаемые в **элементе MergedFreeBusy.** Каждое число в **потоке MergedFreeBusy** представляет один интервал, определенный элементом [MergedFreeBusyIntervalInMinutes.](mergedfreebusyintervalinminutes.md) В следующей таблице перечислены возможные значения для отдельного интервала. 
  
|**Digit**|**Доступность**|
|:-----|:-----|
|0  <br/> |Свободна  <br/> |
|1   <br/> |Предварительная  <br/> |
|2  <br/> |Занята  <br/> |
|3   <br/> |Отсутствие на работе (OOF)  <br/> |
|4   <br/> |Нет данных  <br/> |
   
Например, запрос на бесплатные/загруженные данные включает элемент [TimeWindow,](timewindow.md) который представляет четыре часа, и элемент [MergedFreeBusyIntervalInMinutes,](mergedfreebusyintervalinminutes.md) который представляет 60 минут. Если календарь запрашиваемого пользователя является OOF в течение первых 60 минут, занят в течение следующих 90 минут и не запланирован на последние 90 минут в окне времени, поток **MergedFreeBusy** будет 3220. Если интервал содержит несколько классификаций доступности, для классификации этого интервала используется самое большое число. 
  
Уровень детализации, предоставляемой этим элементом, зависит от разрешений, предоставленных запросчику.
  
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

