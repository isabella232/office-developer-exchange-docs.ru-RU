---
title: CreateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponseMessage
api_type:
- schema
ms.assetid: 595d36c2-f87a-4d50-8e8b-f58d7641564b
description: Элемент CreateItemResponseMessage содержит состояние и результат одного запроса операции CreateItem.
ms.openlocfilehash: 099dc799bedb527472bbe7d34cad0dbc8e98bec5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761907"
---
# <a name="createitemresponsemessage"></a><span data-ttu-id="43caa-103">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="43caa-103">CreateItemResponseMessage</span></span>

<span data-ttu-id="43caa-104">Элемент **CreateItemResponseMessage** содержит состояние и результат один запрос [CreateItem операции](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="43caa-104">The **CreateItemResponseMessage** element contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="43caa-105">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="43caa-105">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="43caa-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="43caa-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="43caa-107">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="43caa-107">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
  
```xml
<CreateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CreateItemResponseMessage>
```

 <span data-ttu-id="43caa-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="43caa-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43caa-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="43caa-109">Attributes and elements</span></span>

<span data-ttu-id="43caa-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="43caa-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43caa-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="43caa-111">Attributes</span></span>

|<span data-ttu-id="43caa-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="43caa-112">**Attribute**</span></span>|<span data-ttu-id="43caa-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43caa-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="43caa-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="43caa-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="43caa-115">Описание состояния ответа [операции CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="43caa-115">Describes the status of a [CreateItem operation](createitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="43caa-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="43caa-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="43caa-117">-Success</span><span class="sxs-lookup"><span data-stu-id="43caa-117">-  Success</span></span>  <br/><span data-ttu-id="43caa-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="43caa-118">-  Warning</span></span>  <br/><span data-ttu-id="43caa-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="43caa-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="43caa-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="43caa-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="43caa-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="43caa-121">**Value**</span></span>|<span data-ttu-id="43caa-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43caa-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="43caa-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="43caa-123">**Success**</span></span> <br/> |<span data-ttu-id="43caa-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="43caa-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="43caa-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="43caa-125">**Warning**</span></span> <br/> | <span data-ttu-id="43caa-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="43caa-126">Describes a request that was not processed.</span></span> <span data-ttu-id="43caa-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="43caa-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="43caa-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="43caa-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="43caa-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="43caa-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="43caa-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="43caa-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="43caa-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="43caa-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="43caa-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="43caa-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="43caa-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="43caa-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="43caa-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="43caa-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="43caa-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="43caa-135">**Error**</span></span> <br/> | <span data-ttu-id="43caa-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="43caa-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="43caa-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="43caa-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="43caa-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="43caa-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="43caa-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="43caa-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="43caa-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="43caa-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="43caa-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="43caa-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="43caa-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="43caa-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="43caa-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="43caa-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="43caa-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="43caa-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="43caa-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="43caa-145">Child elements</span></span>

|<span data-ttu-id="43caa-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43caa-146">**Element**</span></span>|<span data-ttu-id="43caa-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43caa-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43caa-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="43caa-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="43caa-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="43caa-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="43caa-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="43caa-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="43caa-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="43caa-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="43caa-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="43caa-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="43caa-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="43caa-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="43caa-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="43caa-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="43caa-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="43caa-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="43caa-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="43caa-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="43caa-157">Элементы</span><span class="sxs-lookup"><span data-stu-id="43caa-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="43caa-158">Содержит массив созданных элементов.</span><span class="sxs-lookup"><span data-stu-id="43caa-158">Contains an array of created items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43caa-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="43caa-159">Parent elements</span></span>

|<span data-ttu-id="43caa-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43caa-160">**Element**</span></span>|<span data-ttu-id="43caa-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43caa-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43caa-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="43caa-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="43caa-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="43caa-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43caa-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="43caa-164">Remarks</span></span>

<span data-ttu-id="43caa-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="43caa-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43caa-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="43caa-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43caa-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="43caa-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="43caa-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="43caa-168">Schema Name</span></span>  <br/> |<span data-ttu-id="43caa-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="43caa-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="43caa-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="43caa-170">Validation File</span></span>  <br/> |<span data-ttu-id="43caa-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="43caa-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="43caa-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="43caa-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="43caa-173">False</span><span class="sxs-lookup"><span data-stu-id="43caa-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43caa-174">См. также</span><span class="sxs-lookup"><span data-stu-id="43caa-174">See also</span></span>

- [<span data-ttu-id="43caa-175">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="43caa-175">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="43caa-176">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="43caa-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="43caa-177">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="43caa-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

