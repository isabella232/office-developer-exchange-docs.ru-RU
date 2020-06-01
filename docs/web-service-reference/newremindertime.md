---
title: невреминдертиме
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: Элемент Невреминдертиме указывает новое время напоминания.
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465956"
---
# <a name="newremindertime"></a>невреминдертиме

Элемент **невреминдертиме** указывает новое время напоминания. 
  
```XML
<NewReminderTime/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[реминдеритемактион](reminderitemaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **невреминдертиме** — новое время напоминания. Элемент **невреминдертиме** используется, [когда элемент "](actiontype-reminderactiontype.md) элемент" имеет значение **отсрочки**, чтобы отложить напоминание. Значение Невреминдертиме должно быть больше, чем [ReminderTime](remindertime.md) , возвращенное [операцией](getreminders-operation.md) **NewReminderTime** .
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[реминдеритемактион](reminderitemaction.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

