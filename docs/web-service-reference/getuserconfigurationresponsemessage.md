---
title: GetUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: f75e29eb-ae98-46fd-8da2-1c76a57f5458
description: Элемент GetUserConfigurationResponseMessage представляет ответа, которое возвращает объект конфигурации пользователя.
ms.openlocfilehash: 28c14d11218294bd8dd64f70e755cda8f8335856
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833690"
---
# <a name="getuserconfigurationresponsemessage"></a><span data-ttu-id="d0ad9-103">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d0ad9-103">GetUserConfigurationResponseMessage</span></span>

<span data-ttu-id="d0ad9-104">Элемент **GetUserConfigurationResponseMessage** представляет ответа, которое возвращает объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-104">The **GetUserConfigurationResponseMessage** element represents a response that returns a user configuration object.</span></span> 
  
```xml
<GetUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <UserConfiguration/>
</GetUserConfigurationResponseMessage>
```

 <span data-ttu-id="d0ad9-105">**GetUserConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-105">**GetUserConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0ad9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0ad9-106">Attributes and elements</span></span>

<span data-ttu-id="d0ad9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0ad9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d0ad9-108">Attributes</span></span>

|<span data-ttu-id="d0ad9-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-109">**Attribute**</span></span>|<span data-ttu-id="d0ad9-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0ad9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d0ad9-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d0ad9-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d0ad9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d0ad9-114">-Success</span><span class="sxs-lookup"><span data-stu-id="d0ad9-114">-  Success</span></span>  <br/><span data-ttu-id="d0ad9-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d0ad9-115">-  Warning</span></span>  <br/><span data-ttu-id="d0ad9-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d0ad9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d0ad9-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d0ad9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d0ad9-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-118">**Value**</span></span>|<span data-ttu-id="d0ad9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d0ad9-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-120">**Success**</span></span> <br/> |<span data-ttu-id="d0ad9-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d0ad9-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-122">**Warning**</span></span> <br/> | <span data-ttu-id="d0ad9-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d0ad9-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d0ad9-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="d0ad9-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d0ad9-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d0ad9-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d0ad9-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d0ad9-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d0ad9-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d0ad9-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d0ad9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-132">**Error**</span></span> <br/> | <span data-ttu-id="d0ad9-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="d0ad9-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d0ad9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d0ad9-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0ad9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d0ad9-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d0ad9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d0ad9-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d0ad9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d0ad9-138">-Атрибута или элемента не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d0ad9-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="d0ad9-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="d0ad9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d0ad9-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d0ad9-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d0ad9-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d0ad9-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d0ad9-142">Child elements</span></span>

|<span data-ttu-id="d0ad9-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-143">**Element**</span></span>|<span data-ttu-id="d0ad9-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0ad9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d0ad9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d0ad9-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d0ad9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d0ad9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d0ad9-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d0ad9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d0ad9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d0ad9-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d0ad9-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d0ad9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d0ad9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d0ad9-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d0ad9-154">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0ad9-154">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="d0ad9-155">Содержит объект конфигурации одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-155">Contains a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0ad9-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d0ad9-156">Parent elements</span></span>

|<span data-ttu-id="d0ad9-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-157">**Element**</span></span>|<span data-ttu-id="d0ad9-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0ad9-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0ad9-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d0ad9-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d0ad9-160">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0ad9-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d0ad9-161">Text value</span></span>

<span data-ttu-id="d0ad9-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0ad9-163">Замечания</span><span class="sxs-lookup"><span data-stu-id="d0ad9-163">Remarks</span></span>

<span data-ttu-id="d0ad9-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0ad9-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0ad9-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d0ad9-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0ad9-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d0ad9-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0ad9-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d0ad9-167">Schema Name</span></span>  <br/> |<span data-ttu-id="d0ad9-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d0ad9-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0ad9-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d0ad9-169">Validation File</span></span>  <br/> |<span data-ttu-id="d0ad9-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0ad9-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0ad9-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d0ad9-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0ad9-172">False</span><span class="sxs-lookup"><span data-stu-id="d0ad9-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0ad9-173">См. также</span><span class="sxs-lookup"><span data-stu-id="d0ad9-173">See also</span></span>

- [<span data-ttu-id="d0ad9-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d0ad9-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

