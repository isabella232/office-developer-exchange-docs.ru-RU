---
title: Watermark
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
description: Элемент водяного знака представляет закладку события в очереди событий почтового ящика.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840487"
---
# <a name="watermark"></a><span data-ttu-id="d8abb-103">Watermark</span><span class="sxs-lookup"><span data-stu-id="d8abb-103">Watermark</span></span>

<span data-ttu-id="d8abb-104">Элемент **водяного знака** представляет закладку события в очереди событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d8abb-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="d8abb-105">**ватермарктипе**</span><span class="sxs-lookup"><span data-stu-id="d8abb-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8abb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8abb-106">Attributes and elements</span></span>

<span data-ttu-id="d8abb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d8abb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8abb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8abb-108">Attributes</span></span>

<span data-ttu-id="d8abb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8abb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8abb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8abb-110">Child elements</span></span>

<span data-ttu-id="d8abb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8abb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8abb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8abb-112">Parent elements</span></span>

|<span data-ttu-id="d8abb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8abb-113">**Element**</span></span>|<span data-ttu-id="d8abb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8abb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8abb-115">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="d8abb-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="d8abb-116">Представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="d8abb-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-117">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="d8abb-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="d8abb-118">Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="d8abb-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="d8abb-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="d8abb-120">Представляет операцию, используемую клиентами опрашивающей репликации для запроса уведомлений с сервера.</span><span class="sxs-lookup"><span data-stu-id="d8abb-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-121">копиедевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d8abb-122">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="d8abb-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-123">креатедевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="d8abb-124">Представляет событие, в котором создается элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="d8abb-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-125">делетедевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="d8abb-126">Представляет событие, в котором удаляется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="d8abb-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-127">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d8abb-128">Представляет событие, в котором изменяется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="d8abb-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-129">моведевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d8abb-130">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="d8abb-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-131">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="d8abb-132">Представляет событие, инициированное новым почтовым элементом в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d8abb-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-133">статусевент</span><span class="sxs-lookup"><span data-stu-id="d8abb-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="d8abb-134">Представляет уведомление о том, что в почтовом ящике не было новых действий.</span><span class="sxs-lookup"><span data-stu-id="d8abb-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8abb-135">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="d8abb-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="d8abb-136">Содержит состояние и результат запроса на подписку.</span><span class="sxs-lookup"><span data-stu-id="d8abb-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8abb-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d8abb-137">Text value</span></span>

<span data-ttu-id="d8abb-138">Текстовое значение может быть обязательным или необязательным в зависимости от того, как этот элемент используется.</span><span class="sxs-lookup"><span data-stu-id="d8abb-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8abb-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="d8abb-139">Remarks</span></span>

<span data-ttu-id="d8abb-140">Если запрос на подписку содержит водяной знак, создается подписка на основе перенаправления водяного знака.</span><span class="sxs-lookup"><span data-stu-id="d8abb-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="d8abb-141">Если запрос на подписку содержит водяной знак, не найденный в таблице событий почтовых ящиков, клиентское приложение возвращает `ErrorInvalidWatermark` сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d8abb-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="d8abb-142">Это может произойти, если водяной знак является слишком старым и был удален из 30-дневного окна таблицы события или если водяного знака отсутствовал в таблице Events.</span><span class="sxs-lookup"><span data-stu-id="d8abb-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="d8abb-143">Например, это может произойти, если водяной знак получен из другой подписки для почтового ящика в другой базе данных.</span><span class="sxs-lookup"><span data-stu-id="d8abb-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="d8abb-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d8abb-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8abb-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8abb-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8abb-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8abb-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8abb-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8abb-147">Schema name</span></span>  <br/> |<span data-ttu-id="d8abb-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d8abb-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8abb-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8abb-149">Validation file</span></span>  <br/> |<span data-ttu-id="d8abb-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d8abb-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8abb-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8abb-151">Can be empty</span></span>  <br/> |<span data-ttu-id="d8abb-152">False</span><span class="sxs-lookup"><span data-stu-id="d8abb-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8abb-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d8abb-153">See also</span></span>



[<span data-ttu-id="d8abb-154">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="d8abb-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d8abb-155">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="d8abb-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d8abb-156">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="d8abb-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)

