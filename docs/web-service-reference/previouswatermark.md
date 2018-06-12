---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: Элемент PreviousWatermark представляет водяной знак последнего события, которое было успешно передан клиенту для подписки.
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834886"
---
# <a name="previouswatermark"></a><span data-ttu-id="d51bc-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="d51bc-103">PreviousWatermark</span></span>

<span data-ttu-id="d51bc-104">Элемент **PreviousWatermark** представляет водяной знак последнего события, которое было успешно передан клиенту для подписки.</span><span class="sxs-lookup"><span data-stu-id="d51bc-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="d51bc-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="d51bc-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d51bc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d51bc-106">Attributes and elements</span></span>

<span data-ttu-id="d51bc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d51bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d51bc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d51bc-108">Attributes</span></span>

<span data-ttu-id="d51bc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d51bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d51bc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d51bc-110">Child elements</span></span>

<span data-ttu-id="d51bc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d51bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d51bc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d51bc-112">Parent elements</span></span>

|<span data-ttu-id="d51bc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d51bc-113">**Element**</span></span>|<span data-ttu-id="d51bc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d51bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d51bc-115">Уведомление</span><span class="sxs-lookup"><span data-stu-id="d51bc-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d51bc-116">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="d51bc-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d51bc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d51bc-117">Text value</span></span>

<span data-ttu-id="d51bc-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d51bc-118">A text value is required.</span></span> <span data-ttu-id="d51bc-119">Текстовое значение представляет последние водяного знака.</span><span class="sxs-lookup"><span data-stu-id="d51bc-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="d51bc-120">Текстовое значение не может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="d51bc-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d51bc-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="d51bc-121">Remarks</span></span>

<span data-ttu-id="d51bc-122">Свойство **PreviousWatermark** можно использовать для клиента в определение последнего успешного уведомления.</span><span class="sxs-lookup"><span data-stu-id="d51bc-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="d51bc-123">К примеру Если подписка содержит три события с подложки 1, 2 и 3, и следующего уведомления отправляются со значением **PreviousWatermark** 3, клиента позволяет сравнивать это значение со значением водяного знака последнего уведомления, полученного.</span><span class="sxs-lookup"><span data-stu-id="d51bc-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="d51bc-124">Это позволяет клиента для обеспечения непрерывности событий.</span><span class="sxs-lookup"><span data-stu-id="d51bc-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="d51bc-125">Для клиентов push **PreviousWatermark** сравнивается с последней подложки известные локального, со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="d51bc-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="d51bc-126">Если значения не совпадают, клиент было пропущено уведомление о событии и необходимо восстановить подписки с использованием последних локального водяного знака.</span><span class="sxs-lookup"><span data-stu-id="d51bc-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="d51bc-127">К примеру push клиент получает три события подписки с подложки 1, 2 и 3 для следующего уведомления, поступающие с **PreviousWatermark** значение 5, клиент было пропущено по крайней мере один уведомлений и следует создать новую подписку Передача 3 в качестве водяного знака.</span><span class="sxs-lookup"><span data-stu-id="d51bc-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="d51bc-128">В случае клиентом репликации по запросу значение **PreviousWatermark** будет совпадать с [водяного знака](watermark.md) , включенные клиентом в вызове GetEvents.</span><span class="sxs-lookup"><span data-stu-id="d51bc-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="d51bc-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d51bc-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d51bc-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d51bc-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d51bc-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d51bc-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d51bc-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d51bc-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d51bc-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d51bc-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d51bc-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d51bc-134">Validation File</span></span>  <br/> |<span data-ttu-id="d51bc-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d51bc-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d51bc-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d51bc-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d51bc-137">False</span><span class="sxs-lookup"><span data-stu-id="d51bc-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d51bc-138">См. также</span><span class="sxs-lookup"><span data-stu-id="d51bc-138">See also</span></span>



[<span data-ttu-id="d51bc-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="d51bc-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d51bc-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="d51bc-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d51bc-141">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="d51bc-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

