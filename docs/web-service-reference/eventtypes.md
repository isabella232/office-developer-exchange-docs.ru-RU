---
title: евенттипес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: Элемент Евенттипес содержит коллекцию типов уведомлений о событиях, которые используются для создания подписки.
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530630"
---
# <a name="eventtypes"></a>евенттипес

Элемент **евенттипес** содержит коллекцию типов уведомлений о событиях, которые используются для создания подписки. 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 **нонемптяррайофнотификатионевенттипестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EventType](eventtype.md) <br/> |Представляет запрошенный тип уведомления о событии, который используется для создания подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[пуллсубскриптионрекуест](pullsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях по запросу.  <br/> |
|[пушсубскриптионрекуест](pushsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.  <br/> |
|[стреамингсубскриптионрекуест](streamingsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях потоковой передачи.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция GetStreamingEvents](getstreamingevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

