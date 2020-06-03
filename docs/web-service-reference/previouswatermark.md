---
title: превиаусватермарк
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
description: Элемент Превиаусватермарк представляет водяной знак последнего события, который был успешно передан клиенту для подписки.
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461655"
---
# <a name="previouswatermark"></a><span data-ttu-id="5abae-103">превиаусватермарк</span><span class="sxs-lookup"><span data-stu-id="5abae-103">PreviousWatermark</span></span>

<span data-ttu-id="5abae-104">Элемент **превиаусватермарк** представляет водяной знак последнего события, который был успешно передан клиенту для подписки.</span><span class="sxs-lookup"><span data-stu-id="5abae-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="5abae-105">**ватермарктипе**</span><span class="sxs-lookup"><span data-stu-id="5abae-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5abae-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5abae-106">Attributes and elements</span></span>

<span data-ttu-id="5abae-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5abae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5abae-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5abae-108">Attributes</span></span>

<span data-ttu-id="5abae-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5abae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5abae-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5abae-110">Child elements</span></span>

<span data-ttu-id="5abae-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5abae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5abae-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5abae-112">Parent elements</span></span>

|<span data-ttu-id="5abae-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5abae-113">**Element**</span></span>|<span data-ttu-id="5abae-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5abae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5abae-115">Уведомление</span><span class="sxs-lookup"><span data-stu-id="5abae-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5abae-116">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="5abae-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5abae-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5abae-117">Text value</span></span>

<span data-ttu-id="5abae-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="5abae-118">A text value is required.</span></span> <span data-ttu-id="5abae-119">Текстовое значение представляет собой последний водяной знак.</span><span class="sxs-lookup"><span data-stu-id="5abae-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="5abae-120">Текстовое значение не может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="5abae-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5abae-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="5abae-121">Remarks</span></span>

<span data-ttu-id="5abae-122">Свойство **превиаусватермарк** используется для клиента при определении последнего успешного уведомления.</span><span class="sxs-lookup"><span data-stu-id="5abae-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="5abae-123">Например, если у подписки есть три события с водяными знаками 1, 2 и 3, а следующее уведомление отправляется со значением **превиаусватермарк** , равным 3, клиент может сравнить это значение со значением водяного знака последнего полученного уведомления.</span><span class="sxs-lookup"><span data-stu-id="5abae-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="5abae-124">Это позволяет клиенту обеспечить непрерывность событий.</span><span class="sxs-lookup"><span data-stu-id="5abae-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="5abae-125">Для клиентов push-уведомлений **превиаусватермарк** сравнивается с локальной последней известной водяной знакю на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="5abae-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="5abae-126">Если значения отличаются, клиент пропустил уведомление о событии и должен повторно создать подписку с помощью последней версии локального водяного знака.</span><span class="sxs-lookup"><span data-stu-id="5abae-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="5abae-127">Например, если Push-клиент получает три события для подписки с водяными знаками 1, 2 и 3, а для следующего уведомления **— значение 5, то клиент** пропустил по крайней мере одно уведомление и создал новую подписку, передавая 3 в качестве водяного знака.</span><span class="sxs-lookup"><span data-stu-id="5abae-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="5abae-128">В случае опрашивающего клиента значение Превиаусватермарк будет совпадать с [водяным знаком](watermark.md) , включенным клиентом в вызове метода **PreviousWatermark** .</span><span class="sxs-lookup"><span data-stu-id="5abae-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="5abae-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5abae-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5abae-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5abae-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5abae-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5abae-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5abae-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5abae-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5abae-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5abae-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5abae-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5abae-134">Validation File</span></span>  <br/> |<span data-ttu-id="5abae-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5abae-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5abae-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5abae-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5abae-137">False</span><span class="sxs-lookup"><span data-stu-id="5abae-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5abae-138">См. также</span><span class="sxs-lookup"><span data-stu-id="5abae-138">See also</span></span>



[<span data-ttu-id="5abae-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="5abae-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5abae-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="5abae-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5abae-141">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="5abae-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

