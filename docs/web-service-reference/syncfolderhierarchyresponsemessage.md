---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: Элемент SyncFolderHierarchyResponseMessage содержит состояние и результат одного запроса SyncFolderHierarchy операции.
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840125"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="ad010-103">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad010-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="ad010-104">Элемент **SyncFolderHierarchyResponseMessage** содержит состояние и результат одного запроса [SyncFolderHierarchy операции](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ad010-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ad010-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="ad010-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="ad010-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ad010-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ad010-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad010-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 <span data-ttu-id="ad010-108">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ad010-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad010-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad010-109">Attributes and elements</span></span>

<span data-ttu-id="ad010-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ad010-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad010-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad010-111">Attributes</span></span>

|<span data-ttu-id="ad010-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ad010-112">**Attribute**</span></span>|<span data-ttu-id="ad010-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad010-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ad010-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ad010-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ad010-115">Описание состояния ответа [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ad010-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="ad010-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ad010-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="ad010-117">-Success</span><span class="sxs-lookup"><span data-stu-id="ad010-117">-  Success</span></span>  <br/><span data-ttu-id="ad010-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="ad010-118">-  Warning</span></span>  <br/><span data-ttu-id="ad010-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="ad010-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ad010-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ad010-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="ad010-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ad010-121">**Value**</span></span>|<span data-ttu-id="ad010-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad010-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ad010-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="ad010-123">**Success**</span></span> <br/> |<span data-ttu-id="ad010-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="ad010-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ad010-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="ad010-125">**Warning**</span></span> <br/> | <span data-ttu-id="ad010-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="ad010-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ad010-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="ad010-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ad010-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="ad010-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ad010-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="ad010-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ad010-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ad010-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ad010-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="ad010-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ad010-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ad010-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ad010-133">-Истек срок действия пароль.</span><span class="sxs-lookup"><span data-stu-id="ad010-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="ad010-134">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="ad010-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="ad010-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="ad010-135">**Error**</span></span> <br/> | <span data-ttu-id="ad010-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="ad010-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ad010-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="ad010-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ad010-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad010-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ad010-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="ad010-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="ad010-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="ad010-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="ad010-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="ad010-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ad010-142">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="ad010-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ad010-143">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="ad010-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ad010-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="ad010-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ad010-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad010-145">Child elements</span></span>

|<span data-ttu-id="ad010-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad010-146">**Element**</span></span>|<span data-ttu-id="ad010-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad010-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad010-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ad010-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ad010-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="ad010-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ad010-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ad010-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ad010-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="ad010-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ad010-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ad010-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ad010-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="ad010-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ad010-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="ad010-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ad010-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ad010-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ad010-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="ad010-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ad010-157">Состояние</span><span class="sxs-lookup"><span data-stu-id="ad010-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ad010-158">Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="ad010-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="ad010-159">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ad010-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="ad010-160">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="ad010-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="ad010-161">Указывает, включены ли последнего элемента для синхронизации в ответе.</span><span class="sxs-lookup"><span data-stu-id="ad010-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="ad010-162">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="ad010-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="ad010-163">Содержит массив последовательности типов изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad010-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad010-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad010-164">Parent elements</span></span>

|<span data-ttu-id="ad010-165">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad010-165">**Element**</span></span>|<span data-ttu-id="ad010-166">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad010-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad010-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ad010-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ad010-168">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad010-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad010-169">Замечания</span><span class="sxs-lookup"><span data-stu-id="ad010-169">Remarks</span></span>

<span data-ttu-id="ad010-170">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ad010-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad010-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad010-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad010-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad010-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad010-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad010-173">Schema Name</span></span>  <br/> |<span data-ttu-id="ad010-174">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ad010-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad010-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad010-175">Validation File</span></span>  <br/> |<span data-ttu-id="ad010-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ad010-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad010-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad010-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad010-178">False</span><span class="sxs-lookup"><span data-stu-id="ad010-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad010-179">См. также</span><span class="sxs-lookup"><span data-stu-id="ad010-179">See also</span></span>

- [<span data-ttu-id="ad010-180">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="ad010-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="ad010-181">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad010-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

