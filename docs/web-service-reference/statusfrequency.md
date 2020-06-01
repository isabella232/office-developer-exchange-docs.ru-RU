---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: Элемент StatusFrequency представляет максимальное значение времени ожидания (в минутах), в течение которого предпринимает попытку выполнить повторные попытки на сервере.
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468245"
---
# <a name="statusfrequency"></a><span data-ttu-id="13117-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="13117-103">StatusFrequency</span></span>

<span data-ttu-id="13117-104">Элемент **StatusFrequency** представляет максимальное значение времени ожидания (в минутах), в течение которого предпринимает попытку выполнить повторные попытки на сервере.</span><span class="sxs-lookup"><span data-stu-id="13117-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="13117-105">Подписаться</span><span class="sxs-lookup"><span data-stu-id="13117-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="13117-106">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="13117-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="13117-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="13117-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="13117-108">**субскриптионстатусфрекуенцитипе**</span><span class="sxs-lookup"><span data-stu-id="13117-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13117-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="13117-109">Attributes and elements</span></span>

<span data-ttu-id="13117-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="13117-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13117-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="13117-111">Attributes</span></span>

<span data-ttu-id="13117-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13117-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13117-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="13117-113">Child elements</span></span>

<span data-ttu-id="13117-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="13117-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="13117-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="13117-115">Parent elements</span></span>

|<span data-ttu-id="13117-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13117-116">**Element**</span></span>|<span data-ttu-id="13117-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13117-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13117-118">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="13117-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="13117-119">Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="13117-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13117-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="13117-120">Text value</span></span>

<span data-ttu-id="13117-121">При использовании этого элемента необходимо указать текстовое значение, представляющее целое число.</span><span class="sxs-lookup"><span data-stu-id="13117-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="13117-122">Возможные значения для этого элемента — от 1 до 1440 включительно.</span><span class="sxs-lookup"><span data-stu-id="13117-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="13117-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="13117-123">This element is optional.</span></span> <span data-ttu-id="13117-124">Значение по умолчанию  30 минут.</span><span class="sxs-lookup"><span data-stu-id="13117-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="13117-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="13117-125">Remarks</span></span>

