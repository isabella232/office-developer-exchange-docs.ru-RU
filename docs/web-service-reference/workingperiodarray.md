---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: Элемент WorkingPeriodArray содержит работа периода сведения для пользователя почтового ящика.
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840531"
---
# <a name="workingperiodarray"></a>WorkingPeriodArray

Элемент **WorkingPeriodArray** содержит работа периода сведения для пользователя почтового ящика. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[WorkingHours](workinghours-ex15websvcsotherref.md)
  
[WorkingPeriodArray](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 **ArrayOfWorkingPeriod**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Содержит рабочей недели, дни и часы пользователя почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является обязательным, если используется элемент [WorkingHours](workinghours-ex15websvcsotherref.md) . Все дочерние элементы, перечислены в последовательности, в котором они изложены. 
  
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
