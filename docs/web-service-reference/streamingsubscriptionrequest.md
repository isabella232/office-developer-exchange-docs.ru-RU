---
title: стреамингсубскриптионрекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: Элемент Стреамингсубскриптионрекуест представляет подписку на подписку на уведомление о событии потоковой передачи.
ms.openlocfilehash: b469ba7598420189c1db0e2fe676a279390eb6bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468231"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="543be-103">стреамингсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="543be-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="543be-104">Элемент **стреамингсубскриптионрекуест** представляет подписку на подписку на уведомление о событии потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="543be-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="543be-105">Подписаться</span><span class="sxs-lookup"><span data-stu-id="543be-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="543be-106">стреамингсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="543be-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="543be-107">**стреамингсубскриптионрекуест**</span><span class="sxs-lookup"><span data-stu-id="543be-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="543be-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="543be-108">Attributes and elements</span></span>

<span data-ttu-id="543be-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="543be-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="543be-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="543be-110">Attributes</span></span>

|<span data-ttu-id="543be-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="543be-111">**Attribute**</span></span>|<span data-ttu-id="543be-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="543be-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="543be-113">**субскрибетоаллфолдерс**</span><span class="sxs-lookup"><span data-stu-id="543be-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="543be-114">Указывает, будет ли сервер подписываться на все папки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="543be-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="543be-115">Значение **true** указывает на то, что сервер будет подписываться.</span><span class="sxs-lookup"><span data-stu-id="543be-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="543be-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="543be-116">Child elements</span></span>

|<span data-ttu-id="543be-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="543be-117">**Element**</span></span>|<span data-ttu-id="543be-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="543be-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="543be-119">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="543be-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="543be-120">Содержит массив идентификаторов папок, которые используются для определения папок, которые необходимо отслеживать для получения уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="543be-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="543be-121">евенттипес</span><span class="sxs-lookup"><span data-stu-id="543be-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="543be-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="543be-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="543be-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="543be-123">Parent elements</span></span>

|<span data-ttu-id="543be-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="543be-124">**Element**</span></span>|<span data-ttu-id="543be-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="543be-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="543be-126">Подписаться</span><span class="sxs-lookup"><span data-stu-id="543be-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="543be-127">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="543be-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="543be-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="543be-128">Text value</span></span>

<span data-ttu-id="543be-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="543be-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="543be-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="543be-130">Remarks</span></span>

<span data-ttu-id="543be-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="543be-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="543be-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="543be-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="543be-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="543be-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="543be-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="543be-134">Schema name</span></span>  <br/> |<span data-ttu-id="543be-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="543be-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="543be-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="543be-136">Validation file</span></span>  <br/> |<span data-ttu-id="543be-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="543be-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="543be-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="543be-138">Can be empty</span></span>  <br/> |<span data-ttu-id="543be-139">False</span><span class="sxs-lookup"><span data-stu-id="543be-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="543be-140">См. также</span><span class="sxs-lookup"><span data-stu-id="543be-140">See also</span></span>



[<span data-ttu-id="543be-141">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="543be-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="543be-142">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="543be-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="543be-143">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="543be-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="543be-144">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="543be-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

