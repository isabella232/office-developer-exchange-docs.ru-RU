---
title: UpdateInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: Элемент UpdateInboxRulesResponse определяет ответ на запрос UpdateInboxRules.
ms.openlocfilehash: cd64e4546f8d9bf573062d9c982477be3fa4d925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840346"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="4379a-103">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4379a-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="4379a-104">Элемент **UpdateInboxRulesResponse** определяет ответ на запрос UpdateInboxRules.</span><span class="sxs-lookup"><span data-stu-id="4379a-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="4379a-105">**UpdateInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="4379a-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4379a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4379a-106">Attributes and elements</span></span>

<span data-ttu-id="4379a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4379a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4379a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4379a-108">Attributes</span></span>

|<span data-ttu-id="4379a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4379a-109">**Attribute**</span></span>|<span data-ttu-id="4379a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4379a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4379a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4379a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4379a-112">Описание состояния ответа [операции отказа от подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4379a-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="4379a-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4379a-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4379a-114">-Success</span><span class="sxs-lookup"><span data-stu-id="4379a-114">-  Success</span></span>  <br/><span data-ttu-id="4379a-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4379a-115">-  Warning</span></span>  <br/><span data-ttu-id="4379a-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="4379a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4379a-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4379a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="4379a-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4379a-118">**Value**</span></span>|<span data-ttu-id="4379a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4379a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4379a-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="4379a-120">**Success**</span></span> <br/> |<span data-ttu-id="4379a-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="4379a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4379a-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="4379a-122">**Warning**</span></span> <br/> | <span data-ttu-id="4379a-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4379a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="4379a-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="4379a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4379a-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="4379a-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4379a-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="4379a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4379a-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4379a-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4379a-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="4379a-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4379a-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4379a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4379a-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="4379a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="4379a-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="4379a-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4379a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="4379a-132">**Error**</span></span> <br/> | <span data-ttu-id="4379a-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4379a-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4379a-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="4379a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4379a-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4379a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4379a-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="4379a-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="4379a-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4379a-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="4379a-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="4379a-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4379a-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="4379a-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4379a-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="4379a-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="4379a-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="4379a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4379a-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4379a-142">Child elements</span></span>

|<span data-ttu-id="4379a-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4379a-143">**Element**</span></span>|<span data-ttu-id="4379a-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4379a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4379a-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="4379a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4379a-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="4379a-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4379a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4379a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4379a-148">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="4379a-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="4379a-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4379a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4379a-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="4379a-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4379a-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4379a-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4379a-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4379a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4379a-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="4379a-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4379a-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="4379a-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="4379a-155">Представляет массив ошибок проверки правил для каждого правила поля, имеющего ошибку.</span><span class="sxs-lookup"><span data-stu-id="4379a-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4379a-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4379a-156">Parent elements</span></span>

<span data-ttu-id="4379a-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="4379a-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4379a-158">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4379a-158">Text value</span></span>

<span data-ttu-id="4379a-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="4379a-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4379a-160">Замечания</span><span class="sxs-lookup"><span data-stu-id="4379a-160">Remarks</span></span>

<span data-ttu-id="4379a-161">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4379a-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4379a-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4379a-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4379a-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4379a-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4379a-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4379a-164">Schema name</span></span>  <br/> |<span data-ttu-id="4379a-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4379a-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4379a-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4379a-166">Validation file</span></span>  <br/> |<span data-ttu-id="4379a-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4379a-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4379a-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4379a-168">Can be empty</span></span>  <br/> |<span data-ttu-id="4379a-169">False</span><span class="sxs-lookup"><span data-stu-id="4379a-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4379a-170">См. также</span><span class="sxs-lookup"><span data-stu-id="4379a-170">See also</span></span>

- [<span data-ttu-id="4379a-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4379a-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="4379a-172">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4379a-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="4379a-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4379a-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

