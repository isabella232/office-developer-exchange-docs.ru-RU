---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: Элемент AppointmentState указывает состояние встречи.
ms.openlocfilehash: f984bbd5a1319a6051a3394ed04d56deabbb2c5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544284"
---
# <a name="appointmentstate"></a>AppointmentState

Элемент **AppointmentState** указывает состояние встречи. 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент содержит текстовое значение, которое представляет набор битов. Это в форме integer. Этот элемент доступен только для чтения. Он будет возвращен только в ответе.
  
## <a name="remarks"></a>Заметки

Возвращаемая сумма представляет битмаску состояния назначения. В следующей таблице описывается каждый бит.
  
|**Имя**|**Bit**|**Описание**|
|:-----|:-----|:-----|
|Нет  <br/> |0x0000  <br/> |Флаги не установлены. Это используется только для встречи, в которую не входят участники.  <br/> |
|Собрание  <br/> |0x0001  <br/> |Это собрание.  <br/> |
|ПОЛУЧЕНО  <br/> |0x0002  <br/> |Это назначение получено.  <br/> |
|Canceled.  <br/> |0x0004  <br/> |Это назначение отменено.  <br/> |
   
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

