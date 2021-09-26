---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: Элемент StartTimeInMinutes представляет начало рабочего дня для пользователя почтового ящика.
ms.openlocfilehash: 0d6d5d89506a081814a0f5143bdc7809a0ca3520
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544649"
---
# <a name="starttimeinminutes"></a>StartTimeInMinutes

Элемент **StartTimeInMinutes** представляет начало рабочего дня для пользователя почтового ящика. 
  
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
|[WorkingPeriod](workingperiod.md) <br/> |Содержит дни и часы работы пользователя почтового ящика.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет начало рабочего дня по времени с момента начала рабочего дня. Например, время начала в 8 утра. представляет 480 минут.
  
Диапазон возможных значений для этого элемента — от 0 до 1440.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

