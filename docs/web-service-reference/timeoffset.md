---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: Элемент TimeOffset представляет смещение времени от скоординированного универсального времени (UTC) для перехода часового пояса.
ms.openlocfilehash: ac2da7d6ab1d59d075111390513b1a3dd58a892e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522546"
---
# <a name="timeoffset"></a>TimeOffset

Элемент **TimeOffset представляет** смещение времени от скоординированного универсального времени (UTC) для перехода часового пояса. 
  
```XML
<TimeOffset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часовой пояс, который происходит в определенную дату каждый год.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часовой зоны, который происходит каждый год в один и тот же день.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **TimeOffset** — это продолжительность, которая указывает смещение времени с UTC для перехода часового пояса. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

