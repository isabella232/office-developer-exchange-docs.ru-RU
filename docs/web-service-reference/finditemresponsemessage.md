---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: Элемент FindItemResponseMessage содержит состояние и результат одного запроса FindItem операции.
ms.openlocfilehash: 0a4bfb3ba8d85b0bff0d03f043be865ce7276229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762578"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="e8e81-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e8e81-103">FindItemResponseMessage</span></span>

<span data-ttu-id="e8e81-104">Элемент **FindItemResponseMessage** содержит состояние и результат одного запроса [FindItem операции](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e8e81-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e8e81-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="e8e81-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="e8e81-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e8e81-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="e8e81-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e8e81-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="e8e81-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e8e81-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8e81-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8e81-109">Attributes and elements</span></span>

<span data-ttu-id="e8e81-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e8e81-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8e81-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8e81-111">Attributes</span></span>

|<span data-ttu-id="e8e81-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e8e81-112">**Attribute**</span></span>|<span data-ttu-id="e8e81-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8e81-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8e81-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e8e81-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e8e81-115">Описание состояния ответа [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e8e81-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="e8e81-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e8e81-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="e8e81-117">-Success</span><span class="sxs-lookup"><span data-stu-id="e8e81-117">-  Success</span></span>  <br/><span data-ttu-id="e8e81-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e8e81-118">-  Warning</span></span>  <br/><span data-ttu-id="e8e81-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="e8e81-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e8e81-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e8e81-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="e8e81-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e8e81-121">**Value**</span></span>|<span data-ttu-id="e8e81-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8e81-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8e81-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="e8e81-123">**Success**</span></span> <br/> |<span data-ttu-id="e8e81-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="e8e81-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e8e81-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="e8e81-125">**Warning**</span></span> <br/> | <span data-ttu-id="e8e81-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e8e81-126">Describes a request that was not processed.</span></span> <span data-ttu-id="e8e81-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента запроса обработке и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="e8e81-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e8e81-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="e8e81-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="e8e81-129">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="e8e81-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="e8e81-130">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="e8e81-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="e8e81-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="e8e81-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e8e81-132">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="e8e81-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="e8e81-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="e8e81-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="e8e81-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="e8e81-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="e8e81-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="e8e81-135">**Error**</span></span> <br/> | <span data-ttu-id="e8e81-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e8e81-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e8e81-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="e8e81-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e8e81-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8e81-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e8e81-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="e8e81-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="e8e81-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e8e81-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="e8e81-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="e8e81-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="e8e81-142">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="e8e81-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e8e81-143">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="e8e81-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="e8e81-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="e8e81-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8e81-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8e81-145">Child elements</span></span>

|<span data-ttu-id="e8e81-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8e81-146">**Element**</span></span>|<span data-ttu-id="e8e81-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8e81-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8e81-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="e8e81-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e8e81-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e8e81-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e8e81-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e8e81-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e8e81-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="e8e81-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e8e81-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e8e81-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e8e81-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e8e81-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e8e81-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e8e81-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e8e81-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e8e81-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e8e81-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e8e81-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e8e81-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="e8e81-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="e8e81-158">Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e8e81-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8e81-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8e81-159">Parent elements</span></span>

|<span data-ttu-id="e8e81-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8e81-160">**Element**</span></span>|<span data-ttu-id="e8e81-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8e81-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8e81-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e8e81-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e8e81-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8e81-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8e81-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="e8e81-164">Remarks</span></span>

<span data-ttu-id="e8e81-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8e81-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8e81-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8e81-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8e81-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8e81-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8e81-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8e81-168">Schema name</span></span>  <br/> |<span data-ttu-id="e8e81-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e8e81-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8e81-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8e81-170">Validation file</span></span>  <br/> |<span data-ttu-id="e8e81-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8e81-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8e81-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8e81-172">Can be empty</span></span>  <br/> |<span data-ttu-id="e8e81-173">False</span><span class="sxs-lookup"><span data-stu-id="e8e81-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8e81-174">См. также</span><span class="sxs-lookup"><span data-stu-id="e8e81-174">See also</span></span>

- [<span data-ttu-id="e8e81-175">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="e8e81-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="e8e81-176">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="e8e81-176">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

