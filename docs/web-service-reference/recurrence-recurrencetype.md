---
title: Повторение (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: Элемент повторения содержит шаблон повторения для элементов календаря и приглашения на собрания.
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835004"
---
# <a name="recurrence-recurrencetype"></a>Повторение (RecurrenceType)

Элемент **повторения** содержит шаблон повторения для элементов календаря и приглашения на собрания. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 **RecurrenceType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительное ежегодно повторяющейся.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Представляет шаблон повторения ежегодно.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Описывает относительное ежемесячный шаблона повторения повторяющегося элемента календаря.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Представляет шаблон повторения ежемесячно.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Описание частоты недели и дней, элемента календаря или задача повторяется.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Описывает период в днях, в котором повторяется элемента календаря или задач.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Описание шаблона повторения, который не имеет определенный срок.  <br/> Использование этого элемента исключает использование элементов [EndDateRecurrence](enddaterecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Описание, Дата начала и Дата окончания повторения элемента.  <br/> Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Описание, Дата начала и число вхождений повторяющегося элемента.  <br/> Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашения на собрание в хранилище Exchange  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

