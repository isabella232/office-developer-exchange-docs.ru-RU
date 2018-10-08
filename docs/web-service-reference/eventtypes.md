---
title: EventTypes
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
description: Элемент EventTypes содержит коллекцию типов событий уведомлений, которые используются для создания подписки.
ms.openlocfilehash: 7ea783dc0bf73abf992616b1f86c7621c5b36fc8
ms.sourcegitcommit: 25cbbc6707e4ec0621c5c46baf7fe49be42d3297
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2018
ms.locfileid: "25440839"
---
# <a name="eventtypes"></a>EventTypes

Элемент **EventTypes** содержит коллекцию типов событий уведомлений, которые используются для создания подписки. 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 **NonEmptyArrayOfNotificationEventTypesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EventType](eventtype.md) <br/> |Представляет тип уведомлений запрошенные событий, который используется для создания подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о принудительной события.  <br/> |
|[StreamingSubscriptionRequest](streamingsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о потоковой передачи событий.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция GetStreamingEvents](getstreamingevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)

