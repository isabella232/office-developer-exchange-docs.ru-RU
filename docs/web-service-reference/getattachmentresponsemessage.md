---
title: GetAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponseMessage
api_type:
- schema
ms.assetid: f0a841af-422d-4c82-b710-41e2038dbee4
description: Элемент GetAttachmentResponseMessage содержит состояние и результат одного запроса операции GetAttachment.
ms.openlocfilehash: 3bf5aac8ba85675e2941acef6f06eb24f0667d17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762703"
---
# <a name="getattachmentresponsemessage"></a><span data-ttu-id="d7cdb-103">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7cdb-103">GetAttachmentResponseMessage</span></span>

<span data-ttu-id="d7cdb-104">Элемент **GetAttachmentResponseMessage** содержит состояние и результат одного запроса [операции GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7cdb-104">The **GetAttachmentResponseMessage** element contains the status and result of a single [GetAttachment operation](getattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d7cdb-105">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="d7cdb-105">GetAttachmentResponse</span></span>](getattachmentresponse.md) 
- [<span data-ttu-id="d7cdb-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7cdb-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="d7cdb-107">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7cdb-107">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
  
```xml
<GetAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</GetAttachmentResponseMessage>
```

 <span data-ttu-id="d7cdb-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-108">**AttachmentInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7cdb-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7cdb-109">Attributes and elements</span></span>

<span data-ttu-id="d7cdb-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7cdb-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d7cdb-111">Attributes</span></span>

|<span data-ttu-id="d7cdb-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-112">**Attribute**</span></span>|<span data-ttu-id="d7cdb-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7cdb-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d7cdb-115">Описание состояния ответа [операции GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7cdb-115">Describes the status of a [GetAttachment operation](getattachment-operation.md) response.</span></span><br/><br/> <span data-ttu-id="d7cdb-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d7cdb-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="d7cdb-117">-Success</span><span class="sxs-lookup"><span data-stu-id="d7cdb-117">-  Success</span></span>  <br/><span data-ttu-id="d7cdb-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d7cdb-118">-  Warning</span></span>  <br/><span data-ttu-id="d7cdb-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d7cdb-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="d7cdb-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d7cdb-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="d7cdb-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-121">**Value**</span></span>|<span data-ttu-id="d7cdb-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7cdb-123">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="d7cdb-123">Success</span></span>  <br/> |<span data-ttu-id="d7cdb-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d7cdb-125">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="d7cdb-125">Warning</span></span>  <br/> | <span data-ttu-id="d7cdb-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d7cdb-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d7cdb-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="d7cdb-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="d7cdb-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d7cdb-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d7cdb-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d7cdb-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d7cdb-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="d7cdb-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d7cdb-135">Error</span><span class="sxs-lookup"><span data-stu-id="d7cdb-135">Error</span></span>  <br/> | <span data-ttu-id="d7cdb-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d7cdb-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d7cdb-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d7cdb-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7cdb-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d7cdb-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d7cdb-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d7cdb-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d7cdb-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="d7cdb-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="d7cdb-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d7cdb-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="d7cdb-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d7cdb-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d7cdb-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d7cdb-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d7cdb-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d7cdb-145">Child elements</span></span>

|<span data-ttu-id="d7cdb-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-146">**Element**</span></span>|<span data-ttu-id="d7cdb-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7cdb-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7cdb-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d7cdb-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d7cdb-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7cdb-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d7cdb-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d7cdb-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7cdb-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d7cdb-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d7cdb-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d7cdb-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d7cdb-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d7cdb-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d7cdb-157">Вложения</span><span class="sxs-lookup"><span data-stu-id="d7cdb-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d7cdb-158">Содержит элементы или файлы, которые являются ttached для элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-158">Contains the items or files that are ttached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7cdb-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d7cdb-159">Parent elements</span></span>

|<span data-ttu-id="d7cdb-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-160">**Element**</span></span>|<span data-ttu-id="d7cdb-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7cdb-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7cdb-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7cdb-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d7cdb-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7cdb-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="d7cdb-164">Remarks</span></span>

<span data-ttu-id="d7cdb-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d7cdb-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7cdb-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d7cdb-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7cdb-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d7cdb-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7cdb-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d7cdb-168">Schema Name</span></span>  <br/> |<span data-ttu-id="d7cdb-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d7cdb-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7cdb-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d7cdb-170">Validation File</span></span>  <br/> |<span data-ttu-id="d7cdb-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7cdb-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7cdb-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d7cdb-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7cdb-173">False</span><span class="sxs-lookup"><span data-stu-id="d7cdb-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7cdb-174">См. также</span><span class="sxs-lookup"><span data-stu-id="d7cdb-174">See also</span></span>

- [<span data-ttu-id="d7cdb-175">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="d7cdb-175">GetAttachment</span></span>](getattachment.md) 
- [<span data-ttu-id="d7cdb-176">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="d7cdb-176">GetAttachment operation</span></span>](getattachment-operation.md)

