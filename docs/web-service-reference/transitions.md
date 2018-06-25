---
title: Переходы между
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: Переходы между элемент представляет массив переходы часового пояса.
ms.openlocfilehash: df7cacdef71c3fdfaa3ecadb486843ea30e6109d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840235"
---
# <a name="transitions"></a>Переходы между

**Переходы между** элемент представляет массив переходы часового пояса. 
  
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
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Представляет переход часовой пояс, который создается в конкретный день и в определенное время.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часового пояса, что происходит в тот же день каждый год.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часового пояса, что происходит на указанном дня года.  <br/> |
|[Переход](transition.md) <br/> |Представляет переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Определяет часовой пояс для времени начала [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Определяет часовой пояс для время окончания [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).  <br/> |
|[Определение часового пояса](timezonedefinition.md) <br/> |Определяет часовой пояс.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

