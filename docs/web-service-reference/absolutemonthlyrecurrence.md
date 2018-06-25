---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: Элемент AbsoluteMonthlyRecurrence представляет ежемесячный шаблона повторения.
ms.openlocfilehash: f4613fa71a9164c45b60a82f675959817cd4bdd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762473"
---
# <a name="absolutemonthlyrecurrence"></a>AbsoluteMonthlyRecurrence

Элемент **AbsoluteMonthlyRecurrence** представляет ежемесячный шаблона повторения. 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 **AbsoluteMonthlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[День месяца](dayofmonth.md) <br/> |Описывает день месяца, которая происходит повторяющегося элемента. Диапазон значений для этого свойства — от 1 до 31. Если за определенный месяц это значение больше, чем число дней в месяце, последний день месяца используется значение для этого свойства.  <br/> |
|[Интервал](interval.md) <br/> |Задает интервал между двумя последовательными повторяющихся элементов. Например если элемент **интервал** имеет значение 5, повторяющегося элемента происходит каждые 5 месяцев. Диапазон допустимых значений — от 1 до 99.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Повторение (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Содержит данные о повторении для повторяющихся задач.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашения на собрания.  <br/> |
   
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

