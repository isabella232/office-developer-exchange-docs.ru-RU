---
title: FindConversationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversationResponse
api_type:
- schema
ms.assetid: a689e29d-5f3d-4deb-81ee-8b6cc60f6dea
description: Элемент FindConversationResponse определяет ответ на запрос операции FindConversation.
ms.openlocfilehash: 5754ea7540fa6daac8cd725386ca213d5bf05c8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762557"
---
# <a name="findconversationresponse"></a><span data-ttu-id="3d723-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="3d723-103">FindConversationResponse</span></span>

<span data-ttu-id="3d723-104">Элемент **FindConversationResponse** определяет ответ на запрос [FindConversation операции](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3d723-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="3d723-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="3d723-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="3d723-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3d723-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d723-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3d723-107">Attributes and elements</span></span>

<span data-ttu-id="3d723-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3d723-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d723-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3d723-109">Attributes</span></span>

|<span data-ttu-id="3d723-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3d723-110">**Attribute**</span></span>|<span data-ttu-id="3d723-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d723-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d723-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3d723-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3d723-113">Описание состояния ответа [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3d723-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="3d723-114">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3d723-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="3d723-115">-Success</span><span class="sxs-lookup"><span data-stu-id="3d723-115">-  Success</span></span>  <br/><span data-ttu-id="3d723-116">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="3d723-116">-  Warning</span></span>  <br/><span data-ttu-id="3d723-117">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="3d723-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3d723-118">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3d723-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="3d723-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3d723-119">**Value**</span></span>|<span data-ttu-id="3d723-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d723-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d723-121">**Успех**</span><span class="sxs-lookup"><span data-stu-id="3d723-121">**Success**</span></span> <br/> |<span data-ttu-id="3d723-122">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="3d723-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3d723-123">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="3d723-123">**Warning**</span></span> <br/> | <span data-ttu-id="3d723-124">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="3d723-124">Describes a request that was not processed.</span></span> <span data-ttu-id="3d723-125">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="3d723-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="3d723-126">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="3d723-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3d723-127">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="3d723-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3d723-128">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3d723-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3d723-129">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="3d723-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="3d723-130">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3d723-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3d723-131">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="3d723-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="3d723-132">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="3d723-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="3d723-133">**Error**</span><span class="sxs-lookup"><span data-stu-id="3d723-133">**Error**</span></span> <br/> | <span data-ttu-id="3d723-134">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="3d723-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3d723-135">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="3d723-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3d723-136">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3d723-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3d723-137">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="3d723-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="3d723-138">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="3d723-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="3d723-139">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="3d723-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="3d723-140">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="3d723-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3d723-141">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="3d723-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3d723-142">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="3d723-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3d723-143">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3d723-143">Child elements</span></span>

|<span data-ttu-id="3d723-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d723-144">**Element**</span></span>|<span data-ttu-id="3d723-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d723-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d723-146">Conversations</span><span class="sxs-lookup"><span data-stu-id="3d723-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3d723-147">Содержит массив бесед.</span><span class="sxs-lookup"><span data-stu-id="3d723-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="3d723-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="3d723-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3d723-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="3d723-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3d723-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3d723-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3d723-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="3d723-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3d723-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3d723-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3d723-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="3d723-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3d723-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3d723-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3d723-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3d723-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3d723-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="3d723-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d723-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3d723-157">Parent elements</span></span>

<span data-ttu-id="3d723-158">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d723-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3d723-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3d723-159">Text value</span></span>

<span data-ttu-id="3d723-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d723-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3d723-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="3d723-161">Remarks</span></span>

<span data-ttu-id="3d723-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3d723-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d723-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3d723-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d723-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3d723-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3d723-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3d723-165">Schema name</span></span>  <br/> |<span data-ttu-id="3d723-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3d723-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3d723-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3d723-167">Validation file</span></span>  <br/> |<span data-ttu-id="3d723-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3d723-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d723-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3d723-169">Can be empty</span></span>  <br/> |<span data-ttu-id="3d723-170">False</span><span class="sxs-lookup"><span data-stu-id="3d723-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d723-171">См. также</span><span class="sxs-lookup"><span data-stu-id="3d723-171">See also</span></span>

- [<span data-ttu-id="3d723-172">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="3d723-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="3d723-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d723-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3d723-174">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="3d723-174">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

