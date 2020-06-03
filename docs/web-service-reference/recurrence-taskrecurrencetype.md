---
title: Повторение (Таскрекурренцетипе)
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
description: Элемент периодичности содержит сведения о повторении для повторяющихся задач.
ms.openlocfilehash: 933fd6b003d8d193e1561f2a22b65ac00237c345
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528834"
---
# <a name="recurrence-taskrecurrencetype"></a>Повторение (Таскрекурренцетипе)

Элемент **периодичности** содержит сведения о повторении для повторяющихся задач. 
  
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


**таскрекурренцетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[релативэйеарлирекурренце](relativeyearlyrecurrence.md) <br/> |Описывает относительный ежегодный шаблон повторения для повторяющейся задачи.  <br/> |
|[абсолутэйеарлирекурренце](absoluteyearlyrecurrence.md) <br/> |Представляет шаблон ежегодного повторения для повторяющейся задачи.  <br/> |
|[релативемонслирекурренце](relativemonthlyrecurrence.md) <br/> |Описывает относительный месячный шаблон повторения для повторяющейся задачи.  <br/> |
|[абсолутемонслирекурренце](absolutemonthlyrecurrence.md) <br/> |Представляет ежемесячный шаблон повторения для повторяющейся задачи.  <br/> |
|[виклирекурренце](weeklyrecurrence.md) <br/> |Описывает частоту в неделях и дни, в которые задача повторяется.  <br/> |
|[даилирекурренце](dailyrecurrence.md) <br/> |Описывает частоту повторения задачи в днях.  <br/> |
|[даилиреженератион](dailyregeneration.md) <br/> |Содержит сведения о том, сколько дней после завершения текущей задачи будет связано со следующим экземпляром.  <br/> |
|[виклиреженератион](weeklyregeneration.md) <br/> |Показывает, сколько недель после завершения текущей задачи будет связано со следующим экземпляром.  <br/> |
|[монслиреженератион](monthlyregeneration.md) <br/> |Содержит сведения о том, сколько месяцев после завершения текущей задачи будет связано со следующим экземпляром.  <br/> |
|[еарлиреженератион](yearlyregeneration.md) <br/> |Описывает, сколько лет после завершения текущей задачи будет выполняться следующее.  <br/> |
|[ноендрекурренце](noendrecurrence.md) <br/> |Описывает шаблон повторения, для которого не определена конечная дата.  <br/> Использование этого элемента исключает использование элементов [енддатерекурренце](enddaterecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .  <br/> |
|[енддатерекурренце](enddaterecurrence.md) <br/> |Описывает дату начала и дату окончания расписания повторения элемента.  <br/> Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .  <br/> [Енддатерекурренце](enddaterecurrence.md) нельзя использовать вместе с шаблоном повторного создания.  <br/> |
|[нумбередрекурренце](numberedrecurrence.md) <br/> |Описывает дату начала и число повторений повторяющегося элемента.  <br/> Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [енддатерекурренце](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

