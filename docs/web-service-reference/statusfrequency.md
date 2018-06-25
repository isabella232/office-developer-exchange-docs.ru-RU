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
description: Элемент StatusFrequency представляет максимальное время ожидания в минутах, в которых повторных попыток на сервере.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835589"
---
# <a name="statusfrequency"></a><span data-ttu-id="dfe9c-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="dfe9c-103">StatusFrequency</span></span>

<span data-ttu-id="dfe9c-104">Элемент **StatusFrequency** представляет максимальное время ожидания в минутах, в которых повторных попыток на сервере.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="dfe9c-105">Подписка</span><span class="sxs-lookup"><span data-stu-id="dfe9c-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="dfe9c-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="dfe9c-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="dfe9c-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="dfe9c-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="dfe9c-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfe9c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfe9c-109">Attributes and elements</span></span>

<span data-ttu-id="dfe9c-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfe9c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfe9c-111">Attributes</span></span>

<span data-ttu-id="dfe9c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfe9c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfe9c-113">Child elements</span></span>

<span data-ttu-id="dfe9c-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dfe9c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfe9c-115">Parent elements</span></span>

|<span data-ttu-id="dfe9c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-116">**Element**</span></span>|<span data-ttu-id="dfe9c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfe9c-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="dfe9c-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="dfe9c-119">Представляет подписка на подписку на уведомления о принудительной события.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dfe9c-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dfe9c-120">Text value</span></span>

<span data-ttu-id="dfe9c-121">Текстовое значение, представляющее целое число является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="dfe9c-122">Возможные значения для этого элемента: 1 до 1440 включительно.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="dfe9c-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-123">This element is optional.</span></span> <span data-ttu-id="dfe9c-124">Значение по умолчанию — 30 минут.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dfe9c-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="dfe9c-125">Remarks</span></span>

