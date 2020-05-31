---
title: Подписаться
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: Элемент Subscribe содержит свойства, используемые для создания подписок.
ms.openlocfilehash: 9f23f566f9105c655b289ed9b434c5e7b917207f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835618"
---
# <a name="subscribe"></a><span data-ttu-id="e6576-103">Подписаться</span><span class="sxs-lookup"><span data-stu-id="e6576-103">Subscribe</span></span>

<span data-ttu-id="e6576-104">Элемент **Subscribe** содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="e6576-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="e6576-105">**субскрибетипе**</span><span class="sxs-lookup"><span data-stu-id="e6576-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6576-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e6576-106">Attributes and elements</span></span>

<span data-ttu-id="e6576-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e6576-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6576-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e6576-108">Attributes</span></span>

<span data-ttu-id="e6576-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e6576-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6576-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e6576-110">Child elements</span></span>

|<span data-ttu-id="e6576-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e6576-111">**Element**</span></span>|<span data-ttu-id="e6576-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e6576-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6576-113">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="e6576-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="e6576-114">Представляет подписку на уведомление о событии на основе запроса.</span><span class="sxs-lookup"><span data-stu-id="e6576-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="e6576-115">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="e6576-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="e6576-116">Представляет подписку на уведомление о событии с использованием push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="e6576-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="e6576-117">стреамингсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="e6576-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="e6576-118">Представляет подписку на уведомление о событии потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="e6576-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6576-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e6576-119">Parent elements</span></span>

<span data-ttu-id="e6576-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="e6576-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e6576-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="e6576-121">Remarks</span></span>

<span data-ttu-id="e6576-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6576-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6576-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e6576-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6576-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e6576-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e6576-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e6576-125">Schema name</span></span>  <br/> |<span data-ttu-id="e6576-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e6576-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e6576-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e6576-127">Validation file</span></span>  <br/> |<span data-ttu-id="e6576-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e6576-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6576-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e6576-129">Can be empty</span></span>  <br/> |<span data-ttu-id="e6576-130">False</span><span class="sxs-lookup"><span data-stu-id="e6576-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6576-131">См. также</span><span class="sxs-lookup"><span data-stu-id="e6576-131">See also</span></span>



[<span data-ttu-id="e6576-132">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="e6576-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="e6576-133">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="e6576-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="e6576-134">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="e6576-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="e6576-135">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="e6576-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

