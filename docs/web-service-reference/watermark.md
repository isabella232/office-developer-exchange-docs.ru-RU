---
title: Водяной знак
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: Элемент водяной знак — это закладка события в очереди событий почтового ящика.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840487"
---
# <a name="watermark"></a><span data-ttu-id="bc891-103">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="bc891-103">Watermark</span></span>

<span data-ttu-id="bc891-104">Элемент **водяной знак** — это закладка события в очереди событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bc891-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="bc891-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="bc891-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc891-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc891-106">Attributes and elements</span></span>

<span data-ttu-id="bc891-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bc891-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc891-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc891-108">Attributes</span></span>

<span data-ttu-id="bc891-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc891-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc891-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc891-110">Child elements</span></span>

<span data-ttu-id="bc891-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc891-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc891-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc891-112">Parent elements</span></span>

|<span data-ttu-id="bc891-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc891-113">**Element**</span></span>|<span data-ttu-id="bc891-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc891-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc891-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="bc891-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="bc891-116">Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="bc891-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="bc891-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="bc891-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="bc891-118">Представляет подписка на подписку на уведомления о принудительной события.</span><span class="sxs-lookup"><span data-stu-id="bc891-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="bc891-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="bc891-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="bc891-120">Представляет операцию, используемую клиентами пула для запроса уведомлений с сервера.</span><span class="sxs-lookup"><span data-stu-id="bc891-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="bc891-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="bc891-122">Представляет событие, куда копируются элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="bc891-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="bc891-123">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="bc891-124">Представляет событие, где создается элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="bc891-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="bc891-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="bc891-126">Представляет событие, где удаления элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="bc891-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="bc891-127">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="bc891-128">Представляет событие, где при изменении элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="bc891-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="bc891-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="bc891-130">Представляет событие, где элемента или папки перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="bc891-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="bc891-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="bc891-132">Представляет события, вызванные нового элемента почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bc891-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bc891-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="bc891-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="bc891-134">Представляет уведомление о том, что не новые действия в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bc891-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bc891-135">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bc891-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="bc891-136">Содержит состояние и результат запроса подписаться.</span><span class="sxs-lookup"><span data-stu-id="bc891-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc891-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc891-137">Text value</span></span>

<span data-ttu-id="bc891-138">Текстовое значение может быть обязательный или необязательный в зависимости от того, как используется данный элемент.</span><span class="sxs-lookup"><span data-stu-id="bc891-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc891-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc891-139">Remarks</span></span>

<span data-ttu-id="bc891-140">Если подписки на запрос содержит водяного знака, от переадресации водяного знака создается подписка.</span><span class="sxs-lookup"><span data-stu-id="bc891-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="bc891-141">Если запрос подписки на содержит водяной знак, не найден в таблице событий почтового ящика `ErrorInvalidWatermark` клиентскому приложению возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="bc891-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="bc891-142">Это может произойти, если водяной знак устарел и был удален из окна 30-дневный таблицы событий или если водяной знак не требуется даже представления в таблице "events".</span><span class="sxs-lookup"><span data-stu-id="bc891-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="bc891-143">Например, это может произойти, если водяной знак получен из другой подписки для почтового ящика в другую базу данных.</span><span class="sxs-lookup"><span data-stu-id="bc891-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="bc891-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc891-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc891-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc891-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc891-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc891-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc891-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc891-147">Schema name</span></span>  <br/> |<span data-ttu-id="bc891-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bc891-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc891-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc891-149">Validation file</span></span>  <br/> |<span data-ttu-id="bc891-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc891-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc891-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc891-151">Can be empty</span></span>  <br/> |<span data-ttu-id="bc891-152">False</span><span class="sxs-lookup"><span data-stu-id="bc891-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc891-153">См. также</span><span class="sxs-lookup"><span data-stu-id="bc891-153">See also</span></span>



[<span data-ttu-id="bc891-154">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="bc891-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="bc891-155">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="bc891-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="bc891-156">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="bc891-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)

