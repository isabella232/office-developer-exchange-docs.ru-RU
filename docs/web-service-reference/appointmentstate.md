---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: Элемент AppointmentState указывает состояние встречи.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761480"
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
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент содержит значение текста, что представляет значение бит. Это в форме целое число. Этот элемент доступен только для чтения. Он только будет возвращен в ответе.
  
## <a name="remarks"></a>Замечания

Целое значение, которое возвращается представляет битовую маску состояние встречи. В следующей таблице описываются каждый бит.
  
|**Имя**|**Бит**|**Описание**|
|:-----|:-----|:-----|
|Нет  <br/> |0x0000  <br/> |Флаги не были установлены. Используется только для встречи, которая не включает участников.  <br/> |
|Собрание  <br/> |0x0001  <br/> |В этом встреча является собранием.  <br/> |
|Получено  <br/> |0x0002  <br/> |В этом встречи был получен.  <br/> |
|Canceled.  <br/> |0x0004  <br/> |В этом встречи было отменено.  <br/> |
   
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

