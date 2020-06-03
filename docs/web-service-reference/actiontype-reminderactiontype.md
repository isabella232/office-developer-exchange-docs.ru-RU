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
ms.openlocfilehash: 5c62b2dd945b23a5ff2bb824385c45dbc617a5a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465060"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [реминдеритемактион](reminderitemaction.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

