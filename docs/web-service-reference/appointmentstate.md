---
title: аппоинтментстате
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
description: Элемент Аппоинтментстате указывает состояние встречи.
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463477"
---
# <a name="appointmentstate"></a>аппоинтментстате

Элемент **аппоинтментстате** указывает состояние встречи. 
  
```XML
<AppointmentState/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент содержит текстовое значение, представляющее набор битов. Это в виде целого числа. Этот элемент доступен только для чтения. Он будет возвращен только в ответе.
  
## <a name="remarks"></a>Примечания

Возвращаемое целое значение представляет битовую маску состояния встречи. В приведенной ниже таблице описывается каждый из этих бит.
  
|**имя**|**Битовая**|**Описание**|
|:-----|:-----|:-----|
|Нет  <br/> |0x0000  <br/> |Флаги не заданы. Используется только для встречи, не включающей участников.  <br/> |
|Назначить  <br/> |0x0001  <br/> |Эта встреча является собранием.  <br/> |
|ПОЛУЧЕНО  <br/> |0x0002  <br/> |Эта встреча получена.  <br/> |
|Canceled.  <br/> |0x0004  <br/> |Эта встреча отменена.  <br/> |
   
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

