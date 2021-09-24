---
title: Уведомление
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: Элемент Notification содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.
ms.openlocfilehash: affd44bb4c1f16029d6da92419908aeac3c26a44
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515413"
---
# <a name="notification"></a>Уведомление

Элемент **Notification** содержит сведения о подписке и событиях, произошедших с момента последнего уведомления. 
  
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
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Представляет идентификатор подписки.  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |Представляет водяной знак последнего события, которое было успешно доведено до клиента для подписки.  <br/> |
|[MoreEvents](moreevents.md) <br/> |Указывает, есть ли в очереди больше событий, которые будут доставлены клиенту.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, в котором создается элемент или папка.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, в котором элемент или папка удаляются.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, в котором элемент или папка изменены.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую родительную.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, которое запускается новым элементом почты в почтовом ящике.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Представляет уведомление о том, что в почтовом ящике не было никаких новых действий.  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |Представляет событие, в котором время свободного и загруженного элемента изменилось.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса SendNotification.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

- [Операции подписки](subscribe-operation.md) 
- [Операция GetEvents](getevents-operation.md) 
- [Операция GetStreamingEvents](getstreamingevents-operation.md) 
- [Операция Unsubscribe](unsubscribe-operation.md)

