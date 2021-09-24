---
title: Transitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: Элемент Transitions представляет массив переходов часового пояса.
ms.openlocfilehash: 7756878ed21bbe778bf51e99ade212f53414f998
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520313"
---
# <a name="transitions"></a>Transitions

Элемент **Transitions** представляет массив переходов часового пояса. 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 **ArrayOfTransitionsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Представляет уникальный идентификатор определения часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Представляет переход часовой пояс, который происходит в определенную дату и в определенное время.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часовой зоны, который происходит каждый год в один и тот же день.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часового пояса, который происходит в указанный день года.  <br/> |
|[Transition](transition.md) <br/> |Представляет переход часовой пояс.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Определяет часовой пояс для времени начала [работы CalendarItem](calendaritem.md) или [MeetingRequest.](meetingrequest.md)  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Определяет часовой пояс для конечного времени [calendarItem](calendaritem.md) или [MeetingRequest.](meetingrequest.md)  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Определяет часовой пояс.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