<span data-ttu-id="13117-126">Значение **StatusFrequency** используется сервером для повторной отправки push-уведомления, когда он не получает ответа на push-уведомление или состояние ping от клиента.</span><span class="sxs-lookup"><span data-stu-id="13117-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="13117-127">Если сервер не получает ответ, он попытается отправить уведомление несколько раз, прежде чем перестало отправлять уведомление.</span><span class="sxs-lookup"><span data-stu-id="13117-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="13117-128">В EWS интервал повтора по умолчанию составляет 30 секунд, а последующие повторы всегда вдвое отличаются от времени последней повторной попытки.</span><span class="sxs-lookup"><span data-stu-id="13117-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="13117-129">Время повтора не точнее, так как они могут быть задержаны из-за других нагрузок на сервере.</span><span class="sxs-lookup"><span data-stu-id="13117-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="13117-130">В приведенной ниже таблице показано, как интервалы повтора происходят в 30 минут, выделенных значением **StatusFrequency** по умолчанию (предполагая, что сервер не столкнулся с задержками).</span><span class="sxs-lookup"><span data-stu-id="13117-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="13117-131">**Повторить**</span><span class="sxs-lookup"><span data-stu-id="13117-131">**Retry**</span></span>|<span data-ttu-id="13117-132">**Секунды**</span><span class="sxs-lookup"><span data-stu-id="13117-132">**Seconds**</span></span>|<span data-ttu-id="13117-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="13117-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="13117-134">нуль</span><span class="sxs-lookup"><span data-stu-id="13117-134">0</span></span>  <br/> |<span data-ttu-id="13117-135">нуль</span><span class="sxs-lookup"><span data-stu-id="13117-135">0</span></span>  <br/> |<span data-ttu-id="13117-136">Начальная синхронизация</span><span class="sxs-lookup"><span data-stu-id="13117-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="13117-137">1 </span><span class="sxs-lookup"><span data-stu-id="13117-137">1</span></span>  <br/> |<span data-ttu-id="13117-138">более</span><span class="sxs-lookup"><span data-stu-id="13117-138">30</span></span>  <br/> |<span data-ttu-id="13117-139">00:30</span><span class="sxs-lookup"><span data-stu-id="13117-139">00:30</span></span>  <br/> |
|<span data-ttu-id="13117-140">2</span><span class="sxs-lookup"><span data-stu-id="13117-140">2</span></span>  <br/> |<span data-ttu-id="13117-141">60</span><span class="sxs-lookup"><span data-stu-id="13117-141">60</span></span>  <br/> |<span data-ttu-id="13117-142">01:00</span><span class="sxs-lookup"><span data-stu-id="13117-142">01:00</span></span>  <br/> |
|<span data-ttu-id="13117-143">4</span><span class="sxs-lookup"><span data-stu-id="13117-143">3</span></span>  <br/> |<span data-ttu-id="13117-144">120</span><span class="sxs-lookup"><span data-stu-id="13117-144">120</span></span>  <br/> |<span data-ttu-id="13117-145">02:00</span><span class="sxs-lookup"><span data-stu-id="13117-145">02:00</span></span>  <br/> |
|<span data-ttu-id="13117-146">4 </span><span class="sxs-lookup"><span data-stu-id="13117-146">4</span></span>  <br/> |<span data-ttu-id="13117-147">240</span><span class="sxs-lookup"><span data-stu-id="13117-147">240</span></span>  <br/> |<span data-ttu-id="13117-148">04:00</span><span class="sxs-lookup"><span data-stu-id="13117-148">04:00</span></span>  <br/> |
|<span data-ttu-id="13117-149">5 </span><span class="sxs-lookup"><span data-stu-id="13117-149">5</span></span>  <br/> |<span data-ttu-id="13117-150">480</span><span class="sxs-lookup"><span data-stu-id="13117-150">480</span></span>  <br/> |<span data-ttu-id="13117-151">08:00</span><span class="sxs-lookup"><span data-stu-id="13117-151">08:00</span></span>  <br/> |
|<span data-ttu-id="13117-152">6 </span><span class="sxs-lookup"><span data-stu-id="13117-152">6</span></span>  <br/> |<span data-ttu-id="13117-153">960</span><span class="sxs-lookup"><span data-stu-id="13117-153">960</span></span>  <br/> |<span data-ttu-id="13117-154">16:00</span><span class="sxs-lookup"><span data-stu-id="13117-154">16:00</span></span>  <br/> |
|<span data-ttu-id="13117-155">7 </span><span class="sxs-lookup"><span data-stu-id="13117-155">7</span></span>  <br/> |<span data-ttu-id="13117-156">1920</span><span class="sxs-lookup"><span data-stu-id="13117-156">1920</span></span>  <br/> |<span data-ttu-id="13117-157">32:00 — значение по умолчанию ( **StatusFrequency** ) — 30, повторная попытка не отправлена</span><span class="sxs-lookup"><span data-stu-id="13117-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="13117-158">Если клиент не получает уведомления от сервера в течение определенного периода времени, который превышает время, указанное в **StatusFrequency**, клиент должен выполнить такие действия, как повторное создание подписки.</span><span class="sxs-lookup"><span data-stu-id="13117-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="13117-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="13117-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13117-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="13117-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13117-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="13117-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13117-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="13117-162">Schema name</span></span>  <br/> |<span data-ttu-id="13117-163">Схема Types</span><span class="sxs-lookup"><span data-stu-id="13117-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="13117-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="13117-164">Validation file</span></span>  <br/> |<span data-ttu-id="13117-165">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="13117-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13117-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="13117-166">Can be empty</span></span>  <br/> |<span data-ttu-id="13117-167">False</span><span class="sxs-lookup"><span data-stu-id="13117-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13117-168">См. также</span><span class="sxs-lookup"><span data-stu-id="13117-168">See also</span></span>



[<span data-ttu-id="13117-169">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="13117-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="13117-170">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="13117-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="13117-171">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="13117-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="13117-172">Watermark</span><span class="sxs-lookup"><span data-stu-id="13117-172">Watermark</span></span>](watermark.md)

