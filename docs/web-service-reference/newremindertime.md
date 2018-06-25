---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: Элемент NewReminderTime Указывает новое время для напоминания.
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834531"
---
# <a name="newremindertime"></a>NewReminderTime

Элемент **NewReminderTime** Указывает новое время для напоминания. 
  
```XML
<NewReminderTime/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **NewReminderTime** — это новое время оповещения. Элемент **NewReminderTime** будет использоваться при элемент [Тип действия](actiontype-reminderactiontype.md) задано значение **отложить**, чтобы задержки напоминания. Значение **NewReminderTime** должно быть больше, чем [ReminderTime](remindertime.md) , возвращенные [операцией GetReminders](getreminders-operation.md).
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[ReminderItemAction](reminderitemaction.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

