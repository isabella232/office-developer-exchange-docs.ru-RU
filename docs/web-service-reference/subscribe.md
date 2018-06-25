---
title: Подписка
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
description: Подписки на элемент содержит свойства, используемые для создания подписок.
ms.openlocfilehash: 9f23f566f9105c655b289ed9b434c5e7b917207f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835618"
---
# <a name="subscribe"></a><span data-ttu-id="d347c-103">Подписка</span><span class="sxs-lookup"><span data-stu-id="d347c-103">Subscribe</span></span>

<span data-ttu-id="d347c-104">**Подписки на** элемент содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="d347c-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="d347c-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="d347c-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d347c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d347c-106">Attributes and elements</span></span>

<span data-ttu-id="d347c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d347c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d347c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d347c-108">Attributes</span></span>

<span data-ttu-id="d347c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d347c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d347c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d347c-110">Child elements</span></span>

|<span data-ttu-id="d347c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d347c-111">**Element**</span></span>|<span data-ttu-id="d347c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d347c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d347c-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d347c-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="d347c-114">Представляет подписку на уведомления событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="d347c-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="d347c-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d347c-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="d347c-116">Представляет подписку на уведомления на основе push события.</span><span class="sxs-lookup"><span data-stu-id="d347c-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="d347c-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d347c-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="d347c-118">Представляет подписки для потоковой передачи уведомления о событии.</span><span class="sxs-lookup"><span data-stu-id="d347c-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d347c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d347c-119">Parent elements</span></span>

<span data-ttu-id="d347c-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="d347c-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d347c-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="d347c-121">Remarks</span></span>

<span data-ttu-id="d347c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d347c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d347c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d347c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d347c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d347c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d347c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d347c-125">Schema name</span></span>  <br/> |<span data-ttu-id="d347c-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d347c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d347c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d347c-127">Validation file</span></span>  <br/> |<span data-ttu-id="d347c-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d347c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d347c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d347c-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d347c-130">False</span><span class="sxs-lookup"><span data-stu-id="d347c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d347c-131">См. также</span><span class="sxs-lookup"><span data-stu-id="d347c-131">See also</span></span>



[<span data-ttu-id="d347c-132">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="d347c-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d347c-133">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="d347c-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d347c-134">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="d347c-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="d347c-135">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="d347c-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

