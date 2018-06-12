---
title: Интервал
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: Элемент интервал определяет интервал между двумя последовательными повторяющихся элементов.
ms.openlocfilehash: 55d26b5b1b51aca3effa93a2e6852c1ae57ef4b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833962"
---
# <a name="interval"></a>Интервал

Элемент **интервал** определяет интервал между двумя последовательными повторяющихся элементов. 
  
```xml
<Interval/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |Представляет шаблон повторения ежемесячно.  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |Описывает период в днях, в которых генерируется задачи.  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |Описывает период в днях, в которых повторения задачи.  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |Описание частоты, месяца, в которых генерируется задачи.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Описывает относительное ежемесячный шаблон для повторяющейся задачи.  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Описание частоты в недель, в котором и дней, на которых повторения задачи.  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |Описание частоты, недель, в которых генерируется задачи.  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |Описание частоты, годы, в которых генерируется задачи.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее целое число является обязательным.
  
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

