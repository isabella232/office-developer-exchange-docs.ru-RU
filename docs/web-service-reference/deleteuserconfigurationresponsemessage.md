---
title: DeleteUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 543b1743-7e1c-4acb-93bd-34532e7fe79b
description: Элемент DeleteUserConfigurationResponseMessage содержит состояние и результат одного запроса DeleteUserConfiguration.
ms.openlocfilehash: 3e07917688ad1f25f7ca3fa06d6db51cf9905503
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762058"
---
# <a name="deleteuserconfigurationresponsemessage"></a><span data-ttu-id="b1590-103">DeleteUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b1590-103">DeleteUserConfigurationResponseMessage</span></span>

<span data-ttu-id="b1590-104">Элемент **DeleteUserConfigurationResponseMessage** содержит состояние и результат одного запроса **DeleteUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="b1590-104">The **DeleteUserConfigurationResponseMessage** element contains the status and result of a single **DeleteUserConfiguration** request.</span></span> 
  
```xml
<DeleteUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteUserConfigurationResponseMessage>
```

 <span data-ttu-id="b1590-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b1590-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1590-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b1590-106">Attributes and elements</span></span>

<span data-ttu-id="b1590-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b1590-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1590-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b1590-108">Attributes</span></span>

|<span data-ttu-id="b1590-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b1590-109">**Attribute**</span></span>|<span data-ttu-id="b1590-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1590-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1590-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b1590-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b1590-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="b1590-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="b1590-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="b1590-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="b1590-114">-Success</span><span class="sxs-lookup"><span data-stu-id="b1590-114">-  Success</span></span>  <br/><span data-ttu-id="b1590-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="b1590-115">-  Warning</span></span>  <br/><span data-ttu-id="b1590-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="b1590-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b1590-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b1590-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b1590-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b1590-118">**Value**</span></span>|<span data-ttu-id="b1590-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1590-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1590-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="b1590-120">**Success**</span></span> <br/> |<span data-ttu-id="b1590-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="b1590-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b1590-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="b1590-122">**Warning**</span></span> <br/> | <span data-ttu-id="b1590-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="b1590-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b1590-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="b1590-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="b1590-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="b1590-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="b1590-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="b1590-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b1590-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b1590-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b1590-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="b1590-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b1590-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b1590-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b1590-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="b1590-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b1590-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="b1590-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b1590-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="b1590-132">**Error**</span></span> <br/> | <span data-ttu-id="b1590-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="b1590-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="b1590-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="b1590-134">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="b1590-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b1590-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b1590-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="b1590-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b1590-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="b1590-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b1590-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="b1590-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b1590-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="b1590-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b1590-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="b1590-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="b1590-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="b1590-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b1590-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b1590-142">Child elements</span></span>

|<span data-ttu-id="b1590-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b1590-143">**Element**</span></span>|<span data-ttu-id="b1590-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1590-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1590-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b1590-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b1590-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="b1590-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b1590-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b1590-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b1590-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="b1590-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b1590-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b1590-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b1590-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="b1590-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b1590-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="b1590-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b1590-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b1590-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b1590-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="b1590-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1590-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b1590-154">Parent elements</span></span>

|<span data-ttu-id="b1590-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b1590-155">**Element**</span></span>|<span data-ttu-id="b1590-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1590-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1590-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b1590-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b1590-158">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1590-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b1590-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b1590-159">Text value</span></span>

<span data-ttu-id="b1590-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1590-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b1590-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="b1590-161">Remarks</span></span>

<span data-ttu-id="b1590-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1590-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1590-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b1590-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1590-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b1590-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b1590-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b1590-165">Schema Name</span></span>  <br/> |<span data-ttu-id="b1590-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b1590-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b1590-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b1590-167">Validation File</span></span>  <br/> |<span data-ttu-id="b1590-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b1590-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b1590-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b1590-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="b1590-170">False</span><span class="sxs-lookup"><span data-stu-id="b1590-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b1590-171">См. также</span><span class="sxs-lookup"><span data-stu-id="b1590-171">See also</span></span>

- [<span data-ttu-id="b1590-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b1590-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

