---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: Элемент DaysOfWeek описывает дни недели, используемые в расписаниях повторов элемента.
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762003"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

Элемент **DaysOfWeek** описывает дни недели, используемые в расписаниях повторов элемента. 
  
```XML
<DaysOfWeek/>
```

**DaysOfWeekType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Описание еженедельно повторяющейся.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Ниже перечислены возможные значения.
  
- Воскресенье    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота    
- День (это значение является недопустимым для шаблона повторения Еженедельно)    
- День недели (это значение является недопустимым для шаблона повторения Еженедельно)    
- WeekendDay (это значение является недопустимым для шаблона повторения Еженедельно)
    
Еженедельно повторяющейся может содержать несколько значений. Значений, разделенных пробел. Например еженедельного повторения по вторникам и четвергам текстовое значение будет «Вторник четверг».
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

