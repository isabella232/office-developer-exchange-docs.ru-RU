---
title: StreamingSubscriptionRequest
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
description: Элемент StreamingSubscriptionRequest — подписка на подписку на уведомления о потоковой передачи событий.
ms.openlocfilehash: 088ec3b8048d70803b4837548ca918c0005d91bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835601"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="22074-103">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="22074-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="22074-104">Элемент **StreamingSubscriptionRequest** — подписка на подписку на уведомления о потоковой передачи событий.</span><span class="sxs-lookup"><span data-stu-id="22074-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="22074-105">Подписка</span><span class="sxs-lookup"><span data-stu-id="22074-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="22074-106">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="22074-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="22074-107">**StreamingSubscriptionRequest**</span><span class="sxs-lookup"><span data-stu-id="22074-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22074-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22074-108">Attributes and elements</span></span>

<span data-ttu-id="22074-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="22074-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22074-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22074-110">Attributes</span></span>

|<span data-ttu-id="22074-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="22074-111">**Attribute**</span></span>|<span data-ttu-id="22074-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22074-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22074-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="22074-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="22074-114">Указывает, будет ли сервер будет создана подписка на всех папок в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="22074-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="22074-115">Значение **true** указывает, что сервер будет создана подписка.</span><span class="sxs-lookup"><span data-stu-id="22074-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22074-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22074-116">Child elements</span></span>

|<span data-ttu-id="22074-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22074-117">**Element**</span></span>|<span data-ttu-id="22074-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22074-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22074-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="22074-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="22074-120">Содержит массив идентификаторов папок, которые используются для определения папок для наблюдения за уведомления о событиях.</span><span class="sxs-lookup"><span data-stu-id="22074-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="22074-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="22074-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="22074-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="22074-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22074-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22074-123">Parent elements</span></span>

|<span data-ttu-id="22074-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22074-124">**Element**</span></span>|<span data-ttu-id="22074-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22074-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22074-126">Подписка</span><span class="sxs-lookup"><span data-stu-id="22074-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="22074-127">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="22074-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22074-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="22074-128">Text value</span></span>

<span data-ttu-id="22074-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="22074-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22074-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="22074-130">Remarks</span></span>

<span data-ttu-id="22074-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="22074-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22074-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22074-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22074-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22074-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22074-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22074-134">Schema name</span></span>  <br/> |<span data-ttu-id="22074-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="22074-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22074-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22074-136">Validation file</span></span>  <br/> |<span data-ttu-id="22074-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22074-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22074-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22074-138">Can be empty</span></span>  <br/> |<span data-ttu-id="22074-139">False</span><span class="sxs-lookup"><span data-stu-id="22074-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22074-140">См. также</span><span class="sxs-lookup"><span data-stu-id="22074-140">See also</span></span>



[<span data-ttu-id="22074-141">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="22074-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="22074-142">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="22074-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="22074-143">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="22074-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="22074-144">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="22074-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

