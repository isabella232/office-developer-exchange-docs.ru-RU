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
ms.openlocfilehash: f60e67654fb6af76e8081036a3463f5be401862d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530960"
---
# <a name="subscribe"></a><span data-ttu-id="51b99-103">Подписаться</span><span class="sxs-lookup"><span data-stu-id="51b99-103">Subscribe</span></span>

<span data-ttu-id="51b99-104">Элемент **Subscribe** содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="51b99-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="51b99-105">**субскрибетипе**</span><span class="sxs-lookup"><span data-stu-id="51b99-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51b99-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="51b99-106">Attributes and elements</span></span>

<span data-ttu-id="51b99-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="51b99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51b99-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="51b99-108">Attributes</span></span>

<span data-ttu-id="51b99-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51b99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51b99-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="51b99-110">Child elements</span></span>

|<span data-ttu-id="51b99-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51b99-111">**Element**</span></span>|<span data-ttu-id="51b99-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51b99-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51b99-113">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="51b99-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="51b99-114">Представляет подписку на уведомление о событии на основе запроса.</span><span class="sxs-lookup"><span data-stu-id="51b99-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="51b99-115">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="51b99-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="51b99-116">Представляет подписку на уведомление о событии с использованием push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="51b99-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="51b99-117">стреамингсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="51b99-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="51b99-118">Представляет подписку на уведомление о событии потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="51b99-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51b99-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="51b99-119">Parent elements</span></span>

<span data-ttu-id="51b99-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="51b99-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51b99-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="51b99-121">Remarks</span></span>

<span data-ttu-id="51b99-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="51b99-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51b99-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="51b99-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51b99-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="51b99-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="51b99-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="51b99-125">Schema name</span></span>  <br/> |<span data-ttu-id="51b99-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="51b99-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="51b99-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="51b99-127">Validation file</span></span>  <br/> |<span data-ttu-id="51b99-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="51b99-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51b99-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="51b99-129">Can be empty</span></span>  <br/> |<span data-ttu-id="51b99-130">False</span><span class="sxs-lookup"><span data-stu-id="51b99-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51b99-131">См. также</span><span class="sxs-lookup"><span data-stu-id="51b99-131">See also</span></span>



[<span data-ttu-id="51b99-132">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="51b99-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="51b99-133">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="51b99-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="51b99-134">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="51b99-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="51b99-135">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="51b99-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

