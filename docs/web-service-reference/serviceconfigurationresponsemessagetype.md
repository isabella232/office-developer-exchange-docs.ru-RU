---
title: ServiceConfigurationResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: Элемент ServiceConfigurationResponseMessageType содержит параметры конфигурации службы.
ms.openlocfilehash: fb7841f346083017319cece4479fea8bbfb6de17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835393"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="d32e9-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="d32e9-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="d32e9-104">Элемент **ServiceConfigurationResponseMessageType** содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="d32e9-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="d32e9-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d32e9-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d32e9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d32e9-106">Attributes and elements</span></span>

<span data-ttu-id="d32e9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d32e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d32e9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d32e9-108">Attributes</span></span>

|<span data-ttu-id="d32e9-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d32e9-109">**Attribute**</span></span>|<span data-ttu-id="d32e9-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d32e9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d32e9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d32e9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d32e9-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d32e9-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="d32e9-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d32e9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d32e9-114">-Success</span><span class="sxs-lookup"><span data-stu-id="d32e9-114">-  Success</span></span>  <br/><span data-ttu-id="d32e9-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d32e9-115">-  Warning</span></span>  <br/><span data-ttu-id="d32e9-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d32e9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d32e9-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d32e9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d32e9-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d32e9-118">**Value**</span></span>|<span data-ttu-id="d32e9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d32e9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d32e9-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="d32e9-120">**Success**</span></span> <br/> |<span data-ttu-id="d32e9-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d32e9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d32e9-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="d32e9-122">**Warning**</span></span> <br/> | <span data-ttu-id="d32e9-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d32e9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d32e9-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d32e9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d32e9-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="d32e9-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d32e9-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d32e9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d32e9-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d32e9-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d32e9-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="d32e9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d32e9-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d32e9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d32e9-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d32e9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d32e9-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="d32e9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d32e9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d32e9-132">**Error**</span></span> <br/> | <span data-ttu-id="d32e9-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d32e9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d32e9-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d32e9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d32e9-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d32e9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d32e9-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d32e9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d32e9-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d32e9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d32e9-138">-Атрибута или элемента не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d32e9-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="d32e9-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="d32e9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d32e9-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d32e9-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d32e9-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d32e9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d32e9-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d32e9-142">Child elements</span></span>

|<span data-ttu-id="d32e9-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d32e9-143">**Element**</span></span>|<span data-ttu-id="d32e9-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d32e9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d32e9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d32e9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d32e9-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d32e9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d32e9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d32e9-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d32e9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d32e9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d32e9-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d32e9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d32e9-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d32e9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d32e9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d32e9-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d32e9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="d32e9-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="d32e9-155">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="d32e9-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="d32e9-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="d32e9-157">Содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d32e9-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="d32e9-158">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="d32e9-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="d32e9-159">Содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="d32e9-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d32e9-160">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d32e9-160">Parent elements</span></span>

|<span data-ttu-id="d32e9-161">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d32e9-161">**Element**</span></span>|<span data-ttu-id="d32e9-162">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d32e9-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d32e9-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="d32e9-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="d32e9-164">Содержит массив сообщений ответа конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="d32e9-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d32e9-165">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d32e9-165">Text value</span></span>

<span data-ttu-id="d32e9-166">Нет.</span><span class="sxs-lookup"><span data-stu-id="d32e9-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d32e9-167">Замечания</span><span class="sxs-lookup"><span data-stu-id="d32e9-167">Remarks</span></span>

<span data-ttu-id="d32e9-168">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d32e9-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d32e9-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d32e9-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d32e9-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d32e9-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d32e9-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d32e9-171">Schema Name</span></span>  <br/> |<span data-ttu-id="d32e9-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d32e9-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d32e9-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d32e9-173">Validation File</span></span>  <br/> |<span data-ttu-id="d32e9-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d32e9-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d32e9-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d32e9-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="d32e9-176">False</span><span class="sxs-lookup"><span data-stu-id="d32e9-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d32e9-177">См. также</span><span class="sxs-lookup"><span data-stu-id="d32e9-177">See also</span></span>

- [<span data-ttu-id="d32e9-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d32e9-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

