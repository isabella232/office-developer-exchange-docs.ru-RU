---
title: субскрибереспонсемессаже
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
description: Элемент Субскрибереспонсемессаже содержит состояние и результат запроса на операцию одиночной подписки.
ms.openlocfilehash: 97c7bd9f12511ff226e75f53278c13481679c8a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="bf169-103">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bf169-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="bf169-104">Элемент **субскрибереспонсемессаже** содержит состояние и результат запроса на операцию одиночной [подписки](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bf169-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="bf169-105">субскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="bf169-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="bf169-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bf169-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="bf169-107">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bf169-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="bf169-108">**субскрибереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="bf169-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf169-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf169-109">Attributes and elements</span></span>

<span data-ttu-id="bf169-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bf169-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf169-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf169-111">Attributes</span></span>

|<span data-ttu-id="bf169-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bf169-112">**Attribute**</span></span>|<span data-ttu-id="bf169-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf169-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf169-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="bf169-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bf169-115">Описывает состояние ответа [операции подписки](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bf169-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="bf169-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bf169-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="bf169-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="bf169-117">-  Success</span></span>  <br/><span data-ttu-id="bf169-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bf169-118">-  Warning</span></span>  <br/><span data-ttu-id="bf169-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="bf169-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bf169-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="bf169-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bf169-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bf169-121">**Value**</span></span>|<span data-ttu-id="bf169-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf169-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf169-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="bf169-123">**Success**</span></span> <br/> |<span data-ttu-id="bf169-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="bf169-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bf169-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="bf169-125">**Warning**</span></span> <br/> | <span data-ttu-id="bf169-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bf169-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bf169-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="bf169-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="bf169-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="bf169-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="bf169-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="bf169-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bf169-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bf169-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bf169-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="bf169-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bf169-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bf169-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bf169-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="bf169-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bf169-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="bf169-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bf169-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="bf169-135">**Error**</span></span> <br/> | <span data-ttu-id="bf169-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bf169-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bf169-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="bf169-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bf169-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="bf169-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bf169-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="bf169-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="bf169-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bf169-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="bf169-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="bf169-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="bf169-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="bf169-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bf169-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="bf169-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="bf169-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bf169-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bf169-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf169-145">Child elements</span></span>

|<span data-ttu-id="bf169-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf169-146">**Element**</span></span>|<span data-ttu-id="bf169-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf169-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf169-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bf169-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bf169-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="bf169-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bf169-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bf169-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bf169-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="bf169-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bf169-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bf169-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bf169-153">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bf169-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bf169-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bf169-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bf169-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="bf169-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bf169-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bf169-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bf169-157">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="bf169-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="bf169-158">Представляет идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="bf169-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="bf169-159">Watermark</span><span class="sxs-lookup"><span data-stu-id="bf169-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="bf169-160">Представляет закладку события в очереди событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf169-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf169-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf169-161">Parent elements</span></span>

|<span data-ttu-id="bf169-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf169-162">**Element**</span></span>|<span data-ttu-id="bf169-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf169-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf169-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bf169-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bf169-165">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf169-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf169-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="bf169-166">Remarks</span></span>

<span data-ttu-id="bf169-167">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bf169-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf169-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf169-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf169-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf169-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bf169-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf169-170">Schema Name</span></span>  <br/> |<span data-ttu-id="bf169-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bf169-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bf169-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf169-172">Validation File</span></span>  <br/> |<span data-ttu-id="bf169-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bf169-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bf169-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf169-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf169-175">False</span><span class="sxs-lookup"><span data-stu-id="bf169-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf169-176">См. также</span><span class="sxs-lookup"><span data-stu-id="bf169-176">See also</span></span>

- [<span data-ttu-id="bf169-177">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="bf169-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="bf169-178">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="bf169-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="bf169-179">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="bf169-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

