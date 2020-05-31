---
title: релативэйеарлирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: Элемент Релативэйеарлирекурренце описывает относительный ежегодный шаблон повторения.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835057"
---
# <a name="relativeyearlyrecurrence"></a>релативэйеарлирекурренце

Элемент **релативэйеарлирекурренце** описывает относительный ежегодный шаблон повторения. 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 **релативэйеарлирекурренцепаттернтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DaysOfWeek (Дайофвиктипе)](daysofweek-dayofweektype.md) <br/> |Описывает дни недели, которые используются в шаблонах повторения элементов.  <br/> |
|[дайофвикиндекс](dayofweekindex.md) <br/> |Описывает, какая неделя месяца используется в качестве относительного ежегодного повторения.  <br/> |
|[Month (повторение элемента)](month-item-recurrence.md) <br/> |Описывает месяц, когда происходит ежегодно повторяющийся элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Повторение (Таскрекурренцетипе)](recurrence-taskrecurrencetype.md) <br/> |Содержит сведения о повторении для повторяющихся задач.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашений на собрание.  <br/> |
|[Standard](standard.md) <br/> |Представляет дату и время изменения времени с летнего на стандартное время.  <br/> |
|[Переход](daylight.md) <br/> |Представляет дату и время изменения времени со стандартного времени на летнее.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

