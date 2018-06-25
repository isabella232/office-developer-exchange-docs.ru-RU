---
title: Уведомления
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
ms.openlocfilehash: a769d8988eb68d0fa0b02f3838cd891e714571b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834547"
---
# <a name="notification"></a><span data-ttu-id="d8c8f-103">Уведомления</span><span class="sxs-lookup"><span data-stu-id="d8c8f-103">Notification</span></span>

<span data-ttu-id="d8c8f-104">Элемент **уведомление** содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

 <span data-ttu-id="d8c8f-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="d8c8f-105">**NotificationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8c8f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8c8f-106">Attributes and elements</span></span>

<span data-ttu-id="d8c8f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8c8f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8c8f-108">Attributes</span></span>

<span data-ttu-id="d8c8f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8c8f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8c8f-110">Child elements</span></span>

|<span data-ttu-id="d8c8f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8c8f-111">**Element**</span></span>|<span data-ttu-id="d8c8f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8c8f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c8f-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="d8c8f-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="d8c8f-114">Представляет идентификатор для подписки.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="d8c8f-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="d8c8f-116">Представляет водяной знак последнего события, которое было успешно передан клиенту для подписки.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-117">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="d8c8f-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="d8c8f-118">Указывает, есть ли дополнительные события в очереди доставки для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d8c8f-120">Представляет событие, в котором копирование элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="d8c8f-122">Представляет событие, в котором создается элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="d8c8f-124">Представляет событие, в котором удаляется элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-125">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d8c8f-126">Представляет событие, в котором изменения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d8c8f-128">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="d8c8f-130">Представляет событие, которое инициируется нового элемента почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="d8c8f-132">Представляет уведомление о том, что не новые действия в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="d8c8f-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="d8c8f-134">Представляет событие, в котором был изменен занятости элемента.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8c8f-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8c8f-135">Parent elements</span></span>

|<span data-ttu-id="d8c8f-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8c8f-136">**Element**</span></span>|<span data-ttu-id="d8c8f-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8c8f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c8f-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d8c8f-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="d8c8f-139">Содержит состояние и результат одного запроса GetEvents.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="d8c8f-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d8c8f-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="d8c8f-141">Содержит состояние и результат одного запроса SendNotification.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8c8f-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d8c8f-142">Text value</span></span>

<span data-ttu-id="d8c8f-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8c8f-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="d8c8f-144">Remarks</span></span>

<span data-ttu-id="d8c8f-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8c8f-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8c8f-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8c8f-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8c8f-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8c8f-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8c8f-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8c8f-148">Schema Name</span></span>  <br/> |<span data-ttu-id="d8c8f-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d8c8f-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8c8f-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8c8f-150">Validation File</span></span>  <br/> |<span data-ttu-id="d8c8f-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8c8f-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8c8f-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8c8f-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8c8f-153">False</span><span class="sxs-lookup"><span data-stu-id="d8c8f-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8c8f-154">См. также</span><span class="sxs-lookup"><span data-stu-id="d8c8f-154">See also</span></span>



[<span data-ttu-id="d8c8f-155">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="d8c8f-155">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d8c8f-156">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="d8c8f-156">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d8c8f-157">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="d8c8f-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="d8c8f-158">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="d8c8f-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)

