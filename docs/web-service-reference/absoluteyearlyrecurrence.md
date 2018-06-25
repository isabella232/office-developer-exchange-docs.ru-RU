---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: Элемент AbsoluteYearlyRecurrence представляет ежегодного шаблона повторения.
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762468"
---
# <a name="absoluteyearlyrecurrence"></a>AbsoluteYearlyRecurrence

Элемент **AbsoluteYearlyRecurrence** представляет ежегодного шаблона повторения. 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 **AbsoluteYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[День месяца](dayofmonth.md) <br/> |Описывает день месяца, на котором происходит повторяющегося элемента. Диапазон значений для этого свойства — от 1 до 31. Если за определенный месяц это значение больше, чем число дней в месяце, последний день месяца используется значение для этого свойства.  <br/> |
|[Месяц (повторение элемента)](month-item-recurrence.md) <br/> |Описывает месяц, в котором ежегодно повторяющегося элемента.  <br/> |
   
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

