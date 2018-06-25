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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840362"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="4daf1-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4daf1-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="4daf1-104">Элемент **UpdateItemResponseMessage** содержит состояние и результат одного запроса [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4daf1-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4daf1-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="4daf1-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="4daf1-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4daf1-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4daf1-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4daf1-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
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

 <span data-ttu-id="4daf1-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4daf1-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4daf1-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4daf1-109">Attributes and elements</span></span>

<span data-ttu-id="4daf1-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4daf1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4daf1-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4daf1-111">Attributes</span></span>

|<span data-ttu-id="4daf1-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4daf1-112">**Attribute**</span></span>|<span data-ttu-id="4daf1-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4daf1-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4daf1-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4daf1-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4daf1-115">Описание состояния ответа [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4daf1-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4daf1-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4daf1-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4daf1-117">-Success</span><span class="sxs-lookup"><span data-stu-id="4daf1-117">-  Success</span></span>  <br/><span data-ttu-id="4daf1-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4daf1-118">-  Warning</span></span>  <br/><span data-ttu-id="4daf1-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="4daf1-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4daf1-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4daf1-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4daf1-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4daf1-121">**Value**</span></span>|<span data-ttu-id="4daf1-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4daf1-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4daf1-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="4daf1-123">**Success**</span></span> <br/> |<span data-ttu-id="4daf1-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="4daf1-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4daf1-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="4daf1-125">**Warning**</span></span> <br/> | <span data-ttu-id="4daf1-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4daf1-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4daf1-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="4daf1-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4daf1-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="4daf1-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4daf1-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="4daf1-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4daf1-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4daf1-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4daf1-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="4daf1-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4daf1-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4daf1-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4daf1-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="4daf1-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="4daf1-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="4daf1-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4daf1-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="4daf1-135">**Error**</span></span> <br/> | <span data-ttu-id="4daf1-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4daf1-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4daf1-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="4daf1-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4daf1-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4daf1-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4daf1-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="4daf1-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4daf1-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4daf1-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="4daf1-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="4daf1-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="4daf1-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="4daf1-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4daf1-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="4daf1-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4daf1-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="4daf1-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4daf1-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4daf1-145">Child elements</span></span>

|<span data-ttu-id="4daf1-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4daf1-146">**Element**</span></span>|<span data-ttu-id="4daf1-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4daf1-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4daf1-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4daf1-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4daf1-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="4daf1-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4daf1-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4daf1-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4daf1-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="4daf1-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4daf1-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4daf1-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4daf1-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="4daf1-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4daf1-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4daf1-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4daf1-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4daf1-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4daf1-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="4daf1-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4daf1-157">Элементы</span><span class="sxs-lookup"><span data-stu-id="4daf1-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="4daf1-158">Содержит массив обновленных элементов.</span><span class="sxs-lookup"><span data-stu-id="4daf1-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="4daf1-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="4daf1-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="4daf1-160">Содержит число конфликтов в ответ [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4daf1-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4daf1-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4daf1-161">Parent elements</span></span>

|<span data-ttu-id="4daf1-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4daf1-162">**Element**</span></span>|<span data-ttu-id="4daf1-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4daf1-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4daf1-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4daf1-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4daf1-165">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4daf1-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4daf1-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="4daf1-166">Remarks</span></span>

<span data-ttu-id="4daf1-167">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4daf1-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4daf1-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4daf1-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4daf1-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4daf1-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4daf1-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4daf1-170">Schema Name</span></span>  <br/> |<span data-ttu-id="4daf1-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4daf1-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4daf1-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4daf1-172">Validation File</span></span>  <br/> |<span data-ttu-id="4daf1-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4daf1-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4daf1-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4daf1-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="4daf1-175">False</span><span class="sxs-lookup"><span data-stu-id="4daf1-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4daf1-176">См. также</span><span class="sxs-lookup"><span data-stu-id="4daf1-176">See also</span></span>

- [<span data-ttu-id="4daf1-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="4daf1-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="4daf1-178">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="4daf1-178">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="4daf1-179">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="4daf1-179">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

