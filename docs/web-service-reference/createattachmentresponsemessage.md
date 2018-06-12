---
title: CreateAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: Элемент CreateAttachmentResponseMessage содержит состояние и результат одного запроса CreateAttachment операции.
ms.openlocfilehash: a6d3adde07dedb7a2533d6e9c7fc6ff0497792bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761866"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="451c5-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="451c5-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="451c5-104">Элемент **CreateAttachmentResponseMessage** содержит состояние и результат одного запроса [CreateAttachment операции](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="451c5-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="451c5-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="451c5-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="451c5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="451c5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="451c5-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="451c5-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="451c5-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="451c5-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="451c5-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="451c5-109">Attributes and elements</span></span>

<span data-ttu-id="451c5-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="451c5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="451c5-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="451c5-111">Attributes</span></span>

|<span data-ttu-id="451c5-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="451c5-112">**Attribute**</span></span>|<span data-ttu-id="451c5-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="451c5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="451c5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="451c5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="451c5-115">Описание состояния ответа [операции CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="451c5-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="451c5-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="451c5-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="451c5-117">-Success</span><span class="sxs-lookup"><span data-stu-id="451c5-117">-  Success</span></span>  <br/><span data-ttu-id="451c5-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="451c5-118">-  Warning</span></span>  <br/><span data-ttu-id="451c5-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="451c5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="451c5-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="451c5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="451c5-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="451c5-121">**Value**</span></span>|<span data-ttu-id="451c5-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="451c5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="451c5-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="451c5-123">**Success**</span></span> <br/> |<span data-ttu-id="451c5-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="451c5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="451c5-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="451c5-125">**Warning**</span></span> <br/> | <span data-ttu-id="451c5-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="451c5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="451c5-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="451c5-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="451c5-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="451c5-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="451c5-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="451c5-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="451c5-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="451c5-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="451c5-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="451c5-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="451c5-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="451c5-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="451c5-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="451c5-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="451c5-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="451c5-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="451c5-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="451c5-135">**Error**</span></span> <br/> | <span data-ttu-id="451c5-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="451c5-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="451c5-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="451c5-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="451c5-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="451c5-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="451c5-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="451c5-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="451c5-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="451c5-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="451c5-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="451c5-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="451c5-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="451c5-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="451c5-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="451c5-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="451c5-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="451c5-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="451c5-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="451c5-145">Child elements</span></span>

|<span data-ttu-id="451c5-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="451c5-146">**Element**</span></span>|<span data-ttu-id="451c5-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="451c5-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="451c5-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="451c5-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="451c5-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="451c5-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="451c5-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="451c5-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="451c5-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="451c5-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="451c5-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="451c5-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="451c5-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="451c5-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="451c5-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="451c5-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="451c5-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="451c5-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="451c5-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="451c5-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="451c5-157">Вложения</span><span class="sxs-lookup"><span data-stu-id="451c5-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="451c5-158">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="451c5-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="451c5-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="451c5-159">Parent elements</span></span>

|<span data-ttu-id="451c5-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="451c5-160">**Element**</span></span>|<span data-ttu-id="451c5-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="451c5-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="451c5-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="451c5-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="451c5-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="451c5-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="451c5-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="451c5-164">Remarks</span></span>

<span data-ttu-id="451c5-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="451c5-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="451c5-166">Если несколько вложений присоединены к элементу в одном обращение, атрибут **RootItemChangeKey** в последнее сообщение ответа — это, соответствующий новый ключ изменения элемента с вложениями.</span><span class="sxs-lookup"><span data-stu-id="451c5-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="451c5-167">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="451c5-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="451c5-168">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="451c5-168">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="451c5-169">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="451c5-169">Schema Name</span></span>  <br/> |<span data-ttu-id="451c5-170">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="451c5-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="451c5-171">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="451c5-171">Validation File</span></span>  <br/> |<span data-ttu-id="451c5-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="451c5-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="451c5-173">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="451c5-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="451c5-174">False</span><span class="sxs-lookup"><span data-stu-id="451c5-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="451c5-175">См. также</span><span class="sxs-lookup"><span data-stu-id="451c5-175">See also</span></span>

- [<span data-ttu-id="451c5-176">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="451c5-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="451c5-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="451c5-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="451c5-178">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="451c5-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="451c5-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="451c5-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
