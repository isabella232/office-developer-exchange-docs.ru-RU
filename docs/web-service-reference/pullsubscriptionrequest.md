---
title: пуллсубскриптионрекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: Элемент Пуллсубскриптионрекуест представляет подписку на подписку на уведомления о событиях по запросу.
ms.openlocfilehash: fb9712c9e1481678c2821ee344052783d5c25bf9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468868"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="4a8ac-103">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="4a8ac-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="4a8ac-104">Элемент **пуллсубскриптионрекуест** представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="4a8ac-105">Подписаться</span><span class="sxs-lookup"><span data-stu-id="4a8ac-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="4a8ac-106">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="4a8ac-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="4a8ac-107">**пуллсубскриптионрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a8ac-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4a8ac-108">Attributes and elements</span></span>

<span data-ttu-id="4a8ac-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a8ac-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4a8ac-110">Attributes</span></span>

|<span data-ttu-id="4a8ac-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-111">**Attribute**</span></span>|<span data-ttu-id="4a8ac-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a8ac-113">**субскрибетоаллфолдерс**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="4a8ac-114">Указывает, следует ли подписываться на все доступные папки.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="4a8ac-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4a8ac-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4a8ac-116">Child elements</span></span>

|<span data-ttu-id="4a8ac-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-117">**Element**</span></span>|<span data-ttu-id="4a8ac-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a8ac-119">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="4a8ac-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="4a8ac-120">Содержит массив идентификаторов папок, которые используются для определения папок, которые необходимо отслеживать для получения уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="4a8ac-121">евенттипес</span><span class="sxs-lookup"><span data-stu-id="4a8ac-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="4a8ac-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="4a8ac-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="4a8ac-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="4a8ac-124">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="4a8ac-125">Используется для создания подписки, которая начинается с события, представленного водяным знаком.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="4a8ac-126">Если водяной знак из запроса на подписку не найден, клиенту будет возвращен ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="4a8ac-127">Эта ошибка может возникать, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4a8ac-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="4a8ac-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="4a8ac-129">Представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a8ac-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4a8ac-130">Parent elements</span></span>

|<span data-ttu-id="4a8ac-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-131">**Element**</span></span>|<span data-ttu-id="4a8ac-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a8ac-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a8ac-133">Подписаться</span><span class="sxs-lookup"><span data-stu-id="4a8ac-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="4a8ac-134">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a8ac-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4a8ac-135">Text value</span></span>

<span data-ttu-id="4a8ac-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a8ac-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="4a8ac-137">Remarks</span></span>

<span data-ttu-id="4a8ac-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a8ac-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a8ac-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4a8ac-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a8ac-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4a8ac-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a8ac-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4a8ac-141">Schema name</span></span>  <br/> |<span data-ttu-id="4a8ac-142">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4a8ac-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4a8ac-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4a8ac-143">Validation file</span></span>  <br/> |<span data-ttu-id="4a8ac-144">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4a8ac-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a8ac-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4a8ac-145">Can be empty</span></span>  <br/> |<span data-ttu-id="4a8ac-146">False</span><span class="sxs-lookup"><span data-stu-id="4a8ac-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a8ac-147">См. также</span><span class="sxs-lookup"><span data-stu-id="4a8ac-147">See also</span></span>



[<span data-ttu-id="4a8ac-148">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="4a8ac-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="4a8ac-149">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="4a8ac-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="4a8ac-150">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="4a8ac-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="4a8ac-151">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="4a8ac-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="4a8ac-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4a8ac-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

