---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: Элемент SendItemResponseMessage содержит состояние и результат одного запроса операции SendItem.
ms.openlocfilehash: 70355aa2b46303bfceafa2cfe89f1c84896f3158
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835344"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="3425b-103">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3425b-103">SendItemResponseMessage</span></span>

<span data-ttu-id="3425b-104">Элемент **SendItemResponseMessage** содержит состояние и результат одного запроса [операции SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3425b-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="3425b-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3425b-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3425b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3425b-106">Attributes and elements</span></span>

<span data-ttu-id="3425b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3425b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3425b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3425b-108">Attributes</span></span>

|<span data-ttu-id="3425b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3425b-109">**Attribute**</span></span>|<span data-ttu-id="3425b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3425b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3425b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3425b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3425b-112">Описание состояния ответа [операции SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3425b-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="3425b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3425b-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="3425b-114">-Success</span><span class="sxs-lookup"><span data-stu-id="3425b-114">-  Success</span></span>  <br/><span data-ttu-id="3425b-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="3425b-115">-  Warning</span></span>  <br/><span data-ttu-id="3425b-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="3425b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3425b-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3425b-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="3425b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3425b-118">**Value**</span></span>|<span data-ttu-id="3425b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3425b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3425b-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="3425b-120">**Success**</span></span> <br/> |<span data-ttu-id="3425b-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="3425b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3425b-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="3425b-122">**Warning**</span></span> <br/> | <span data-ttu-id="3425b-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="3425b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="3425b-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="3425b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3425b-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="3425b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3425b-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="3425b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3425b-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3425b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3425b-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="3425b-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="3425b-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3425b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3425b-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="3425b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="3425b-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="3425b-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="3425b-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="3425b-132">**Error**</span></span> <br/> | <span data-ttu-id="3425b-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="3425b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3425b-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="3425b-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="3425b-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3425b-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3425b-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="3425b-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="3425b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="3425b-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="3425b-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="3425b-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="3425b-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="3425b-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3425b-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="3425b-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="3425b-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="3425b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3425b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3425b-142">Child elements</span></span>

|<span data-ttu-id="3425b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3425b-143">**Element**</span></span>|<span data-ttu-id="3425b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3425b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3425b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="3425b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3425b-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="3425b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3425b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3425b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3425b-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="3425b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3425b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3425b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3425b-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="3425b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3425b-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3425b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3425b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3425b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3425b-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="3425b-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3425b-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3425b-154">Parent elements</span></span>

|<span data-ttu-id="3425b-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3425b-155">**Element**</span></span>|<span data-ttu-id="3425b-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3425b-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3425b-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3425b-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3425b-158">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3425b-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3425b-159">Замечания</span><span class="sxs-lookup"><span data-stu-id="3425b-159">Remarks</span></span>

<span data-ttu-id="3425b-160">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3425b-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3425b-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3425b-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3425b-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3425b-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3425b-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3425b-163">Schema Name</span></span>  <br/> |<span data-ttu-id="3425b-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3425b-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3425b-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3425b-165">Validation File</span></span>  <br/> |<span data-ttu-id="3425b-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3425b-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3425b-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3425b-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="3425b-168">False</span><span class="sxs-lookup"><span data-stu-id="3425b-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3425b-169">См. также</span><span class="sxs-lookup"><span data-stu-id="3425b-169">See also</span></span>

- [<span data-ttu-id="3425b-170">SendItem Operation</span><span class="sxs-lookup"><span data-stu-id="3425b-170">SendItem operation</span></span>](senditem-operation.md)
- [<span data-ttu-id="3425b-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3425b-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

