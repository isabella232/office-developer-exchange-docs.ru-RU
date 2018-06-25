---
title: EventTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: Элемент EventTypes содержит коллекцию типов событий уведомлений, которые используются для создания подписки.
ms.openlocfilehash: f4c622376f6b607ed390511d7bb5f0f723889420
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762396"
---
# <a name="eventtypes"></a><span data-ttu-id="27fae-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="27fae-103">EventTypes</span></span>

<span data-ttu-id="27fae-104">Элемент **EventTypes** содержит коллекцию типов событий уведомлений, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="27fae-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="27fae-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="27fae-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27fae-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="27fae-106">Attributes and elements</span></span>

<span data-ttu-id="27fae-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="27fae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27fae-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="27fae-108">Attributes</span></span>

<span data-ttu-id="27fae-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="27fae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27fae-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="27fae-110">Child elements</span></span>

|<span data-ttu-id="27fae-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27fae-111">**Element**</span></span>|<span data-ttu-id="27fae-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27fae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27fae-113">EventType</span><span class="sxs-lookup"><span data-stu-id="27fae-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="27fae-114">Представляет тип уведомлений запрошенные событий, который используется для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="27fae-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27fae-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="27fae-115">Parent elements</span></span>

|<span data-ttu-id="27fae-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27fae-116">**Element**</span></span>|<span data-ttu-id="27fae-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27fae-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27fae-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="27fae-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="27fae-119">Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="27fae-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="27fae-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="27fae-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="27fae-121">Представляет подписка на подписку на уведомления о принудительной события.</span><span class="sxs-lookup"><span data-stu-id="27fae-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="27fae-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="27fae-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="27fae-123">Представляет подписка на подписку на уведомления о потоковой передачи событий.</span><span class="sxs-lookup"><span data-stu-id="27fae-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27fae-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="27fae-124">Text value</span></span>

<span data-ttu-id="27fae-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="27fae-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27fae-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="27fae-126">Remarks</span></span>

<span data-ttu-id="27fae-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="27fae-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27fae-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="27fae-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27fae-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="27fae-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27fae-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="27fae-130">Schema Name</span></span>  <br/> |<span data-ttu-id="27fae-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="27fae-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="27fae-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="27fae-132">Validation File</span></span>  <br/> |<span data-ttu-id="27fae-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="27fae-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27fae-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="27fae-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="27fae-135">False</span><span class="sxs-lookup"><span data-stu-id="27fae-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27fae-136">См. также</span><span class="sxs-lookup"><span data-stu-id="27fae-136">See also</span></span>



[<span data-ttu-id="27fae-137">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="27fae-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="27fae-138">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="27fae-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="27fae-139">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="27fae-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="27fae-140">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="27fae-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

