---
title: Notification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: Элемент уведомление содержит сведения о подписке и события, произошедшие с момента последнего уведомления.
ms.openlocfilehash: 942ec18521fc484a7a3aa1385fb54f480ce9d11f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354353"
---
# <a name="notification"></a>Notification

Элемент **уведомление** содержит сведения о подписке и события, произошедшие с момента последнего уведомления. 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

**NotificationType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Представляет идентификатор для подписки.  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |Представляет водяной знак последнего события, которое было успешно передан клиенту для подписки.  <br/> |
|[MoreEvents](moreevents.md) <br/> |Указывает, есть ли дополнительные события в очереди доставки для клиента.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копирование элемента или папки.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, в котором создается элемента или папки.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, в котором удаляется элемент или папку.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, в котором изменения элемента или папки.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, которое инициируется нового элемента почты в почтовом ящике.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Представляет уведомление о том, что не новые действия в почтовом ящике.  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |Представляет событие, в котором был изменен занятости элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendNotification.  <br/> |
   
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

- [Операции подписки](subscribe-operation.md) 
- [Операция GetEvents](getevents-operation.md) 
- [Операция GetStreamingEvents](getstreamingevents-operation.md) 
- [Отписаться операции](unsubscribe-operation.md)

