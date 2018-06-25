---
title: UnsubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponseMessage
api_type:
- schema
ms.assetid: 92c53b13-0ca1-4b44-b925-b23682e9417c
description: Элемент UnsubscribeResponseMessage содержит состояние и результат одного запроса операции отказа от подписки.
ms.openlocfilehash: 09475b8c858ddcd0e404819b6b9a281cbf7cfcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840314"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="bbdd2-103">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bbdd2-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="bbdd2-104">Элемент **UnsubscribeResponseMessage** содержит состояние и результат одного запроса [операции отказа от подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bbdd2-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="bbdd2-105">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="bbdd2-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="bbdd2-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bbdd2-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="bbdd2-107">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bbdd2-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="bbdd2-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bbdd2-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bbdd2-109">Attributes and elements</span></span>

<span data-ttu-id="bbdd2-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbdd2-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bbdd2-111">Attributes</span></span>

|<span data-ttu-id="bbdd2-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-112">**Attribute**</span></span>|<span data-ttu-id="bbdd2-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbdd2-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bbdd2-115">Описание состояния ответа [операции отказа от подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bbdd2-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="bbdd2-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bbdd2-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="bbdd2-117">-Success</span><span class="sxs-lookup"><span data-stu-id="bbdd2-117">-  Success</span></span>  <br/><span data-ttu-id="bbdd2-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bbdd2-118">-  Warning</span></span>  <br/><span data-ttu-id="bbdd2-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="bbdd2-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bbdd2-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bbdd2-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bbdd2-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-121">**Value**</span></span>|<span data-ttu-id="bbdd2-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbdd2-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-123">**Success**</span></span> <br/> |<span data-ttu-id="bbdd2-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bbdd2-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-125">**Warning**</span></span> <br/> | <span data-ttu-id="bbdd2-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bbdd2-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="bbdd2-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="bbdd2-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="bbdd2-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bbdd2-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bbdd2-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="bbdd2-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bbdd2-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bbdd2-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="bbdd2-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-135">**Error**</span></span> <br/> | <span data-ttu-id="bbdd2-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bbdd2-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="bbdd2-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bbdd2-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bbdd2-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bbdd2-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="bbdd2-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="bbdd2-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bbdd2-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="bbdd2-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="bbdd2-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="bbdd2-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="bbdd2-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bbdd2-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="bbdd2-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="bbdd2-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bbdd2-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bbdd2-145">Child elements</span></span>

|<span data-ttu-id="bbdd2-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-146">**Element**</span></span>|<span data-ttu-id="bbdd2-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbdd2-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="bbdd2-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bbdd2-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bbdd2-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bbdd2-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bbdd2-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bbdd2-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bbdd2-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bbdd2-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bbdd2-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bbdd2-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bbdd2-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bbdd2-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bbdd2-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bbdd2-157">Parent elements</span></span>

|<span data-ttu-id="bbdd2-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-158">**Element**</span></span>|<span data-ttu-id="bbdd2-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bbdd2-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbdd2-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bbdd2-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bbdd2-161">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bbdd2-162">Замечания</span><span class="sxs-lookup"><span data-stu-id="bbdd2-162">Remarks</span></span>

<span data-ttu-id="bbdd2-163">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bbdd2-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbdd2-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bbdd2-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbdd2-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bbdd2-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bbdd2-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bbdd2-166">Schema Name</span></span>  <br/> |<span data-ttu-id="bbdd2-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bbdd2-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bbdd2-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bbdd2-168">Validation File</span></span>  <br/> |<span data-ttu-id="bbdd2-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bbdd2-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bbdd2-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bbdd2-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbdd2-171">False</span><span class="sxs-lookup"><span data-stu-id="bbdd2-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbdd2-172">См. также</span><span class="sxs-lookup"><span data-stu-id="bbdd2-172">See also</span></span>

- [<span data-ttu-id="bbdd2-173">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="bbdd2-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="bbdd2-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bbdd2-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

