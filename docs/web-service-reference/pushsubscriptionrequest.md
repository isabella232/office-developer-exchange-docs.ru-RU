---
title: пушсубскриптионрекуест
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
description: Элемент Пушсубскриптионрекуест представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465515"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="450cd-103">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="450cd-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="450cd-104">Элемент **пушсубскриптионрекуест** представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="450cd-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="450cd-105">Подписаться</span><span class="sxs-lookup"><span data-stu-id="450cd-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="450cd-106">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="450cd-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="450cd-107">**пушсубскриптионрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="450cd-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="450cd-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="450cd-108">Attributes and elements</span></span>

<span data-ttu-id="450cd-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="450cd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="450cd-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="450cd-110">Attributes</span></span>

|<span data-ttu-id="450cd-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="450cd-111">**Attribute**</span></span>|<span data-ttu-id="450cd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="450cd-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="450cd-113">**субскрибетоаллфолдерс**</span><span class="sxs-lookup"><span data-stu-id="450cd-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="450cd-114">Указывает, следует ли подписываться на все доступные папки.</span><span class="sxs-lookup"><span data-stu-id="450cd-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="450cd-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="450cd-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="450cd-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="450cd-116">Child elements</span></span>

|<span data-ttu-id="450cd-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="450cd-117">**Element**</span></span>|<span data-ttu-id="450cd-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="450cd-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="450cd-119">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="450cd-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="450cd-120">Содержит массив идентификаторов папок, которые используются для определения папок, которые необходимо отслеживать для получения уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="450cd-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="450cd-121">евенттипес</span><span class="sxs-lookup"><span data-stu-id="450cd-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="450cd-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="450cd-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="450cd-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="450cd-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="450cd-124">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="450cd-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="450cd-125">Используется для создания подписки, начиная с события, представленного водяным знаком.</span><span class="sxs-lookup"><span data-stu-id="450cd-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="450cd-126">Если водяной знак из запроса на подписку не найден, клиенту будет возвращен ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="450cd-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="450cd-127">Это может произойти, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="450cd-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="450cd-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="450cd-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="450cd-129">Представляет частоту, заданную в минутах, с которой сообщения уведомлений будут отправляться клиенту при отсутствии событий.</span><span class="sxs-lookup"><span data-stu-id="450cd-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="450cd-130">Адрес</span><span class="sxs-lookup"><span data-stu-id="450cd-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="450cd-131">Представляет расположение клиентской веб-службы для push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="450cd-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="450cd-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="450cd-132">Parent elements</span></span>

|<span data-ttu-id="450cd-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="450cd-133">**Element**</span></span>|<span data-ttu-id="450cd-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="450cd-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="450cd-135">Подписаться</span><span class="sxs-lookup"><span data-stu-id="450cd-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="450cd-136">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="450cd-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="450cd-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="450cd-137">Text value</span></span>

<span data-ttu-id="450cd-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="450cd-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="450cd-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="450cd-139">Remarks</span></span>

<span data-ttu-id="450cd-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="450cd-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="450cd-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="450cd-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="450cd-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="450cd-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="450cd-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="450cd-143">Schema name</span></span>  <br/> |<span data-ttu-id="450cd-144">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="450cd-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="450cd-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="450cd-145">Validation file</span></span>  <br/> |<span data-ttu-id="450cd-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="450cd-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="450cd-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="450cd-147">Can be empty</span></span>  <br/> |<span data-ttu-id="450cd-148">False</span><span class="sxs-lookup"><span data-stu-id="450cd-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="450cd-149">См. также</span><span class="sxs-lookup"><span data-stu-id="450cd-149">See also</span></span>



[<span data-ttu-id="450cd-150">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="450cd-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="450cd-151">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="450cd-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="450cd-152">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="450cd-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

