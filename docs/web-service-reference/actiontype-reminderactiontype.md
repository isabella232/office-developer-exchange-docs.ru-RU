---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: Элемент ActionType указывает действие, необходимое для напоминания.
ms.openlocfilehash: d78725c75ad13a71d69d7749f0a71cd99d606929
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522259"
---
# <a name="actiontype-reminderactiontype"></a>ActionType (ReminderActionType)

Элемент **ActionType** указывает действие, необходимое для напоминания. 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **ActionType** указывает действие, необходимое для напоминания. Текстовое значение **Dismiss** указывает, что напоминание должно быть отклонено. Текстовое значение **Snooze** указывает, что напоминание следует отложить до времени, указанного [элементом NewReminderTime.](newremindertime.md) 
  
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

- [ReminderItemAction](reminderitemaction.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

