---
title: WorkingHours
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: Элемент WorkingHours представляет параметры часовой зоны и рабочие часы для запрашиваемой пользователя почтовых ящиков.
ms.openlocfilehash: 6453ddbf3d1bf96ce09073ff62a65bd5a6ccc515
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525500"
---
# <a name="workinghours"></a>WorkingHours

Элемент **WorkingHours** представляет параметры часовой зоны и рабочие часы для запрашиваемой пользователя почтовых ящиков. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[WorkingHours](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 **WorkingHours**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZone (доступность)](timezone-availability.md) <br/> |Содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе между стандартным временем и летнее время. Этот элемент необходим, если используется элемент **WorkingHours.**  <br/> |
|[WorkingPeriodArray](workingperiodarray.md) <br/> |Содержит сведения о рабочем периоде для пользователя почтового ящика. Этот элемент необходим, если используется элемент **WorkingHours.**  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |Содержит сведения о доступности для определенного пользователя.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
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

