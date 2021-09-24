---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: Элемент NewReminderTime указывает новое время напоминания.
ms.openlocfilehash: 9e6cb75396f35f606bcd974e374f24957ee5d1ec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515448"
---
# <a name="newremindertime"></a>NewReminderTime

Элемент **NewReminderTime** указывает новое время напоминания. 
  
```XML
<NewReminderTime/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **NewReminderTime** — это новое время для напоминания. Элемент **NewReminderTime** используется, когда элемент [ActionType](actiontype-reminderactiontype.md) настроен на **Snooze,** чтобы отложить напоминание. Значение **NewReminderTime** должно быть больше, чем значение [ReminderTime,](remindertime.md) возвращенного операцией [GetReminders.](getreminders-operation.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[ReminderItemAction](reminderitemaction.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

