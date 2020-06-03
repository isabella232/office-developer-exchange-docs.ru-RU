---
title: коннектионфаилурекаусе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: Элемент Коннектионфаилурекаусе указывает причину отключения от телефонного звонка.
ms.openlocfilehash: 6385641eaee140a114906703232974d51d5ce344
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529450"
---
# <a name="connectionfailurecause"></a>коннектионфаилурекаусе

Элемент **коннектионфаилурекаусе** указывает причину отключения от телефонного звонка. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **коннектионфаилурекаусетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фонекаллинформатион](phonecallinformation.md) <br/> |Задает сведения о состоянии телефонного звонка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **коннектионфаилурекаусе** . 
  
**Значения элементов Коннектионфаилурекаусе**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Состояние вызова не отключено или причина отключения неизвестна.  <br/> |
|усербуси  <br/> |Линия вызываемой стороны занята.  <br/> |
|Ответ  <br/> |Вызываемая сторона не ответила.  <br/> |
|Выходе  <br/> |Номер вызываемого абонента был недоступен.  <br/> |
|Другое  <br/> |Перехватить все для других причин отключения.  <br/> |
   
## <a name="remarks"></a>Примечания

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

