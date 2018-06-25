---
title: UploadItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: Элемент UploadItemsResponseMessage содержит состояние и результаты запроса для отправки элемента одного почтового ящика.
ms.openlocfilehash: 9a1a33011aa1e240ab7e15794e2e89401238ffda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840398"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="15520-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="15520-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="15520-104">Элемент **UploadItemsResponseMessage** содержит состояние и результаты запроса для отправки элемента одного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="15520-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="15520-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="15520-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="15520-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="15520-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="15520-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="15520-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="15520-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="15520-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15520-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15520-109">Attributes and elements</span></span>

<span data-ttu-id="15520-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="15520-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15520-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15520-111">Attributes</span></span>

|<span data-ttu-id="15520-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="15520-112">**Attribute**</span></span>|<span data-ttu-id="15520-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15520-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="15520-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="15520-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="15520-115">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="15520-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="15520-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="15520-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="15520-117">-Success</span><span class="sxs-lookup"><span data-stu-id="15520-117">-  Success</span></span>  <br/><span data-ttu-id="15520-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="15520-118">-  Warning</span></span>  <br/><span data-ttu-id="15520-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="15520-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="15520-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="15520-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="15520-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="15520-121">**Value**</span></span>|<span data-ttu-id="15520-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15520-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="15520-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="15520-123">**Success**</span></span> <br/> |<span data-ttu-id="15520-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="15520-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="15520-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="15520-125">**Warning**</span></span> <br/> | <span data-ttu-id="15520-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="15520-126">Describes a request that was not processed.</span></span> <span data-ttu-id="15520-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="15520-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="15520-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="15520-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="15520-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="15520-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="15520-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="15520-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="15520-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="15520-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="15520-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="15520-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="15520-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="15520-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="15520-134">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="15520-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="15520-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="15520-135">**Error**</span></span> <br/> | <span data-ttu-id="15520-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="15520-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="15520-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="15520-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="15520-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15520-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="15520-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="15520-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="15520-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="15520-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="15520-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="15520-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="15520-142">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="15520-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="15520-143">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="15520-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="15520-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="15520-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="15520-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15520-145">Child elements</span></span>

|<span data-ttu-id="15520-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15520-146">**Element**</span></span>|<span data-ttu-id="15520-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15520-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15520-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="15520-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="15520-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="15520-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="15520-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="15520-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="15520-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="15520-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="15520-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="15520-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="15520-153">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="15520-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="15520-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="15520-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="15520-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="15520-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="15520-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="15520-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="15520-157">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="15520-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="15520-158">Содержит идентификатор элемента загруженного элемента.</span><span class="sxs-lookup"><span data-stu-id="15520-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15520-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15520-159">Parent elements</span></span>

|<span data-ttu-id="15520-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15520-160">**Element**</span></span>|<span data-ttu-id="15520-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15520-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15520-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="15520-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="15520-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="15520-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15520-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="15520-164">Text value</span></span>

<span data-ttu-id="15520-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="15520-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15520-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="15520-166">Remarks</span></span>

<span data-ttu-id="15520-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="15520-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15520-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15520-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15520-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15520-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15520-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15520-170">Schema Name</span></span>  <br/> |<span data-ttu-id="15520-171">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="15520-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="15520-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15520-172">Validation File</span></span>  <br/> |<span data-ttu-id="15520-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="15520-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15520-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15520-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="15520-175">False</span><span class="sxs-lookup"><span data-stu-id="15520-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15520-176">См. также</span><span class="sxs-lookup"><span data-stu-id="15520-176">See also</span></span>

- [<span data-ttu-id="15520-177">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="15520-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="15520-178">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="15520-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="15520-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="15520-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

