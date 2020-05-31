---
title: Себя (Реминдерактионтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: Элемент действия указывает действие, выполняемое с напоминанием.
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761327"
---
# <a name="actiontype-reminderactiontype"></a>Себя (Реминдерактионтипе)

Элемент **действия** указывает действие, выполняемое с напоминанием. 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **реминдерактионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[реминдеритемактион](reminderitemaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое **значение элемента действия** указывает действие, выполняемое с напоминанием. Текстовое значение **отклонения** указывает, что напоминание должно быть закрыто. Текстовое значение **откладывания** указывает на то, что напоминание должно быть задержано до момента времени, указанного в элементе [невреминдертиме](newremindertime.md) . 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [реминдеритемактион](reminderitemaction.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