<span data-ttu-id="dfe9c-126">Значение **StatusFrequency** используется сервером-Повтор push-уведомления, когда не получает ответ push-уведомлений или состояние ping от клиента.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="dfe9c-127">Если сервер не получает ответ, повторов отправки уведомления несколько раз до остановки его отправки.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="dfe9c-128">В веб-служб Exchange интервал повтора по умолчанию — 30 секунд и последующих попыток, всегда double времени последнего интервал повтора.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="dfe9c-129">Время повтора не точное, как их можно отложить из-за другие нагрузки на сервере.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="dfe9c-130">В следующей таблице показаны как интервалы повтора возникают в 30 минут, выделенной значением по умолчанию **StatusFrequency** (предполагается, что сервер не обнаружил любой задержки).</span><span class="sxs-lookup"><span data-stu-id="dfe9c-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="dfe9c-131">**Число повторов**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-131">**Retry**</span></span>|<span data-ttu-id="dfe9c-132">**Секунд**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-132">**Seconds**</span></span>|<span data-ttu-id="dfe9c-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="dfe9c-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dfe9c-134">0</span><span class="sxs-lookup"><span data-stu-id="dfe9c-134">0</span></span>  <br/> |<span data-ttu-id="dfe9c-135">0</span><span class="sxs-lookup"><span data-stu-id="dfe9c-135">0</span></span>  <br/> |<span data-ttu-id="dfe9c-136">Начальной синхронизации</span><span class="sxs-lookup"><span data-stu-id="dfe9c-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="dfe9c-137">1</span><span class="sxs-lookup"><span data-stu-id="dfe9c-137">1</span></span>  <br/> |<span data-ttu-id="dfe9c-138">30</span><span class="sxs-lookup"><span data-stu-id="dfe9c-138">30</span></span>  <br/> |<span data-ttu-id="dfe9c-139">00:30</span><span class="sxs-lookup"><span data-stu-id="dfe9c-139">00:30</span></span>  <br/> |
|<span data-ttu-id="dfe9c-140">2</span><span class="sxs-lookup"><span data-stu-id="dfe9c-140">2</span></span>  <br/> |<span data-ttu-id="dfe9c-141">60</span><span class="sxs-lookup"><span data-stu-id="dfe9c-141">60</span></span>  <br/> |<span data-ttu-id="dfe9c-142">01:00</span><span class="sxs-lookup"><span data-stu-id="dfe9c-142">01:00</span></span>  <br/> |
|<span data-ttu-id="dfe9c-143">3</span><span class="sxs-lookup"><span data-stu-id="dfe9c-143">3</span></span>  <br/> |<span data-ttu-id="dfe9c-144">120</span><span class="sxs-lookup"><span data-stu-id="dfe9c-144">120</span></span>  <br/> |<span data-ttu-id="dfe9c-145">02:00</span><span class="sxs-lookup"><span data-stu-id="dfe9c-145">02:00</span></span>  <br/> |
|<span data-ttu-id="dfe9c-146">4</span><span class="sxs-lookup"><span data-stu-id="dfe9c-146">4</span></span>  <br/> |<span data-ttu-id="dfe9c-147">240</span><span class="sxs-lookup"><span data-stu-id="dfe9c-147">240</span></span>  <br/> |<span data-ttu-id="dfe9c-148">04:00</span><span class="sxs-lookup"><span data-stu-id="dfe9c-148">04:00</span></span>  <br/> |
|<span data-ttu-id="dfe9c-149">5</span><span class="sxs-lookup"><span data-stu-id="dfe9c-149">5</span></span>  <br/> |<span data-ttu-id="dfe9c-150">480</span><span class="sxs-lookup"><span data-stu-id="dfe9c-150">480</span></span>  <br/> |<span data-ttu-id="dfe9c-151">08:00</span><span class="sxs-lookup"><span data-stu-id="dfe9c-151">08:00</span></span>  <br/> |
|<span data-ttu-id="dfe9c-152">6</span><span class="sxs-lookup"><span data-stu-id="dfe9c-152">6</span></span>  <br/> |<span data-ttu-id="dfe9c-153">960</span><span class="sxs-lookup"><span data-stu-id="dfe9c-153">960</span></span>  <br/> |<span data-ttu-id="dfe9c-154">16:00</span><span class="sxs-lookup"><span data-stu-id="dfe9c-154">16:00</span></span>  <br/> |
|<span data-ttu-id="dfe9c-155">7</span><span class="sxs-lookup"><span data-stu-id="dfe9c-155">7</span></span>  <br/> |<span data-ttu-id="dfe9c-156">1920</span><span class="sxs-lookup"><span data-stu-id="dfe9c-156">1920</span></span>  <br/> |<span data-ttu-id="dfe9c-157">32:00 - **StatusFrequency** значение по умолчанию 30 превышено, не отправляются число повторов</span><span class="sxs-lookup"><span data-stu-id="dfe9c-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="dfe9c-158">Если клиент не получает уведомления с сервера на определенный период времени, превышающее дважды времени, заданного параметром **StatusFrequency**, клиент должен выполнять действий, например повторного создания подписки.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="dfe9c-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfe9c-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfe9c-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfe9c-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfe9c-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfe9c-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dfe9c-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfe9c-162">Schema name</span></span>  <br/> |<span data-ttu-id="dfe9c-163">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dfe9c-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="dfe9c-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfe9c-164">Validation file</span></span>  <br/> |<span data-ttu-id="dfe9c-165">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dfe9c-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dfe9c-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfe9c-166">Can be empty</span></span>  <br/> |<span data-ttu-id="dfe9c-167">False</span><span class="sxs-lookup"><span data-stu-id="dfe9c-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dfe9c-168">См. также</span><span class="sxs-lookup"><span data-stu-id="dfe9c-168">See also</span></span>



[<span data-ttu-id="dfe9c-169">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="dfe9c-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="dfe9c-170">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="dfe9c-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="dfe9c-171">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="dfe9c-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="dfe9c-172">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="dfe9c-172">Watermark</span></span>](watermark.md)

