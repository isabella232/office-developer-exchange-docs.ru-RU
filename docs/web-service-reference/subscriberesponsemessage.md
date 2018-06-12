---
title: SubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponseMessage
api_type:
- schema
ms.assetid: d121d38a-a61a-4f9c-a477-fc6d7f9af77e
description: Элемент SubscribeResponseMessage содержит состояние и результат одного запроса подписки на операции.
ms.openlocfilehash: 97c7bd9f12511ff226e75f53278c13481679c8a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="886f2-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="886f2-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="886f2-104">Элемент **SubscribeResponseMessage** содержит состояние и результат одной [подписки на операции](subscribe-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="886f2-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="886f2-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="886f2-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="886f2-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="886f2-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="886f2-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="886f2-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
```xml
<SubscribeResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SubscriptionId/>
   <Watermark/>
</SubscribeResponseMessage>
```

 <span data-ttu-id="886f2-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="886f2-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="886f2-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="886f2-109">Attributes and elements</span></span>

<span data-ttu-id="886f2-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="886f2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="886f2-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="886f2-111">Attributes</span></span>

|<span data-ttu-id="886f2-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="886f2-112">**Attribute**</span></span>|<span data-ttu-id="886f2-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="886f2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="886f2-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="886f2-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="886f2-115">Описание состояния ответа [подписки на операции](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="886f2-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="886f2-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="886f2-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="886f2-117">-Success</span><span class="sxs-lookup"><span data-stu-id="886f2-117">-  Success</span></span>  <br/><span data-ttu-id="886f2-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="886f2-118">-  Warning</span></span>  <br/><span data-ttu-id="886f2-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="886f2-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="886f2-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="886f2-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="886f2-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="886f2-121">**Value**</span></span>|<span data-ttu-id="886f2-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="886f2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="886f2-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="886f2-123">**Success**</span></span> <br/> |<span data-ttu-id="886f2-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="886f2-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="886f2-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="886f2-125">**Warning**</span></span> <br/> | <span data-ttu-id="886f2-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="886f2-126">Describes a request that was not processed.</span></span> <span data-ttu-id="886f2-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="886f2-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="886f2-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="886f2-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="886f2-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="886f2-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="886f2-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="886f2-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="886f2-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="886f2-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="886f2-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="886f2-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="886f2-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="886f2-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="886f2-134">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="886f2-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="886f2-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="886f2-135">**Error**</span></span> <br/> | <span data-ttu-id="886f2-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="886f2-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="886f2-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="886f2-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="886f2-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="886f2-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="886f2-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="886f2-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="886f2-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="886f2-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="886f2-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="886f2-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="886f2-142">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="886f2-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="886f2-143">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="886f2-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="886f2-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="886f2-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="886f2-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="886f2-145">Child elements</span></span>

|<span data-ttu-id="886f2-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="886f2-146">**Element**</span></span>|<span data-ttu-id="886f2-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="886f2-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="886f2-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="886f2-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="886f2-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="886f2-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="886f2-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="886f2-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="886f2-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="886f2-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="886f2-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="886f2-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="886f2-153">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="886f2-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="886f2-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="886f2-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="886f2-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="886f2-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="886f2-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="886f2-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="886f2-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="886f2-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="886f2-158">Представляет идентификатор для подписки.</span><span class="sxs-lookup"><span data-stu-id="886f2-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="886f2-159">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="886f2-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="886f2-160">Представляет закладку события в очереди событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="886f2-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="886f2-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="886f2-161">Parent elements</span></span>

|<span data-ttu-id="886f2-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="886f2-162">**Element**</span></span>|<span data-ttu-id="886f2-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="886f2-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="886f2-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="886f2-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="886f2-165">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="886f2-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="886f2-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="886f2-166">Remarks</span></span>

<span data-ttu-id="886f2-167">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="886f2-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="886f2-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="886f2-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="886f2-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="886f2-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="886f2-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="886f2-170">Schema Name</span></span>  <br/> |<span data-ttu-id="886f2-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="886f2-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="886f2-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="886f2-172">Validation File</span></span>  <br/> |<span data-ttu-id="886f2-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="886f2-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="886f2-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="886f2-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="886f2-175">False</span><span class="sxs-lookup"><span data-stu-id="886f2-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="886f2-176">См. также</span><span class="sxs-lookup"><span data-stu-id="886f2-176">See also</span></span>

- [<span data-ttu-id="886f2-177">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="886f2-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="886f2-178">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="886f2-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="886f2-179">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="886f2-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

