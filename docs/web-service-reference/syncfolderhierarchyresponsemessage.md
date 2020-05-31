---
title: синкфолдерхиерарчиреспонсемессаже
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
description: Элемент Синкфолдерхиерарчиреспонсемессаже содержит состояние и результат одного запроса операции SyncFolderHierarchy.
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840125"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="a08d0-103">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a08d0-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="a08d0-104">Элемент **синкфолдерхиерарчиреспонсемессаже** содержит состояние и результат одного запроса [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a08d0-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a08d0-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a08d0-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="a08d0-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a08d0-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a08d0-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a08d0-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
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

 <span data-ttu-id="a08d0-108">**синкфолдерхиерарчиреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="a08d0-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a08d0-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a08d0-109">Attributes and elements</span></span>

<span data-ttu-id="a08d0-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a08d0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a08d0-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a08d0-111">Attributes</span></span>

|<span data-ttu-id="a08d0-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a08d0-112">**Attribute**</span></span>|<span data-ttu-id="a08d0-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a08d0-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a08d0-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="a08d0-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a08d0-115">Описывает состояние ответа [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a08d0-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a08d0-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="a08d0-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="a08d0-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="a08d0-117">-  Success</span></span>  <br/><span data-ttu-id="a08d0-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="a08d0-118">-  Warning</span></span>  <br/><span data-ttu-id="a08d0-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="a08d0-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a08d0-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="a08d0-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a08d0-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a08d0-121">**Value**</span></span>|<span data-ttu-id="a08d0-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a08d0-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a08d0-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="a08d0-123">**Success**</span></span> <br/> |<span data-ttu-id="a08d0-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="a08d0-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a08d0-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="a08d0-125">**Warning**</span></span> <br/> | <span data-ttu-id="a08d0-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="a08d0-126">Describes a request that was not processed.</span></span> <span data-ttu-id="a08d0-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="a08d0-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a08d0-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="a08d0-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a08d0-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="a08d0-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a08d0-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a08d0-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a08d0-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="a08d0-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a08d0-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a08d0-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a08d0-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="a08d0-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="a08d0-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="a08d0-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a08d0-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="a08d0-135">**Error**</span></span> <br/> | <span data-ttu-id="a08d0-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="a08d0-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a08d0-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="a08d0-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a08d0-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="a08d0-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a08d0-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="a08d0-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="a08d0-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="a08d0-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="a08d0-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="a08d0-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="a08d0-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="a08d0-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a08d0-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="a08d0-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="a08d0-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a08d0-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a08d0-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a08d0-145">Child elements</span></span>

|<span data-ttu-id="a08d0-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a08d0-146">**Element**</span></span>|<span data-ttu-id="a08d0-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a08d0-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a08d0-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="a08d0-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a08d0-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="a08d0-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a08d0-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a08d0-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="a08d0-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="a08d0-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a08d0-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="a08d0-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a08d0-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="a08d0-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="a08d0-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a08d0-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a08d0-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-157">синкстате</span><span class="sxs-lookup"><span data-stu-id="a08d0-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a08d0-158">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="a08d0-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="a08d0-159">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a08d0-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-160">инклудесластфолдеринранже</span><span class="sxs-lookup"><span data-stu-id="a08d0-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="a08d0-161">Указывает, включен ли в ответ последний элемент для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a08d0-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="a08d0-162">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="a08d0-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="a08d0-163">Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="a08d0-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a08d0-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a08d0-164">Parent elements</span></span>

|<span data-ttu-id="a08d0-165">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a08d0-165">**Element**</span></span>|<span data-ttu-id="a08d0-166">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a08d0-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a08d0-167">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a08d0-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a08d0-168">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="a08d0-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a08d0-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="a08d0-169">Remarks</span></span>

<span data-ttu-id="a08d0-170">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a08d0-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a08d0-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a08d0-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a08d0-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a08d0-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a08d0-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a08d0-173">Schema Name</span></span>  <br/> |<span data-ttu-id="a08d0-174">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a08d0-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a08d0-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a08d0-175">Validation File</span></span>  <br/> |<span data-ttu-id="a08d0-176">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a08d0-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a08d0-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a08d0-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="a08d0-178">False</span><span class="sxs-lookup"><span data-stu-id="a08d0-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a08d0-179">См. также</span><span class="sxs-lookup"><span data-stu-id="a08d0-179">See also</span></span>

- [<span data-ttu-id="a08d0-180">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a08d0-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="a08d0-181">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a08d0-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

