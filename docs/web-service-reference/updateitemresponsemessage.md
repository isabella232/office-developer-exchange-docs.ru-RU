---
title: UpdateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponseMessage
api_type:
- schema
ms.assetid: dc585b05-5afc-4c74-8763-5a54f9a650ec
description: Элемент UpdateItemResponseMessage содержит состояние и результат одного запроса UpdateItem операции.
ms.openlocfilehash: c971657813784e68a01539899e8fabea67847325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840362"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="5c1e7-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c1e7-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="5c1e7-104">Элемент **UpdateItemResponseMessage** содержит состояние и результат одного запроса [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5c1e7-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5c1e7-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="5c1e7-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="5c1e7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c1e7-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5c1e7-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c1e7-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
```xml
<UpdateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <ConflictResults/>
</UpdateItemResponseMessage>
```

 <span data-ttu-id="5c1e7-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c1e7-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-109">Attributes and elements</span></span>

<span data-ttu-id="5c1e7-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c1e7-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5c1e7-111">Attributes</span></span>

|<span data-ttu-id="5c1e7-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-112">**Attribute**</span></span>|<span data-ttu-id="5c1e7-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c1e7-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5c1e7-115">Описание состояния ответа [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5c1e7-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="5c1e7-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="5c1e7-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="5c1e7-117">-Success</span><span class="sxs-lookup"><span data-stu-id="5c1e7-117">-  Success</span></span>  <br/><span data-ttu-id="5c1e7-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="5c1e7-118">-  Warning</span></span>  <br/><span data-ttu-id="5c1e7-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="5c1e7-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5c1e7-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5c1e7-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="5c1e7-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-121">**Value**</span></span>|<span data-ttu-id="5c1e7-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c1e7-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-123">**Success**</span></span> <br/> |<span data-ttu-id="5c1e7-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5c1e7-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-125">**Warning**</span></span> <br/> | <span data-ttu-id="5c1e7-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5c1e7-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5c1e7-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="5c1e7-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5c1e7-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5c1e7-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5c1e7-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="5c1e7-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5c1e7-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="5c1e7-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="5c1e7-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-135">**Error**</span></span> <br/> | <span data-ttu-id="5c1e7-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5c1e7-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="5c1e7-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5c1e7-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5c1e7-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="5c1e7-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="5c1e7-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="5c1e7-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="5c1e7-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="5c1e7-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="5c1e7-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="5c1e7-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5c1e7-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="5c1e7-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5c1e7-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5c1e7-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-145">Child elements</span></span>

|<span data-ttu-id="5c1e7-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-146">**Element**</span></span>|<span data-ttu-id="5c1e7-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c1e7-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5c1e7-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5c1e7-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5c1e7-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c1e7-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5c1e7-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5c1e7-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5c1e7-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5c1e7-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5c1e7-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5c1e7-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5c1e7-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5c1e7-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5c1e7-157">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="5c1e7-158">Содержит массив обновленных элементов.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="5c1e7-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="5c1e7-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="5c1e7-160">Содержит число конфликтов в ответ [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5c1e7-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c1e7-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-161">Parent elements</span></span>

|<span data-ttu-id="5c1e7-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-162">**Element**</span></span>|<span data-ttu-id="5c1e7-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c1e7-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c1e7-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c1e7-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5c1e7-165">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c1e7-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="5c1e7-166">Remarks</span></span>

<span data-ttu-id="5c1e7-167">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5c1e7-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c1e7-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5c1e7-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c1e7-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5c1e7-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c1e7-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5c1e7-170">Schema Name</span></span>  <br/> |<span data-ttu-id="5c1e7-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5c1e7-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c1e7-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5c1e7-172">Validation File</span></span>  <br/> |<span data-ttu-id="5c1e7-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c1e7-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c1e7-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5c1e7-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c1e7-175">False</span><span class="sxs-lookup"><span data-stu-id="5c1e7-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c1e7-176">См. также</span><span class="sxs-lookup"><span data-stu-id="5c1e7-176">See also</span></span>

- [<span data-ttu-id="5c1e7-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="5c1e7-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="5c1e7-178">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="5c1e7-178">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="5c1e7-179">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="5c1e7-179">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

