---
title: GetSharingMetadataResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponse
api_type:
- schema
ms.assetid: 1acc2d8f-7104-4b36-9c04-dd4fc4f571bb
description: Элемент GetSharingMetadataResponse определяет ответ на запрос операции GetSharingMetadata.
ms.openlocfilehash: 820b5bf7aa5528b61aa6649e5b1886885b5f022e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833676"
---
# <a name="getsharingmetadataresponse"></a><span data-ttu-id="d7530-103">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="d7530-103">GetSharingMetadataResponse</span></span>

<span data-ttu-id="d7530-104">Элемент **GetSharingMetadataResponse** определяет ответ на запрос [GetSharingMetadata операции](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7530-104">The **GetSharingMetadataResponse** element defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponse>
```

 <span data-ttu-id="d7530-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d7530-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7530-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7530-106">Attributes and elements</span></span>

<span data-ttu-id="d7530-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d7530-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7530-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d7530-108">Attributes</span></span>

|<span data-ttu-id="d7530-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d7530-109">**Attribute**</span></span>|<span data-ttu-id="d7530-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7530-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7530-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d7530-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d7530-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d7530-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d7530-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d7530-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d7530-114">-Success</span><span class="sxs-lookup"><span data-stu-id="d7530-114">-  Success</span></span>  <br/><span data-ttu-id="d7530-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d7530-115">-  Warning</span></span>  <br/><span data-ttu-id="d7530-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d7530-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d7530-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d7530-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d7530-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d7530-118">**Value**</span></span>|<span data-ttu-id="d7530-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7530-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7530-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="d7530-120">**Success**</span></span> <br/> |<span data-ttu-id="d7530-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d7530-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d7530-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="d7530-122">**Warning**</span></span> <br/> | <span data-ttu-id="d7530-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d7530-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d7530-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d7530-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d7530-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="d7530-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d7530-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d7530-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d7530-127">-К службе каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d7530-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="d7530-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="d7530-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d7530-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d7530-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d7530-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d7530-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d7530-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="d7530-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d7530-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d7530-132">**Error**</span></span> <br/> | <span data-ttu-id="d7530-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d7530-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d7530-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d7530-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d7530-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7530-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d7530-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d7530-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d7530-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d7530-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="d7530-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="d7530-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d7530-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="d7530-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d7530-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d7530-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="d7530-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d7530-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d7530-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d7530-142">Child elements</span></span>

|<span data-ttu-id="d7530-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7530-143">**Element**</span></span>|<span data-ttu-id="d7530-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7530-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7530-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7530-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d7530-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d7530-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d7530-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7530-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d7530-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d7530-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d7530-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7530-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d7530-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d7530-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d7530-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d7530-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d7530-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d7530-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d7530-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d7530-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d7530-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="d7530-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="d7530-155">Содержит коллекцию структур данных, которые клиент может использовать для авторизации, общий доступ к его календаря или контактов данных с помощью других клиентов.</span><span class="sxs-lookup"><span data-stu-id="d7530-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="d7530-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="d7530-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="d7530-157">Представляет получателей папки, общий доступ к запроса, которые являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="d7530-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7530-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d7530-158">Parent elements</span></span>

<span data-ttu-id="d7530-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="d7530-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d7530-160">Замечания</span><span class="sxs-lookup"><span data-stu-id="d7530-160">Remarks</span></span>

<span data-ttu-id="d7530-161">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d7530-161">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7530-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d7530-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7530-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d7530-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7530-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d7530-164">Schema Name</span></span>  <br/> |<span data-ttu-id="d7530-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d7530-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7530-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d7530-166">Validation File</span></span>  <br/> |<span data-ttu-id="d7530-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7530-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7530-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d7530-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7530-169">False</span><span class="sxs-lookup"><span data-stu-id="d7530-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7530-170">См. также</span><span class="sxs-lookup"><span data-stu-id="d7530-170">See also</span></span>

- [<span data-ttu-id="d7530-171">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d7530-171">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="d7530-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d7530-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

