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
ms.openlocfilehash: c4a5206c14985ec46cf40162a9ce4eaec68242ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530389"
---
# <a name="notification"></a><span data-ttu-id="49bee-103">Уведомление</span><span class="sxs-lookup"><span data-stu-id="49bee-103">Notification</span></span>

<span data-ttu-id="49bee-104">Элемент **Notification** содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="49bee-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
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

<span data-ttu-id="49bee-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="49bee-105">**NotificationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49bee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49bee-106">Attributes and elements</span></span>

<span data-ttu-id="49bee-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="49bee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49bee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49bee-108">Attributes</span></span>

<span data-ttu-id="49bee-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49bee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49bee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49bee-110">Child elements</span></span>

|<span data-ttu-id="49bee-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49bee-111">**Element**</span></span>|<span data-ttu-id="49bee-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49bee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49bee-113">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="49bee-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="49bee-114">Представляет идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="49bee-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="49bee-115">превиаусватермарк</span><span class="sxs-lookup"><span data-stu-id="49bee-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="49bee-116">Представляет водяной знак последнего события, который был успешно передан клиенту для подписки.</span><span class="sxs-lookup"><span data-stu-id="49bee-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="49bee-117">моривентс</span><span class="sxs-lookup"><span data-stu-id="49bee-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="49bee-118">Указывает, есть ли в очереди больше событий для доставки клиенту.</span><span class="sxs-lookup"><span data-stu-id="49bee-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="49bee-119">копиедевент</span><span class="sxs-lookup"><span data-stu-id="49bee-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="49bee-120">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="49bee-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="49bee-121">креатедевент</span><span class="sxs-lookup"><span data-stu-id="49bee-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="49bee-122">Представляет событие, в котором создается элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="49bee-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="49bee-123">делетедевент</span><span class="sxs-lookup"><span data-stu-id="49bee-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="49bee-124">Представляет событие, в котором удаляется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="49bee-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="49bee-125">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="49bee-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="49bee-126">Представляет событие, в котором изменяется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="49bee-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="49bee-127">моведевент</span><span class="sxs-lookup"><span data-stu-id="49bee-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="49bee-128">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="49bee-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="49bee-129">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="49bee-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="49bee-130">Представляет событие, которое вызывается новым почтовым элементом в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="49bee-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="49bee-131">статусевент</span><span class="sxs-lookup"><span data-stu-id="49bee-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="49bee-132">Представляет уведомление о том, что в почтовом ящике не было новых действий.</span><span class="sxs-lookup"><span data-stu-id="49bee-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="49bee-133">фрибусичанжедевент</span><span class="sxs-lookup"><span data-stu-id="49bee-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="49bee-134">Представляет событие, в котором изменилось свободное и занятое время элемента.</span><span class="sxs-lookup"><span data-stu-id="49bee-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49bee-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49bee-135">Parent elements</span></span>

|<span data-ttu-id="49bee-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49bee-136">**Element**</span></span>|<span data-ttu-id="49bee-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49bee-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49bee-138">жетевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="49bee-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="49bee-139">Содержит состояние и результат запроса на единичные события.</span><span class="sxs-lookup"><span data-stu-id="49bee-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="49bee-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49bee-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="49bee-141">Содержит состояние и результат одного запроса Сенднотификатион.</span><span class="sxs-lookup"><span data-stu-id="49bee-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49bee-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="49bee-142">Text value</span></span>

<span data-ttu-id="49bee-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="49bee-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49bee-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="49bee-144">Remarks</span></span>

<span data-ttu-id="49bee-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="49bee-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49bee-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49bee-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49bee-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49bee-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49bee-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49bee-148">Schema Name</span></span>  <br/> |<span data-ttu-id="49bee-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="49bee-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="49bee-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49bee-150">Validation File</span></span>  <br/> |<span data-ttu-id="49bee-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="49bee-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49bee-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49bee-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="49bee-153">False</span><span class="sxs-lookup"><span data-stu-id="49bee-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49bee-154">См. также</span><span class="sxs-lookup"><span data-stu-id="49bee-154">See also</span></span>

- [<span data-ttu-id="49bee-155">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="49bee-155">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="49bee-156">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="49bee-156">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="49bee-157">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="49bee-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) 
- [<span data-ttu-id="49bee-158">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="49bee-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)

