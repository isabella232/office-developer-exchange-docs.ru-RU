---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: Элемент ConvertIdResponseMessage содержит состояние и результат операции запроса ConvertId.
ms.openlocfilehash: 6668c0b3254191ca628413bae5ff957c3cb95b5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761837"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="d36b6-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d36b6-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="d36b6-104">Элемент **ConvertIdResponseMessage** содержит состояние и результат [операции ConvertId](convertid-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="d36b6-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d36b6-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="d36b6-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="d36b6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d36b6-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d36b6-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d36b6-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="d36b6-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d36b6-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d36b6-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d36b6-109">Attributes and elements</span></span>

<span data-ttu-id="d36b6-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d36b6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d36b6-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d36b6-111">Attributes</span></span>

|<span data-ttu-id="d36b6-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d36b6-112">**Attribute**</span></span>|<span data-ttu-id="d36b6-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d36b6-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d36b6-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d36b6-115">Описание состояния ответа [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d36b6-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="d36b6-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d36b6-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="d36b6-117">-Success</span><span class="sxs-lookup"><span data-stu-id="d36b6-117">- Success</span></span>  <br/><span data-ttu-id="d36b6-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d36b6-118">-  Warning</span></span>  <br/><span data-ttu-id="d36b6-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d36b6-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d36b6-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d36b6-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d36b6-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d36b6-121">**Value**</span></span>|<span data-ttu-id="d36b6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b6-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d36b6-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="d36b6-123">**Success**</span></span> <br/> |<span data-ttu-id="d36b6-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d36b6-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d36b6-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="d36b6-125">**Warning**</span></span> <br/> | <span data-ttu-id="d36b6-126">Описание запроса, который не был полностью обработан или для которого произошло непредвиденные результаты.</span><span class="sxs-lookup"><span data-stu-id="d36b6-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="d36b6-127">**Error**</span><span class="sxs-lookup"><span data-stu-id="d36b6-127">**Error**</span></span> <br/> | <span data-ttu-id="d36b6-128">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d36b6-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="d36b6-129">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d36b6-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d36b6-130">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d36b6-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d36b6-131">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d36b6-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d36b6-132">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d36b6-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="d36b6-133">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d36b6-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d36b6-134">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="d36b6-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d36b6-135">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d36b6-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="d36b6-136">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d36b6-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d36b6-137">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d36b6-137">Child elements</span></span>

|<span data-ttu-id="d36b6-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d36b6-138">**Element**</span></span>|<span data-ttu-id="d36b6-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b6-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d36b6-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="d36b6-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d36b6-141">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d36b6-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d36b6-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d36b6-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d36b6-143">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d36b6-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d36b6-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d36b6-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d36b6-145">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d36b6-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d36b6-146">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d36b6-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d36b6-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d36b6-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d36b6-148">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d36b6-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d36b6-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="d36b6-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="d36b6-150">Описывает преобразованные идентификатор в ответе.</span><span class="sxs-lookup"><span data-stu-id="d36b6-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d36b6-151">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d36b6-151">Parent elements</span></span>

|<span data-ttu-id="d36b6-152">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d36b6-152">**Element**</span></span>|<span data-ttu-id="d36b6-153">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b6-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d36b6-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d36b6-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d36b6-155">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d36b6-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d36b6-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="d36b6-156">Remarks</span></span>

<span data-ttu-id="d36b6-157">Возвращается одно сообщение ответа каждого преобразованные идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d36b6-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="d36b6-158">Элемент [AlternateId](alternateid.md) будет отсутствовать из ответа Если возвращает код ошибки</span><span class="sxs-lookup"><span data-stu-id="d36b6-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="d36b6-159">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="d36b6-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d36b6-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d36b6-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d36b6-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d36b6-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d36b6-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d36b6-162">Schema Name</span></span>  <br/> |<span data-ttu-id="d36b6-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d36b6-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d36b6-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d36b6-164">Validation File</span></span>  <br/> |<span data-ttu-id="d36b6-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d36b6-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d36b6-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d36b6-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="d36b6-167">False</span><span class="sxs-lookup"><span data-stu-id="d36b6-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d36b6-168">См. также</span><span class="sxs-lookup"><span data-stu-id="d36b6-168">See also</span></span>

- [<span data-ttu-id="d36b6-169">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="d36b6-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="d36b6-170">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d36b6-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

