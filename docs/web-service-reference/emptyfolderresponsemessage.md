---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: Элемент EmptyFolderResponseMessage содержит состояние и результат одного запроса EmptyFolder.
ms.openlocfilehash: ebdaac28cdd16a55811276ef0d11c03b00d3897a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762329"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="09c22-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="09c22-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="09c22-104">Элемент **EmptyFolderResponseMessage** содержит состояние и результат одного запроса [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="09c22-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="09c22-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="09c22-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09c22-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09c22-106">Attributes and elements</span></span>

<span data-ttu-id="09c22-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="09c22-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09c22-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09c22-108">Attributes</span></span>

|<span data-ttu-id="09c22-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="09c22-109">**Attribute**</span></span>|<span data-ttu-id="09c22-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09c22-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="09c22-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="09c22-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="09c22-112">Описание состояния ответа [операции EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="09c22-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="09c22-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="09c22-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="09c22-114">-Success</span><span class="sxs-lookup"><span data-stu-id="09c22-114">-  Success</span></span>  <br/><span data-ttu-id="09c22-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="09c22-115">-  Warning</span></span>  <br/><span data-ttu-id="09c22-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="09c22-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="09c22-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="09c22-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="09c22-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="09c22-118">**Value**</span></span>|<span data-ttu-id="09c22-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09c22-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="09c22-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="09c22-120">**Success**</span></span> <br/> |<span data-ttu-id="09c22-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="09c22-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="09c22-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="09c22-122">**Warning**</span></span> <br/> | <span data-ttu-id="09c22-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="09c22-123">Describes a request that was not processed.</span></span> <span data-ttu-id="09c22-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="09c22-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="09c22-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="09c22-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="09c22-126">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="09c22-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="09c22-127">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="09c22-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="09c22-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="09c22-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="09c22-129">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="09c22-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="09c22-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="09c22-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="09c22-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="09c22-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="09c22-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="09c22-132">**Error**</span></span> <br/> | <span data-ttu-id="09c22-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="09c22-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="09c22-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="09c22-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="09c22-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09c22-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="09c22-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="09c22-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="09c22-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="09c22-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="09c22-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="09c22-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="09c22-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="09c22-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="09c22-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="09c22-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="09c22-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="09c22-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="09c22-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09c22-142">Child elements</span></span>

|<span data-ttu-id="09c22-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09c22-143">**Element**</span></span>|<span data-ttu-id="09c22-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09c22-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09c22-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="09c22-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="09c22-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="09c22-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="09c22-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="09c22-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="09c22-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="09c22-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="09c22-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="09c22-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="09c22-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="09c22-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="09c22-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="09c22-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="09c22-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="09c22-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="09c22-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="09c22-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09c22-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09c22-154">Parent elements</span></span>

|<span data-ttu-id="09c22-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09c22-155">**Element**</span></span>|<span data-ttu-id="09c22-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09c22-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09c22-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="09c22-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="09c22-158">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="09c22-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09c22-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="09c22-159">Text value</span></span>

<span data-ttu-id="09c22-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="09c22-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09c22-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="09c22-161">Remarks</span></span>

<span data-ttu-id="09c22-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="09c22-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09c22-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="09c22-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09c22-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="09c22-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09c22-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="09c22-165">Schema Name</span></span>  <br/> |<span data-ttu-id="09c22-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="09c22-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="09c22-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="09c22-167">Validation File</span></span>  <br/> |<span data-ttu-id="09c22-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="09c22-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09c22-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="09c22-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="09c22-170">False</span><span class="sxs-lookup"><span data-stu-id="09c22-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09c22-171">См. также</span><span class="sxs-lookup"><span data-stu-id="09c22-171">See also</span></span>

- [<span data-ttu-id="09c22-172">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="09c22-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="09c22-173">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="09c22-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="09c22-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="09c22-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
