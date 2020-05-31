---
title: Уведомление
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
description: Элемент Notification содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.
ms.openlocfilehash: 942ec18521fc484a7a3aa1385fb54f480ce9d11f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354353"
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SubscriptionId (Events)](subscriptionid-getevents.md) <br/> |Представляет идентификатор подписки.  <br/> |
|[превиаусватермарк](previouswatermark.md) <br/> |Представляет водяной знак последнего события, который был успешно передан клиенту для подписки.  <br/> |
|[моривентс](moreevents.md) <br/> |Указывает, есть ли в очереди больше событий для доставки клиенту.  <br/> |
|[копиедевент](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[креатедевент](createdevent.md) <br/> |Представляет событие, в котором создается элемент или папка.  <br/> |
|[делетедевент](deletedevent.md) <br/> |Представляет событие, в котором удаляется элемент или папка.  <br/> |
|[модифиедевент](modifiedevent.md) <br/> |Представляет событие, в котором изменяется элемент или папка.  <br/> |
|[моведевент](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.  <br/> |
|[невмаилевент](newmailevent.md) <br/> |Представляет событие, которое вызывается новым почтовым элементом в почтовом ящике.  <br/> |
|[статусевент](statusevent.md) <br/> |Представляет уведомление о том, что в почтовом ящике не было новых действий.  <br/> |
|[фрибусичанжедевент](freebusychangedevent.md) <br/> |Представляет событие, в котором изменилось свободное и занятое время элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетевентсреспонсемессаже](geteventsresponsemessage.md) <br/> |Содержит состояние и результат запроса на единичные события.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Содержит состояние и результат одного запроса Сенднотификатион.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операции подписки](subscribe-operation.md) 
- [Операция GetEvents](getevents-operation.md) 
- [Операция GetStreamingEvents](getstreamingevents-operation.md) 
- [Операция по отмене подписки](unsubscribe-operation.md)

