---
title: Recurrence (TaskRecurrenceType)
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
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: Элемент повторения содержит данные о повторении для повторяющихся задач.
ms.openlocfilehash: 0ec43447e47050a0bd483d8441da88e4a7f08923
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354423"
---
# <a name="recurrence-taskrecurrencetype"></a>Recurrence (TaskRecurrenceType)

Элемент **повторения** содержит данные о повторении для повторяющихся задач. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <MonthlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRegeneration/> 
       <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRecurrence/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```


**TaskRecurrenceType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительное ежегодный шаблон повторения для повторяющейся задачи.  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |Представляет шаблон повторения ежегодно повторяющейся задачи.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Описывает относительное ежемесячный шаблон повторения для повторяющейся задачи.  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Представляет шаблон повторения ежемесячно для повторяющейся задачи.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Описание частоты в недели и дней, на которых повторения задачи.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Описывает период в днях, в которых повторения задачи.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Описывает через сколько дней после завершения текущей задачи следующее вхождение должны быть выполнены.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Описывает сколько недель после завершения текущей задачи следующее вхождение должны быть выполнены.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Описывает число месяцев после завершения текущей задачи следующее вхождение должны быть выполнены.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Описывает сколько лет после завершения текущей задачи следующее вхождение должны быть выполнены.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Описание шаблона повторения, который не имеет определенный срок.  <br/> Использование этого элемента исключает использование элементов [EndDateRecurrence](enddaterecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Описание, Дата начала и Дата окончания повторения элемента.  <br/> Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .  <br/> [EndDateRecurrence](enddaterecurrence.md) не может использоваться вместе с повторного создания шаблона.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Описание, Дата начала и число вхождений повторяющегося элемента.  <br/> Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [EndDateRecurrence](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
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

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

