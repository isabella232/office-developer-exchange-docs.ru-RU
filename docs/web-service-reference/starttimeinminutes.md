---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: Элемент StartTimeInMinutes представляет начала рабочего дня для пользователя почтового ящика.
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835558"
---
# <a name="starttimeinminutes"></a>StartTimeInMinutes

Элемент **StartTimeInMinutes** представляет начала рабочего дня для пользователя почтового ящика. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [FreeBusyResponseArray](freebusyresponsearray.md)
  
- [FreeBusyResponse](freebusyresponse.md)
  
- [FreeBusyView](freebusyview.md)
  
- [WorkingHours](workinghours-ex15websvcsotherref.md)
  
- [WorkingPeriodArray](workingperiodarray.md)
  
- [WorkingPeriod](workingperiod.md)
  
- [StartTimeInMinutes](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Содержит рабочей недели, дни и часы пользователя почтового ящика.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет начала рабочего дня, сколько минут, прошедшее с момента начала дня. Например время начала 8: 00 представлены 480 минут.
  
Диапазон допустимых значений для этого элемента — 0 до 1440.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
