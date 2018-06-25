---
title: RefreshSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponseMessage
api_type:
- schema
ms.assetid: 53ee65bd-cf75-4e04-9b27-eff1b040ae82
description: Элемент RefreshSharingFolderResponseMessage содержит состояние и результат одного запроса RefreshSharingFolder операции.
ms.openlocfilehash: 9dbb66c294439f33a9307d51c03dd1cd127e95e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835052"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="e16b3-103">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e16b3-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="e16b3-104">Элемент **RefreshSharingFolderResponseMessage** содержит состояние и результат одного запроса [RefreshSharingFolder операции](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e16b3-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="e16b3-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e16b3-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e16b3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e16b3-106">Attributes and elements</span></span>

<span data-ttu-id="e16b3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e16b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e16b3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e16b3-108">Attributes</span></span>

|<span data-ttu-id="e16b3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e16b3-109">**Attribute**</span></span>|<span data-ttu-id="e16b3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e16b3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e16b3-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e16b3-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e16b3-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e16b3-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="e16b3-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e16b3-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e16b3-114">-Success</span><span class="sxs-lookup"><span data-stu-id="e16b3-114">-  Success</span></span>  <br/><span data-ttu-id="e16b3-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e16b3-115">-  Warning</span></span>  <br/><span data-ttu-id="e16b3-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="e16b3-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e16b3-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e16b3-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="e16b3-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e16b3-118">**Value**</span></span>|<span data-ttu-id="e16b3-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e16b3-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e16b3-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="e16b3-120">**Success**</span></span> <br/> |<span data-ttu-id="e16b3-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="e16b3-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e16b3-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="e16b3-122">**Warning**</span></span> <br/> | <span data-ttu-id="e16b3-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e16b3-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e16b3-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="e16b3-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e16b3-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="e16b3-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="e16b3-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="e16b3-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e16b3-127">-К службе каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e16b3-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="e16b3-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="e16b3-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e16b3-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e16b3-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e16b3-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="e16b3-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e16b3-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="e16b3-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="e16b3-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="e16b3-132">**Error**</span></span> <br/> | <span data-ttu-id="e16b3-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e16b3-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e16b3-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="e16b3-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e16b3-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e16b3-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e16b3-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="e16b3-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e16b3-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e16b3-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e16b3-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="e16b3-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e16b3-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="e16b3-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e16b3-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="e16b3-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="e16b3-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="e16b3-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e16b3-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e16b3-142">Child elements</span></span>

|<span data-ttu-id="e16b3-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e16b3-143">**Element**</span></span>|<span data-ttu-id="e16b3-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e16b3-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e16b3-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="e16b3-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e16b3-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e16b3-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e16b3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e16b3-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e16b3-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="e16b3-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e16b3-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e16b3-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e16b3-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e16b3-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="e16b3-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e16b3-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e16b3-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e16b3-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e16b3-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e16b3-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e16b3-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e16b3-154">Parent elements</span></span>

|<span data-ttu-id="e16b3-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e16b3-155">**Element**</span></span>|<span data-ttu-id="e16b3-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e16b3-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e16b3-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e16b3-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e16b3-158">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e16b3-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e16b3-159">Замечания</span><span class="sxs-lookup"><span data-stu-id="e16b3-159">Remarks</span></span>

<span data-ttu-id="e16b3-160">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e16b3-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e16b3-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e16b3-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e16b3-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e16b3-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e16b3-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e16b3-163">Schema Name</span></span>  <br/> |<span data-ttu-id="e16b3-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e16b3-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e16b3-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e16b3-165">Validation File</span></span>  <br/> |<span data-ttu-id="e16b3-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e16b3-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e16b3-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e16b3-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="e16b3-168">False</span><span class="sxs-lookup"><span data-stu-id="e16b3-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e16b3-169">См. также</span><span class="sxs-lookup"><span data-stu-id="e16b3-169">See also</span></span>

- [<span data-ttu-id="e16b3-170">Операция RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e16b3-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="e16b3-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e16b3-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

