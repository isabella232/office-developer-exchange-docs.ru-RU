---
title: DisconnectPhoneCallResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCallResponse
api_type:
- schema
ms.assetid: 05041799-5b81-4b87-ada8-ce6c506ffe01
description: Элемент DisconnectPhoneCallResponse содержит состояние и результат одного запроса DisconnectPhoneCall.
ms.openlocfilehash: 06471ea342424298a4e1d5a0562f8ed9866e26d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762138"
---
# <a name="disconnectphonecallresponse"></a><span data-ttu-id="22e64-103">DisconnectPhoneCallResponse</span><span class="sxs-lookup"><span data-stu-id="22e64-103">DisconnectPhoneCallResponse</span></span>

<span data-ttu-id="22e64-104">Элемент **DisconnectPhoneCallResponse** содержит состояние и результат одного запроса **DisconnectPhoneCall** .</span><span class="sxs-lookup"><span data-stu-id="22e64-104">The **DisconnectPhoneCallResponse** element contains the status and result of a single **DisconnectPhoneCall** request.</span></span> 
  
```xml
<DisconnectPhoneCallResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DisconnectPhoneCallResponse>
```

 <span data-ttu-id="22e64-105">**DisconnectPhoneCallResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="22e64-105">**DisconnectPhoneCallResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22e64-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22e64-106">Attributes and elements</span></span>

<span data-ttu-id="22e64-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="22e64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22e64-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22e64-108">Attributes</span></span>

|<span data-ttu-id="22e64-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="22e64-109">**Attribute**</span></span>|<span data-ttu-id="22e64-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22e64-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22e64-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="22e64-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="22e64-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="22e64-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="22e64-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="22e64-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="22e64-114">-Success</span><span class="sxs-lookup"><span data-stu-id="22e64-114">-  Success</span></span>  <br/><span data-ttu-id="22e64-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="22e64-115">-  Warning</span></span>  <br/><span data-ttu-id="22e64-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="22e64-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="22e64-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="22e64-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="22e64-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="22e64-118">**Value**</span></span>|<span data-ttu-id="22e64-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22e64-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22e64-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="22e64-120">**Success**</span></span> <br/> |<span data-ttu-id="22e64-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="22e64-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="22e64-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="22e64-122">**Warning**</span></span> <br/> | <span data-ttu-id="22e64-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="22e64-123">Describes a request that was not processed.</span></span> <span data-ttu-id="22e64-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="22e64-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="22e64-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="22e64-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="22e64-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="22e64-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="22e64-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="22e64-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="22e64-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="22e64-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="22e64-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="22e64-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="22e64-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="22e64-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="22e64-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="22e64-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="22e64-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="22e64-132">**Error**</span></span> <br/> | <span data-ttu-id="22e64-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="22e64-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="22e64-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="22e64-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="22e64-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22e64-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="22e64-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="22e64-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="22e64-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="22e64-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="22e64-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="22e64-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="22e64-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="22e64-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="22e64-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="22e64-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="22e64-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="22e64-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22e64-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22e64-142">Child elements</span></span>

|<span data-ttu-id="22e64-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22e64-143">**Element**</span></span>|<span data-ttu-id="22e64-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22e64-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22e64-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="22e64-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="22e64-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="22e64-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="22e64-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="22e64-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="22e64-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="22e64-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="22e64-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="22e64-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="22e64-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="22e64-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="22e64-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="22e64-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="22e64-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="22e64-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="22e64-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="22e64-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22e64-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22e64-154">Parent elements</span></span>

<span data-ttu-id="22e64-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="22e64-155">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="22e64-156">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="22e64-156">Text value</span></span>

<span data-ttu-id="22e64-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="22e64-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22e64-158">Замечания</span><span class="sxs-lookup"><span data-stu-id="22e64-158">Remarks</span></span>

<span data-ttu-id="22e64-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="22e64-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22e64-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22e64-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22e64-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22e64-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22e64-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22e64-162">Schema Name</span></span>  <br/> |<span data-ttu-id="22e64-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="22e64-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22e64-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22e64-164">Validation File</span></span>  <br/> |<span data-ttu-id="22e64-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22e64-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22e64-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22e64-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="22e64-167">False</span><span class="sxs-lookup"><span data-stu-id="22e64-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22e64-168">См. также</span><span class="sxs-lookup"><span data-stu-id="22e64-168">See also</span></span>

- [<span data-ttu-id="22e64-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="22e64-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

