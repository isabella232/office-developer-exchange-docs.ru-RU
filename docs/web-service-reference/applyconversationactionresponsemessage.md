---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: Элемент ApplyConversationActionResponseMessage содержит состояние и результаты запроса операции ApplyConversationAction.
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761472"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="ef9b1-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef9b1-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="ef9b1-104">Элемент **ApplyConversationActionResponseMessage** содержит состояние и результаты запроса [ApplyConversationAction операции](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ef9b1-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="ef9b1-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="ef9b1-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="ef9b1-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef9b1-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ef9b1-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef9b1-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="ef9b1-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef9b1-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ef9b1-109">Attributes and elements</span></span>

<span data-ttu-id="ef9b1-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef9b1-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ef9b1-111">Attributes</span></span>

|<span data-ttu-id="ef9b1-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-112">**Attribute**</span></span>|<span data-ttu-id="ef9b1-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef9b1-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ef9b1-115">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="ef9b1-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ef9b1-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="ef9b1-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="ef9b1-117">Success</span></span></li><li><span data-ttu-id="ef9b1-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="ef9b1-118">Warning</span></span></li><li><span data-ttu-id="ef9b1-119">Error</span><span class="sxs-lookup"><span data-stu-id="ef9b1-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ef9b1-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ef9b1-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="ef9b1-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-121">**Value**</span></span>|<span data-ttu-id="ef9b1-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef9b1-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-123">**Success**</span></span> <br/> |<span data-ttu-id="ef9b1-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ef9b1-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-125">**Warning**</span></span> <br/> | <span data-ttu-id="ef9b1-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ef9b1-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="ef9b1-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="ef9b1-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="ef9b1-129">Во время пакет недоступен в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="ef9b1-130">Доменных служб Active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="ef9b1-131">Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="ef9b1-132">База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="ef9b1-133">Истек срок действия пароля.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-133">A password is expired.</span></span></li><li><span data-ttu-id="ef9b1-134">Квота превышена.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="ef9b1-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-135">**Error**</span></span> <br/> | <span data-ttu-id="ef9b1-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="ef9b1-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="ef9b1-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="ef9b1-138">Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ef9b1-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="ef9b1-139">Атрибуты и элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="ef9b1-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="ef9b1-140">Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="ef9b1-140">An unknown tag</span></span>  </li><li><span data-ttu-id="ef9b1-141">Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="ef9b1-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="ef9b1-142">Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="ef9b1-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="ef9b1-143">Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="ef9b1-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="ef9b1-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef9b1-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ef9b1-145">Child elements</span></span>

|<span data-ttu-id="ef9b1-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-146">**Element**</span></span>|<span data-ttu-id="ef9b1-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef9b1-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ef9b1-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ef9b1-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ef9b1-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ef9b1-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ef9b1-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ef9b1-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ef9b1-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ef9b1-153">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="ef9b1-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ef9b1-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ef9b1-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ef9b1-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef9b1-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ef9b1-157">Parent elements</span></span>

|<span data-ttu-id="ef9b1-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-158">**Element**</span></span>|<span data-ttu-id="ef9b1-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef9b1-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef9b1-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef9b1-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ef9b1-161">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef9b1-162">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ef9b1-162">Text value</span></span>

<span data-ttu-id="ef9b1-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ef9b1-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef9b1-164">Remarks</span></span>

<span data-ttu-id="ef9b1-165">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ef9b1-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="ef9b1-166">Различия версий</span><span class="sxs-lookup"><span data-stu-id="ef9b1-166">Version differences</span></span>

<span data-ttu-id="ef9b1-167">В версиях Exchange, начиная с построения 15.00.0986.00 **ApplyConversationActionResponseMessage** элемент имеет тип **ApplyConversationActionResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="ef9b1-168">В предыдущих версиях элемент имеет тип **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="ef9b1-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef9b1-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ef9b1-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef9b1-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ef9b1-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef9b1-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ef9b1-171">Schema Name</span></span>  <br/> |<span data-ttu-id="ef9b1-172">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="ef9b1-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="ef9b1-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ef9b1-173">Validation File</span></span>  <br/> |<span data-ttu-id="ef9b1-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ef9b1-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef9b1-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ef9b1-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef9b1-176">False</span><span class="sxs-lookup"><span data-stu-id="ef9b1-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef9b1-177">См. также</span><span class="sxs-lookup"><span data-stu-id="ef9b1-177">See also</span></span>

- [<span data-ttu-id="ef9b1-178">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ef9b1-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="ef9b1-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ef9b1-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

