---
title: GetServiceConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfigurationResponse
api_type:
- schema
ms.assetid: 313dac99-0e5c-4198-bafa-89e749934ac7
description: Элемент GetServiceConfigurationResponse определяет ответ на запрос GetServiceConfiguration.
ms.openlocfilehash: 7abc81222125334de2a6ab6e4a618b48fe0caf4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833668"
---
# <a name="getserviceconfigurationresponse"></a><span data-ttu-id="0e706-103">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="0e706-103">GetServiceConfigurationResponse</span></span>

<span data-ttu-id="0e706-104">Элемент **GetServiceConfigurationResponse** определяет ответ на запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e706-104">The **GetServiceConfigurationResponse** element defines a response to a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfigurationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResponseMessages/>
</GetServiceConfigurationResponse>
```

 <span data-ttu-id="0e706-105">**GetServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0e706-105">**GetServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e706-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e706-106">Attributes and elements</span></span>

<span data-ttu-id="0e706-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0e706-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e706-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e706-108">Attributes</span></span>

|<span data-ttu-id="0e706-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0e706-109">**Attribute**</span></span>|<span data-ttu-id="0e706-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e706-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0e706-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0e706-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0e706-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="0e706-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0e706-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="0e706-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0e706-114">-Success</span><span class="sxs-lookup"><span data-stu-id="0e706-114">-  Success</span></span>  <br/><span data-ttu-id="0e706-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="0e706-115">-  Warning</span></span>  <br/><span data-ttu-id="0e706-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="0e706-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0e706-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0e706-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="0e706-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0e706-118">**Value**</span></span>|<span data-ttu-id="0e706-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e706-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0e706-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="0e706-120">**Success**</span></span> <br/> |<span data-ttu-id="0e706-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="0e706-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0e706-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="0e706-122">**Warning**</span></span> <br/> | <span data-ttu-id="0e706-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="0e706-123">Describes a request that was not processed.</span></span> <span data-ttu-id="0e706-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="0e706-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0e706-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="0e706-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0e706-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="0e706-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0e706-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0e706-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0e706-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="0e706-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0e706-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0e706-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0e706-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="0e706-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="0e706-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="0e706-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0e706-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="0e706-132">**Error**</span></span> <br/> | <span data-ttu-id="0e706-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="0e706-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0e706-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="0e706-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0e706-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e706-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0e706-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="0e706-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0e706-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="0e706-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="0e706-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="0e706-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="0e706-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="0e706-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0e706-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="0e706-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="0e706-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="0e706-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0e706-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e706-142">Child elements</span></span>

|<span data-ttu-id="0e706-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e706-143">**Element**</span></span>|<span data-ttu-id="0e706-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e706-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e706-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="0e706-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0e706-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="0e706-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0e706-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0e706-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0e706-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="0e706-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0e706-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0e706-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0e706-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="0e706-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="0e706-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="0e706-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0e706-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0e706-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0e706-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="0e706-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0e706-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="0e706-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="0e706-155">Содержит массив сообщений ответа конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="0e706-155">Contains an array of service configuration response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e706-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e706-156">Parent elements</span></span>

<span data-ttu-id="0e706-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e706-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0e706-158">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0e706-158">Text value</span></span>

<span data-ttu-id="0e706-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e706-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e706-160">Замечания</span><span class="sxs-lookup"><span data-stu-id="0e706-160">Remarks</span></span>

<span data-ttu-id="0e706-161">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e706-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e706-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e706-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e706-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e706-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e706-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e706-164">Schema Name</span></span>  <br/> |<span data-ttu-id="0e706-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0e706-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0e706-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e706-166">Validation File</span></span>  <br/> |<span data-ttu-id="0e706-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0e706-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e706-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e706-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e706-169">False</span><span class="sxs-lookup"><span data-stu-id="0e706-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e706-170">См. также</span><span class="sxs-lookup"><span data-stu-id="0e706-170">See also</span></span>

- [<span data-ttu-id="0e706-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0e706-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

