---
title: абсолутэйеарлирекурренце
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
description: Элемент Абсолутэйеарлирекурренце представляет шаблон ежегодного повторения.
ms.openlocfilehash: 19b617dfd5c0a3d206d62439c880da084fd5f5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460416"
---
# <a name="absoluteyearlyrecurrence"></a>абсолутэйеарлирекурренце

Элемент **абсолутэйеарлирекурренце** представляет шаблон ежегодного повторения. 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 **абсолутэйеарлирекурренцепаттернтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DayOfMonth](dayofmonth.md) <br/> |Описывает день месяца, в который происходит повторяющийся элемент. Диапазон значений этого свойства — от 1 до 31. Если для определенного месяца это значение превышает количество дней в месяце, для этого свойства подразумевается последний день месяца.  <br/> |
|[Month (повторение элемента)](month-item-recurrence.md) <br/> |Описывает месяц, в который происходит ежегодно повторяющийся элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Повторение (Таскрекурренцетипе)](recurrence-taskrecurrencetype.md) <br/> |Содержит сведения о повторении для повторяющихся задач.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашений на собрание.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

