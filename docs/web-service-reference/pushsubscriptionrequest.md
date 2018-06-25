---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: Элемент PushSubscriptionRequest — подписка на подписку на уведомления о принудительной события.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834929"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="5fd74-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="5fd74-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="5fd74-104">Элемент **PushSubscriptionRequest** — подписка на подписку на уведомления о принудительной события.</span><span class="sxs-lookup"><span data-stu-id="5fd74-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="5fd74-105">Подписка</span><span class="sxs-lookup"><span data-stu-id="5fd74-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="5fd74-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="5fd74-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="5fd74-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="5fd74-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fd74-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5fd74-108">Attributes and elements</span></span>

<span data-ttu-id="5fd74-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5fd74-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fd74-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5fd74-110">Attributes</span></span>

|<span data-ttu-id="5fd74-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5fd74-111">**Attribute**</span></span>|<span data-ttu-id="5fd74-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5fd74-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5fd74-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="5fd74-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="5fd74-114">Указывает, следует ли подписка на всех доступных папок.</span><span class="sxs-lookup"><span data-stu-id="5fd74-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="5fd74-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="5fd74-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5fd74-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5fd74-116">Child elements</span></span>

|<span data-ttu-id="5fd74-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5fd74-117">**Element**</span></span>|<span data-ttu-id="5fd74-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5fd74-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fd74-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="5fd74-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="5fd74-120">Содержит массив идентификаторов папок, которые используются для определения папок для наблюдения за уведомления о событиях.</span><span class="sxs-lookup"><span data-stu-id="5fd74-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="5fd74-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="5fd74-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="5fd74-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="5fd74-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="5fd74-123">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="5fd74-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="5fd74-124">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5fd74-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="5fd74-125">Используется для создания подписки, начиная с события, представленного водяного знака.</span><span class="sxs-lookup"><span data-stu-id="5fd74-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="5fd74-126">Если водяного знака из подписки на запрос не найден, возврату ошибки будут возвращены клиенту.</span><span class="sxs-lookup"><span data-stu-id="5fd74-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="5fd74-127">Это может произойти, если водяной знак старше 30 дней или если водяного знака никогда не был указан в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5fd74-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5fd74-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="5fd74-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="5fd74-129">Представляет частоту, в минутах, в какой уведомлении сообщения будут отправляться клиенту возникновения события не.</span><span class="sxs-lookup"><span data-stu-id="5fd74-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="5fd74-130">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="5fd74-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5fd74-131">Представляет расположение клиента веб-службы push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5fd74-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fd74-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5fd74-132">Parent elements</span></span>

|<span data-ttu-id="5fd74-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5fd74-133">**Element**</span></span>|<span data-ttu-id="5fd74-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5fd74-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fd74-135">Подписка</span><span class="sxs-lookup"><span data-stu-id="5fd74-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="5fd74-136">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="5fd74-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5fd74-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5fd74-137">Text value</span></span>

<span data-ttu-id="5fd74-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fd74-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5fd74-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="5fd74-139">Remarks</span></span>

<span data-ttu-id="5fd74-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fd74-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fd74-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5fd74-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fd74-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5fd74-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5fd74-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5fd74-143">Schema name</span></span>  <br/> |<span data-ttu-id="5fd74-144">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5fd74-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5fd74-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5fd74-145">Validation file</span></span>  <br/> |<span data-ttu-id="5fd74-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5fd74-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5fd74-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5fd74-147">Can be empty</span></span>  <br/> |<span data-ttu-id="5fd74-148">False</span><span class="sxs-lookup"><span data-stu-id="5fd74-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fd74-149">См. также</span><span class="sxs-lookup"><span data-stu-id="5fd74-149">See also</span></span>



[<span data-ttu-id="5fd74-150">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="5fd74-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5fd74-151">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="5fd74-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5fd74-152">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="5fd74-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

