---
title: CopyItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: Элемент CopyItemResponseMessage содержит состояние и результат одного запроса CopyItem операции.
ms.openlocfilehash: 6c1acaff422fd731ca81a3ab244d76a73f3b5c15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761845"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="7121a-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7121a-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="7121a-104">Элемент **CopyItemResponseMessage** содержит состояние и результат одного запроса [CopyItem операции](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7121a-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="7121a-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7121a-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7121a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7121a-106">Attributes and elements</span></span>

<span data-ttu-id="7121a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7121a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7121a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7121a-108">Attributes</span></span>

|<span data-ttu-id="7121a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7121a-109">**Attribute**</span></span>|<span data-ttu-id="7121a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7121a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7121a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7121a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7121a-112">Описание состояния ответа [CopyItem операции](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7121a-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="7121a-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="7121a-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="7121a-114">-Success</span><span class="sxs-lookup"><span data-stu-id="7121a-114">- Success</span></span>  <br/><span data-ttu-id="7121a-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="7121a-115">-  Warning</span></span>  <br/><span data-ttu-id="7121a-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="7121a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7121a-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7121a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="7121a-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7121a-118">**Value**</span></span>|<span data-ttu-id="7121a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7121a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7121a-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="7121a-120">**Success**</span></span> <br/> |<span data-ttu-id="7121a-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="7121a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7121a-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="7121a-122">**Warning**</span></span> <br/> | <span data-ttu-id="7121a-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="7121a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7121a-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="7121a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="7121a-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="7121a-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="7121a-126">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="7121a-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="7121a-127">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="7121a-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="7121a-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="7121a-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7121a-129">-Базы данных почтовых ящиков (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="7121a-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="7121a-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="7121a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="7121a-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="7121a-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7121a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="7121a-132">**Error**</span></span> <br/> | <span data-ttu-id="7121a-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="7121a-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="7121a-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="7121a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7121a-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7121a-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7121a-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="7121a-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7121a-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="7121a-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="7121a-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="7121a-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7121a-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="7121a-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7121a-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="7121a-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="7121a-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="7121a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7121a-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7121a-142">Child elements</span></span>

|<span data-ttu-id="7121a-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7121a-143">**Element**</span></span>|<span data-ttu-id="7121a-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7121a-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7121a-145">- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="7121a-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="7121a-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="7121a-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7121a-147">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="7121a-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7121a-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7121a-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7121a-149">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="7121a-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7121a-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7121a-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7121a-151">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="7121a-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7121a-152">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="7121a-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7121a-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7121a-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7121a-154">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="7121a-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7121a-155">Элементы</span><span class="sxs-lookup"><span data-stu-id="7121a-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="7121a-156">Содержит массив скопированной элементов</span><span class="sxs-lookup"><span data-stu-id="7121a-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7121a-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7121a-157">Parent elements</span></span>

|<span data-ttu-id="7121a-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7121a-158">**Element**</span></span>|<span data-ttu-id="7121a-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7121a-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7121a-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7121a-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7121a-161">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7121a-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7121a-162">Замечания</span><span class="sxs-lookup"><span data-stu-id="7121a-162">Remarks</span></span>

<span data-ttu-id="7121a-163">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7121a-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7121a-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7121a-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7121a-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7121a-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7121a-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7121a-166">Schema name</span></span>  <br/> |<span data-ttu-id="7121a-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7121a-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7121a-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7121a-168">Validation file</span></span>  <br/> |<span data-ttu-id="7121a-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7121a-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7121a-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7121a-170">Can be empty</span></span>  <br/> |<span data-ttu-id="7121a-171">False</span><span class="sxs-lookup"><span data-stu-id="7121a-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7121a-172">См. также</span><span class="sxs-lookup"><span data-stu-id="7121a-172">See also</span></span>

- [<span data-ttu-id="7121a-173">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="7121a-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="7121a-174">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="7121a-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

