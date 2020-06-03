---
title: мержедфрибуси
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: Элемент Мержедфрибуси содержит Объединенный поток данных о занятости.
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468728"
---
# <a name="mergedfreebusy"></a>мержедфрибуси

Элемент **мержедфрибуси** содержит Объединенный поток данных о занятости. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
[мержедфрибуси](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусивиев](freebusyview.md) <br/> |Содержит сведения о доступности для определенного пользователя.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение предоставляется сервером, если для элемента [фрибусивиевтипе](freebusyviewtype.md) задано одно из следующих значений: 
  
- детаиледмержед
    
- фрибусимержед
    
- мержедонли
    
Текстовое значение — это поток сведений о занятости. 
  
## <a name="remarks"></a>Примечания

Поток данных, предоставляемых этим элементом, определяется элементами [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) и [TimeWindow](timewindow.md) . Элемент [TimeWindow](timewindow.md) определяет временной интервал, запрашиваемый для обеспечения доступности. Элемент [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) определяет, как время из элемента [TimeWindow](timewindow.md) разбивается на интервалы, возвращаемые в элементе **мержедфрибуси** . Каждое число в потоке **мержедфрибуси** представляет собой один интервал, заданный элементом [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) . В следующей таблице перечислены возможные значения для отдельного интервала. 
  
|**Четырехзначные**|**Доступность**|
|:-----|:-----|
|нуль  <br/> |Свободна  <br/> |
|1   <br/> |Занят  <br/> |
|2  <br/> |Занята  <br/> |
|4  <br/> |Отсутствие на работе (OOF)  <br/> |
|4   <br/> |Нет данных  <br/> |
   
Например, запрос данных о занятости содержит элемент [TimeWindow](timewindow.md) , который представляет четыре часа и элемент [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) , представляющий 60 минут. Если запрашиваемый календарь пользователя не работает в течение первых 60 минут, он занят в течение следующих 90 минут и незапланированный для конечной 90 минут в окне времени, поток **мержедфрибуси** будет равен 3220. Если интервал содержит более одной классификации доступности, для классификации этого интервала используется самый высокий номер. 
  
Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.
  
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

