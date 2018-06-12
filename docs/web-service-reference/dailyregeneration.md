---
title: DailyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRegeneration
api_type:
- schema
ms.assetid: cafb57e4-c518-45e0-b565-2babd0dab1df
description: Элемент DailyRegeneration описывает период в днях, в которых генерируется задачи.
ms.openlocfilehash: 356f7fd2672b2ad87d17e597c52e9f12273ce3c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761962"
---
# <a name="dailyregeneration"></a>DailyRegeneration

Элемент **DailyRegeneration** описывает период в днях, в которых генерируется задачи. 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

**DailyRegeneratingPatternType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Интервал](interval.md) <br/> |Задает интервал в днях между двумя последовательными повторяющихся элементов. Значение должно быть в диапазоне от 1 до 999.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Повторение (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Содержит данные о повторении для повторяющихся задач.  <br/> |
   
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

