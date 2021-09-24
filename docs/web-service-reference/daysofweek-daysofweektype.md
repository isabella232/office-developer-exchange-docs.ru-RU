---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: Элемент DaysOfWeek описывает дни недели, используемые в шаблонах повторения элементов.
ms.openlocfilehash: 9b0786149f943c47ab77bcb69b74542cbc08edd5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519872"
---
# <a name="daysofweek-daysofweektype"></a>DaysOfWeek (DaysOfWeekType)

Элемент **DaysOfWeek** описывает дни недели, используемые в шаблонах повторения элементов. 
  
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
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |Описывает недельный шаблон повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ниже перечислены возможные значения.
  
- Воскресенье    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота    
- Day (это значение не допустимо для еженедельного шаблона повторения)    
- Будний день (это значение не допустимо для еженедельного шаблона повторения)    
- WeekendDay (это значение не допустимо для еженедельного шаблона повторения)
    
Недельный шаблон повторения может содержать несколько значений. Значения разделены пробелом. Например, для еженедельного повторения по вторникам и четвергам текстовое значение будет "вторник четверг".
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

