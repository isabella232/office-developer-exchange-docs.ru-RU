---
title: виклирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: Элемент Виклирекурренце описывает еженедельный шаблон повторения.
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530368"
---
# <a name="weeklyrecurrence"></a>виклирекурренце

Элемент **виклирекурренце** описывает еженедельный шаблон повторения. 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 **виклирекурренцепаттернтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Interval](interval.md) <br/> |Определяет интервал (в неделях) между двумя последовательными еженедельными элементами расписания повторения. Значение может находиться в диапазоне от 1 до 99.  <br/> |
|[DaysOfWeek (Дайсофвиктипе)](daysofweek-daysofweektype.md) <br/> |Описывает дни недели в расписании повторения.  <br/> |
|[FirstDayOfWeek](firstdayofweek.md) <br/> |Указывает первый день недели.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Повторение (Таскрекурренцетипе)](recurrence-taskrecurrencetype.md) <br/> |Содержит сведения о повторении для повторяющихся задач.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашений на собрание.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Сведения о смещении часового пояса теряются, если даты [начала](start.md) и [окончания](end-ex15websvcsotherref.md) повторяющегося элемента шаблона не имеют даты, равной первому появлению еженедельного расписания повторения. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

