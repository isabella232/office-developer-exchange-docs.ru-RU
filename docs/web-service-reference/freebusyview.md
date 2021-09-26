---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: Элемент FreeBusyView содержит сведения о доступности для определенного пользователя.
ms.openlocfilehash: c662e8a44118f61b4c8be642d9ac862051c3a15d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546415"
---
# <a name="freebusyview"></a>FreeBusyView

Элемент **FreeBusyView** содержит сведения о доступности для определенного пользователя. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 **FreeBusyView**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |Представляет тип запрашиваемой бесплатной или занятой информации, возвращаемой в ответе.  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |Содержит объединенный свободный и загруженный поток данных.  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |Содержит набор уникальных событий элементов календаря, которые представляют доступность запрашиваемого пользователя.  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часовой зоны и рабочие часы для запрашиваемой пользователя почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Содержит сведения о бесплатном/загружении для одного пользователя почтового ящика.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>Заметки

Все элементы ребенка перечислены в последовательности, в которой они происходят. Уровень детализации, предоставляемой этим элементом, зависит от разрешений, предоставленных запросчику.
  
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

