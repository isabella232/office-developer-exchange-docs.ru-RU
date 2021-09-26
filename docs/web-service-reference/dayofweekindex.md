---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: Элемент DayOfWeekIndex описывает, какая неделя в месяц используется в относительном шаблоне повторения.
ms.openlocfilehash: 3b9af396bbd5c51b365da6a95b40b00718d47c3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542521"
---
# <a name="dayofweekindex"></a>DayOfWeekIndex

Элемент **DayOfWeekIndex** описывает, какая неделя в месяц используется в относительном шаблоне повторения. 
  
```xml
<DayOfWeekIndex/>
```

**DayOfWeekIndexType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительное ежегодное повторение.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Описывает относительную ежемесячную схему повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ниже перечислены возможные значения.
  
- Первый    
- Секунды    
- Третий    
- Четвертый    
- Последнее
    
## <a name="remarks"></a>Заметки

Например, второй понедельник месяца может произойти в третью неделю этого месяца. Если месяц начинается в пятницу, первая неделя месяца содержит только несколько дней и не содержит понедельника. Поэтому первый понедельник должен произойти во вторую неделю.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

