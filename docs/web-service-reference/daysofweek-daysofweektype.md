---
title: DaysOfWeek (Дайсофвиктипе)
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
description: Элемент DaysOfWeek описывает дни недели, которые используются в шаблонах повторения элементов.
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762003"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (Дайсофвиктипе)

Элемент **DaysOfWeek** описывает дни недели, которые используются в шаблонах повторения элементов. 
  
```XML
<DaysOfWeek/>
```

**дайсофвиктипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[виклирекурренце](weeklyrecurrence.md) <br/> |Описывает еженедельный шаблон повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже перечислены возможные значения.
  
- Воскресеньям    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота    
- Day (это значение не является допустимым для еженедельного расписания повторения)    
- Weekday (это значение не является допустимым для расписания повторения)    
- Викенддай (это значение не является допустимым для еженедельного расписания повторения)
    
Еженедельный шаблон повторения может содержать несколько значений. Значения разделяются символом пробела. Например, для еженедельного повторения в вторникам и четверг, текстовое значение будет "Вторник четверг".
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

