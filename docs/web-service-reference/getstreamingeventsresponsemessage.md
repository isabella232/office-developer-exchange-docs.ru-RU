---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: Элемент GetStreamingEventsResponseMessage содержит состояние и результат одного запроса GetStreamingEvents операции.
ms.openlocfilehash: 5fcc7ddde41b49a5d8b304da0732f4472c61a76a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833682"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="be07b-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="be07b-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="be07b-104">Элемент **GetStreamingEventsResponseMessage** содержит состояние и результат одного запроса [GetStreamingEvents операции](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="be07b-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 <span data-ttu-id="be07b-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="be07b-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be07b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="be07b-106">Attributes and elements</span></span>

<span data-ttu-id="be07b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="be07b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be07b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="be07b-108">Attributes</span></span>

|<span data-ttu-id="be07b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="be07b-109">**Attribute**</span></span>|<span data-ttu-id="be07b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be07b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be07b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="be07b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="be07b-112">Описание состояния ответа [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="be07b-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="be07b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="be07b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="be07b-114">-Success</span><span class="sxs-lookup"><span data-stu-id="be07b-114">-  Success</span></span>  <br/><span data-ttu-id="be07b-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="be07b-115">-  Warning</span></span>  <br/><span data-ttu-id="be07b-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="be07b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="be07b-117">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="be07b-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="be07b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="be07b-118">**Value**</span></span>|<span data-ttu-id="be07b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be07b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be07b-120">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="be07b-120">Success</span></span>  <br/> |<span data-ttu-id="be07b-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="be07b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="be07b-122">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="be07b-122">Warning</span></span>  <br/> | <span data-ttu-id="be07b-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="be07b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="be07b-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="be07b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="be07b-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="be07b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="be07b-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="be07b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="be07b-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="be07b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="be07b-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="be07b-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="be07b-129">-Базы данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="be07b-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="be07b-130">-Истек срок действия пароль.</span><span class="sxs-lookup"><span data-stu-id="be07b-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="be07b-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="be07b-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="be07b-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="be07b-132">Error</span></span>  <br/> | <span data-ttu-id="be07b-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="be07b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="be07b-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="be07b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="be07b-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="be07b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="be07b-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="be07b-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="be07b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="be07b-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="be07b-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="be07b-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="be07b-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="be07b-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="be07b-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="be07b-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="be07b-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="be07b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be07b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="be07b-142">Child elements</span></span>

|<span data-ttu-id="be07b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be07b-143">**Element**</span></span>|<span data-ttu-id="be07b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be07b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be07b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="be07b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="be07b-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="be07b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="be07b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="be07b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="be07b-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="be07b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="be07b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="be07b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="be07b-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="be07b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="be07b-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="be07b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="be07b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="be07b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="be07b-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="be07b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="be07b-154">Уведомления</span><span class="sxs-lookup"><span data-stu-id="be07b-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="be07b-155">Содержит список, содержащий сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="be07b-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="be07b-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="be07b-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="be07b-157">Содержит список идентификаторов, которые являются недопустимыми подписок.</span><span class="sxs-lookup"><span data-stu-id="be07b-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="be07b-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="be07b-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="be07b-159">Предоставляет текстовое описание состояния потоковой передачи подписки.</span><span class="sxs-lookup"><span data-stu-id="be07b-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be07b-160">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="be07b-160">Parent elements</span></span>

|<span data-ttu-id="be07b-161">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be07b-161">**Element**</span></span>|<span data-ttu-id="be07b-162">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be07b-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be07b-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="be07b-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="be07b-164">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="be07b-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be07b-165">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="be07b-165">Text value</span></span>

<span data-ttu-id="be07b-166">Нет.</span><span class="sxs-lookup"><span data-stu-id="be07b-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be07b-167">Замечания</span><span class="sxs-lookup"><span data-stu-id="be07b-167">Remarks</span></span>

<span data-ttu-id="be07b-168">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="be07b-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be07b-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="be07b-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be07b-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="be07b-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be07b-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="be07b-171">Schema Name</span></span>  <br/> |<span data-ttu-id="be07b-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="be07b-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="be07b-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="be07b-173">Validation File</span></span>  <br/> |<span data-ttu-id="be07b-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="be07b-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be07b-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="be07b-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="be07b-176">False</span><span class="sxs-lookup"><span data-stu-id="be07b-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be07b-177">См. также</span><span class="sxs-lookup"><span data-stu-id="be07b-177">See also</span></span>

- [<span data-ttu-id="be07b-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="be07b-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="be07b-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="be07b-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="be07b-180">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="be07b-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

