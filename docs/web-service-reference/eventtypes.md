---
title: евенттипес
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
description: Элемент Евенттипес содержит коллекцию типов уведомлений о событиях, которые используются для создания подписки.
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530630"
---
# <a name="eventtypes"></a><span data-ttu-id="957ac-103">евенттипес</span><span class="sxs-lookup"><span data-stu-id="957ac-103">EventTypes</span></span>

<span data-ttu-id="957ac-104">Элемент **евенттипес** содержит коллекцию типов уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="957ac-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="957ac-105">**нонемптяррайофнотификатионевенттипестипе**</span><span class="sxs-lookup"><span data-stu-id="957ac-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="957ac-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="957ac-106">Attributes and elements</span></span>

<span data-ttu-id="957ac-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="957ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="957ac-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="957ac-108">Attributes</span></span>

<span data-ttu-id="957ac-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="957ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="957ac-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="957ac-110">Child elements</span></span>

|<span data-ttu-id="957ac-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="957ac-111">**Element**</span></span>|<span data-ttu-id="957ac-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="957ac-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="957ac-113">EventType</span><span class="sxs-lookup"><span data-stu-id="957ac-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="957ac-114">Представляет запрошенный тип уведомления о событии, который используется для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="957ac-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="957ac-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="957ac-115">Parent elements</span></span>

|<span data-ttu-id="957ac-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="957ac-116">**Element**</span></span>|<span data-ttu-id="957ac-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="957ac-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="957ac-118">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="957ac-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="957ac-119">Представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="957ac-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="957ac-120">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="957ac-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="957ac-121">Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="957ac-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="957ac-122">стреамингсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="957ac-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="957ac-123">Представляет подписку на подписку на уведомления о событиях потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="957ac-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="957ac-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="957ac-124">Text value</span></span>

<span data-ttu-id="957ac-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="957ac-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="957ac-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="957ac-126">Remarks</span></span>

<span data-ttu-id="957ac-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="957ac-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="957ac-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="957ac-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="957ac-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="957ac-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="957ac-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="957ac-130">Schema Name</span></span>  <br/> |<span data-ttu-id="957ac-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="957ac-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="957ac-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="957ac-132">Validation File</span></span>  <br/> |<span data-ttu-id="957ac-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="957ac-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="957ac-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="957ac-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="957ac-135">False</span><span class="sxs-lookup"><span data-stu-id="957ac-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="957ac-136">См. также</span><span class="sxs-lookup"><span data-stu-id="957ac-136">See also</span></span>



[<span data-ttu-id="957ac-137">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="957ac-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="957ac-138">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="957ac-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="957ac-139">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="957ac-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="957ac-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="957ac-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

