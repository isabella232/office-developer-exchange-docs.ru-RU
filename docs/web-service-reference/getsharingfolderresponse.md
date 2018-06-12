---
title: GetSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponse
api_type:
- schema
ms.assetid: fee90e84-3ad4-4c4b-831f-bbc95070aebf
description: Элемент GetSharingFolderResponse определяет ответ на запрос операции GetSharingFolder.
ms.openlocfilehash: 6d847f1bd80105d52d564770c65b342c89385dad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833675"
---
# <a name="getsharingfolderresponse"></a><span data-ttu-id="b899a-103">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b899a-103">GetSharingFolderResponse</span></span>

<span data-ttu-id="b899a-104">Элемент **GetSharingFolderResponse** определяет ответ на запрос [GetSharingFolder операции](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b899a-104">The **GetSharingFolderResponse** element defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```XML
<GetSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponse>
```

 <span data-ttu-id="b899a-105">**GetSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b899a-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b899a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b899a-106">Attributes and elements</span></span>

<span data-ttu-id="b899a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b899a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b899a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b899a-108">Attributes</span></span>

|<span data-ttu-id="b899a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b899a-109">**Attribute**</span></span>|<span data-ttu-id="b899a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b899a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b899a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b899a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b899a-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="b899a-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="b899a-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="b899a-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b899a-114">-Success</span><span class="sxs-lookup"><span data-stu-id="b899a-114">-  Success</span></span>  <br/><span data-ttu-id="b899a-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="b899a-115">-  Warning</span></span>  <br/><span data-ttu-id="b899a-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="b899a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b899a-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b899a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b899a-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b899a-118">**Value**</span></span>|<span data-ttu-id="b899a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b899a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b899a-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="b899a-120">**Success**</span></span> <br/> |<span data-ttu-id="b899a-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="b899a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b899a-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="b899a-122">**Warning**</span></span> <br/> | <span data-ttu-id="b899a-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="b899a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b899a-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="b899a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b899a-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="b899a-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b899a-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="b899a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b899a-127">-Служба каталогов Active Directory или доменных служб Active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b899a-127">-  The Active Directory directory service or Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b899a-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="b899a-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b899a-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b899a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b899a-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="b899a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b899a-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="b899a-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b899a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="b899a-132">**Error**</span></span> <br/> | <span data-ttu-id="b899a-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="b899a-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b899a-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="b899a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b899a-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b899a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b899a-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="b899a-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b899a-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="b899a-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b899a-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="b899a-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b899a-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="b899a-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b899a-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="b899a-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b899a-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="b899a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b899a-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b899a-142">Child elements</span></span>

|<span data-ttu-id="b899a-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b899a-143">**Element**</span></span>|<span data-ttu-id="b899a-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b899a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b899a-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b899a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b899a-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="b899a-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b899a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b899a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b899a-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="b899a-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b899a-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b899a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b899a-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="b899a-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b899a-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="b899a-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b899a-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b899a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b899a-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="b899a-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b899a-154">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="b899a-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="b899a-155">Представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="b899a-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b899a-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b899a-156">Parent elements</span></span>

<span data-ttu-id="b899a-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="b899a-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b899a-158">Замечания</span><span class="sxs-lookup"><span data-stu-id="b899a-158">Remarks</span></span>

<span data-ttu-id="b899a-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b899a-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b899a-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b899a-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b899a-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b899a-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b899a-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b899a-162">Schema Name</span></span>  <br/> |<span data-ttu-id="b899a-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b899a-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b899a-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b899a-164">Validation File</span></span>  <br/> |<span data-ttu-id="b899a-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b899a-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b899a-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b899a-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="b899a-167">False</span><span class="sxs-lookup"><span data-stu-id="b899a-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b899a-168">См. также</span><span class="sxs-lookup"><span data-stu-id="b899a-168">See also</span></span>

- [<span data-ttu-id="b899a-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b899a-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

