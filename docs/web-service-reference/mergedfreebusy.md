---
title: MergedFreeBusy
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
description: Элемент MergedFreeBusy содержит объединенные занятости поток данных.
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834449"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

Элемент **MergedFreeBusy** содержит объединенные занятости поток данных. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **string**
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

Сервер предоставляет текстовое значение, если значение для элемента [FreeBusyViewType](freebusyviewtype.md) — это один из следующих: 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
Текстовое значение представляет собой поток сведений о доступности. 
  
## <a name="remarks"></a>Замечания

Поток данных, представленные в этом элементе определяется элементов [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) и [значение TimeWindow](timewindow.md) . Элемент [значение TimeWindow](timewindow.md) определяет период времени, запрос для обеспечения доступности. Элемент [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) определяет, как время из элемента [значение TimeWindow](timewindow.md) разбивается на интервалы, возвращаемых в элементе **MergedFreeBusy** . Каждый номер в потоке **MergedFreeBusy** представляет один интервал, определенные в элементе [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) . В следующей таблице перечислены возможные значения для отдельных интервала. 
  
|**Цифры**|**Доступность**|
|:-----|:-----|
|0  <br/> |Свободна  <br/> |
|1  <br/> |Под вопросом  <br/> |
|2  <br/> |Занята  <br/> |
|3  <br/> |Нет на месте (OOF)  <br/> |
|4  <br/> |Нет данных  <br/> |
   
Например запрос на данные о доступности включает в себя элемент [значение TimeWindow](timewindow.md) , представляющий четырех часов и [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) элемент, представляющий 60 минут. Если календарь запрошенного пользователя об отсутствии на работе для первого 60 минут, «занят» для следующих 90 минут и незапланированной для окончательного 90 минут в окне времени в потоке **MergedFreeBusy** будет 3220. Если интервал содержит более одного классификации доступности, самое большое число используется для классификации этого интервала. 
  
Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.
  
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

