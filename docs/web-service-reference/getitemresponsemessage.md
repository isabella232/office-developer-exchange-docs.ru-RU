---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: Элемент GetItemResponseMessage содержит состояние и результат одного запроса операции GetItem.
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762842"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="bb466-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bb466-103">GetItemResponseMessage</span></span>

<span data-ttu-id="bb466-104">Элемент **GetItemResponseMessage** содержит состояние и результат одной [операции GetItem](getitem-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="bb466-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="bb466-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="bb466-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="bb466-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bb466-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="bb466-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bb466-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="bb466-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bb466-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bb466-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bb466-109">Attributes and elements</span></span>

<span data-ttu-id="bb466-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bb466-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb466-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bb466-111">Attributes</span></span>

|<span data-ttu-id="bb466-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bb466-112">**Attribute**</span></span>|<span data-ttu-id="bb466-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb466-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bb466-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bb466-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bb466-115">Описание состояния ответа [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb466-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="bb466-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bb466-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="bb466-117">-Success</span><span class="sxs-lookup"><span data-stu-id="bb466-117">- Success</span></span><br/><span data-ttu-id="bb466-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bb466-118">- Warning</span></span><br/><span data-ttu-id="bb466-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="bb466-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bb466-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bb466-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bb466-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bb466-121">**Value**</span></span>|<span data-ttu-id="bb466-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb466-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bb466-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="bb466-123">**Success**</span></span> <br/> |<span data-ttu-id="bb466-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="bb466-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bb466-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="bb466-125">**Warning**</span></span> <br/> | <span data-ttu-id="bb466-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bb466-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bb466-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="bb466-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="bb466-128">Ниже приведены примеры источников для предупреждения:</span><span class="sxs-lookup"><span data-stu-id="bb466-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="bb466-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="bb466-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="bb466-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bb466-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="bb466-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="bb466-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="bb466-132">-MDB находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bb466-132">- MDB is offline.</span></span><br/><span data-ttu-id="bb466-133">-Истек срок действия пароля.</span><span class="sxs-lookup"><span data-stu-id="bb466-133">- Password is expired.</span></span>  <br/><span data-ttu-id="bb466-134">-Квота превышена.</span><span class="sxs-lookup"><span data-stu-id="bb466-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="bb466-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="bb466-135">**Error**</span></span> <br/> | <span data-ttu-id="bb466-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bb466-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="bb466-137">Ниже приведены примеры источников для ошибки:</span><span class="sxs-lookup"><span data-stu-id="bb466-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="bb466-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bb466-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="bb466-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="bb466-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="bb466-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bb466-140">- Unknown tag</span></span><br/><span data-ttu-id="bb466-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="bb466-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="bb466-142">-Предпринята попытка любой клиент несанкционированного доступа</span><span class="sxs-lookup"><span data-stu-id="bb466-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="bb466-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="bb466-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="bb466-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="bb466-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="bb466-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bb466-145">Child elements</span></span>

|<span data-ttu-id="bb466-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bb466-146">**Element**</span></span>|<span data-ttu-id="bb466-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb466-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb466-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="bb466-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bb466-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="bb466-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bb466-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bb466-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bb466-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="bb466-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bb466-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bb466-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bb466-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bb466-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bb466-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bb466-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bb466-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bb466-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bb466-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="bb466-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bb466-157">Элементы</span><span class="sxs-lookup"><span data-stu-id="bb466-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="bb466-158">Содержит массив возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="bb466-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb466-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bb466-159">Parent elements</span></span>

|<span data-ttu-id="bb466-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bb466-160">**Element**</span></span>|<span data-ttu-id="bb466-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb466-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb466-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bb466-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bb466-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb466-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bb466-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="bb466-164">Remarks</span></span>

<span data-ttu-id="bb466-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bb466-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb466-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bb466-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb466-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bb466-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb466-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bb466-168">Schema Name</span></span>  <br/> |<span data-ttu-id="bb466-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bb466-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb466-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bb466-170">Validation File</span></span>  <br/> |<span data-ttu-id="bb466-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bb466-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb466-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bb466-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb466-173">False</span><span class="sxs-lookup"><span data-stu-id="bb466-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb466-174">См. также</span><span class="sxs-lookup"><span data-stu-id="bb466-174">See also</span></span>

- [<span data-ttu-id="bb466-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="bb466-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="bb466-176">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="bb466-176">GetItem operation</span></span>](getitem-operation.md)

