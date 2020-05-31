---
title: статусевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: Элемент Статусевент представляет уведомление о том, что в почтовом ящике не было новых действий.
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835592"
---
# <a name="statusevent"></a><span data-ttu-id="e3073-103">статусевент</span><span class="sxs-lookup"><span data-stu-id="e3073-103">StatusEvent</span></span>

<span data-ttu-id="e3073-104">Элемент **статусевент** представляет уведомление о том, что в почтовом ящике не было новых действий.</span><span class="sxs-lookup"><span data-stu-id="e3073-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="e3073-105">**басенотификатионевенттипе**</span><span class="sxs-lookup"><span data-stu-id="e3073-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3073-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e3073-106">Attributes and elements</span></span>

<span data-ttu-id="e3073-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e3073-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3073-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e3073-108">Attributes</span></span>

<span data-ttu-id="e3073-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e3073-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3073-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e3073-110">Child elements</span></span>

|<span data-ttu-id="e3073-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3073-111">**Element**</span></span>|<span data-ttu-id="e3073-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3073-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3073-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="e3073-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="e3073-114">Представляет последний действительный водяной знак для подписки.</span><span class="sxs-lookup"><span data-stu-id="e3073-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3073-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e3073-115">Parent elements</span></span>

|<span data-ttu-id="e3073-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3073-116">**Element**</span></span>|<span data-ttu-id="e3073-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3073-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3073-118">Уведомление</span><span class="sxs-lookup"><span data-stu-id="e3073-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e3073-119">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="e3073-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3073-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="e3073-120">Remarks</span></span>

<span data-ttu-id="e3073-121">Элемент **статусевент** возвращается в уведомлении по одной из следующих причин:</span><span class="sxs-lookup"><span data-stu-id="e3073-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="e3073-122">Опрашивающий клиент отправляет запрос на получение событий в подписке, не имеющей действий.</span><span class="sxs-lookup"><span data-stu-id="e3073-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="e3073-123">При достижении [StatusFrequency](statusfrequency.md) в очереди в очереди нет событий.</span><span class="sxs-lookup"><span data-stu-id="e3073-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="e3073-124">[Водяной знак](watermark.md) **статусевент**используется в клиентском приложении так же, как и другие подложки типа события.</span><span class="sxs-lookup"><span data-stu-id="e3073-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="e3073-125">Однако водяной знак для **статусевент** не совпадает с водяными знаками, используемыми для других событий.</span><span class="sxs-lookup"><span data-stu-id="e3073-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="e3073-126">Например, подписка имеет события с водяными знаками 1, 2 и 3, и эти события успешно переданы в уведомлении.</span><span class="sxs-lookup"><span data-stu-id="e3073-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="e3073-127">Возникает период отсутствия активности и отправляется запрос на получение **событий** .</span><span class="sxs-lookup"><span data-stu-id="e3073-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="e3073-128">Сервер клиентского доступа возвращает событие состояния и включает последний водяной знак, 3, как [превиаусватермарк](previouswatermark.md) и текущий [водяной знак](watermark.md).</span><span class="sxs-lookup"><span data-stu-id="e3073-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="e3073-129">Водяной знак не останется одинаковым во всех случаях.</span><span class="sxs-lookup"><span data-stu-id="e3073-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="e3073-130">Записи событий хранятся в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="e3073-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="e3073-131">Чтобы поддерживать активную подписку, CAS периодически обновляет водяные знаки для очередей подписки.</span><span class="sxs-lookup"><span data-stu-id="e3073-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="e3073-132">Обновленные водяные знаки отправляются клиентам для поддержки активной подписки.</span><span class="sxs-lookup"><span data-stu-id="e3073-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="e3073-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e3073-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3073-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e3073-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3073-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e3073-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3073-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e3073-136">Schema name</span></span>  <br/> |<span data-ttu-id="e3073-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e3073-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3073-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e3073-138">Validation file</span></span>  <br/> |<span data-ttu-id="e3073-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e3073-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3073-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e3073-140">Can be empty</span></span>  <br/> |<span data-ttu-id="e3073-141">False</span><span class="sxs-lookup"><span data-stu-id="e3073-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3073-142">См. также</span><span class="sxs-lookup"><span data-stu-id="e3073-142">See also</span></span>



[<span data-ttu-id="e3073-143">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="e3073-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="e3073-144">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="e3073-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="e3073-145">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="e3073-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)

