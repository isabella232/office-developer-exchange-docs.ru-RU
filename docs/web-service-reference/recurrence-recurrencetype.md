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
description: Элемент периодичности содержит шаблон повторения для элементов календаря и приглашений на собрание.
ms.openlocfilehash: d9c6009e11eb5b66cdd749b8e085935060f99ab7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353352"
---
# <a name="recurrence-recurrencetype"></a>Повторение (RecurrenceType)

Элемент **периодичности** содержит шаблон повторения для элементов календаря и приглашений на собрание. 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
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
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
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
      <RelativeYearlyRecurrence/> 
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
      <DailyRecurrence/> 
      <NoEndRecurrence/>
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
      <DailyRecurrence/> 
      <EndDateRecurrence/>
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
      <DailyRecurrence/> 
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
      <AbsoluteMonthlyRecurrence/> 
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
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
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
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

**RecurrenceType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[релативэйеарлирекурренце](relativeyearlyrecurrence.md) <br/> |Описывает относительный ежегодный шаблон повторения.  <br/> |
|[абсолутэйеарлирекурренце](absoluteyearlyrecurrence.md) <br/> |Представляет шаблон ежегодного повторения.  <br/> |
|[релативемонслирекурренце](relativemonthlyrecurrence.md) <br/> |Описывает относительный месячный шаблон повторения для повторяющегося элемента календаря.  <br/> |
|[абсолутемонслирекурренце](absolutemonthlyrecurrence.md) <br/> |Представляет ежемесячный шаблон повторения.  <br/> |
|[виклирекурренце](weeklyrecurrence.md) <br/> |Описывает частоту в неделях и дни, в которые повторяется элемент или задача календаря.  <br/> |
|[даилирекурренце](dailyrecurrence.md) <br/> |Описывает частоту повторения элемента календаря или задачи в днях.  <br/> |
|[ноендрекурренце](noendrecurrence.md) <br/> |Описывает шаблон повторения, для которого не определена конечная дата.  <br/> Использование этого элемента исключает использование элементов [енддатерекурренце](enddaterecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .  <br/> |
|[енддатерекурренце](enddaterecurrence.md) <br/> |Описывает дату начала и дату окончания расписания повторения элемента.  <br/> Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .  <br/> |
|[нумбередрекурренце](numberedrecurrence.md) <br/> |Описывает дату начала и число повторений повторяющегося элемента.  <br/> Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [енддатерекурренце](enddaterecurrence.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

