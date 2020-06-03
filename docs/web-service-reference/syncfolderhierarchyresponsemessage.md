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
ms.openlocfilehash: fda0a37178f89ba0fd5ef860f8b009f335a11391
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465347"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="9f993-103">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9f993-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="9f993-104">Элемент **синкфолдерхиерарчиреспонсемессаже** содержит состояние и результат одного запроса [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f993-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="9f993-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="9f993-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="9f993-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="9f993-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="9f993-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9f993-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
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

 <span data-ttu-id="9f993-108">**синкфолдерхиерарчиреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="9f993-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f993-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9f993-109">Attributes and elements</span></span>

<span data-ttu-id="9f993-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9f993-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f993-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9f993-111">Attributes</span></span>

|<span data-ttu-id="9f993-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9f993-112">**Attribute**</span></span>|<span data-ttu-id="9f993-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f993-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f993-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="9f993-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9f993-115">Описывает состояние ответа [операции SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f993-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9f993-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="9f993-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="9f993-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="9f993-117">-  Success</span></span>  <br/><span data-ttu-id="9f993-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="9f993-118">-  Warning</span></span>  <br/><span data-ttu-id="9f993-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="9f993-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9f993-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="9f993-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="9f993-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9f993-121">**Value**</span></span>|<span data-ttu-id="9f993-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f993-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f993-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="9f993-123">**Success**</span></span> <br/> |<span data-ttu-id="9f993-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="9f993-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9f993-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9f993-125">**Warning**</span></span> <br/> | <span data-ttu-id="9f993-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="9f993-126">Describes a request that was not processed.</span></span> <span data-ttu-id="9f993-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="9f993-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9f993-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="9f993-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9f993-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="9f993-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9f993-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f993-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9f993-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="9f993-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9f993-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f993-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9f993-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="9f993-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="9f993-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="9f993-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9f993-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="9f993-135">**Error**</span></span> <br/> | <span data-ttu-id="9f993-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="9f993-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9f993-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="9f993-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9f993-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="9f993-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9f993-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="9f993-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9f993-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="9f993-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="9f993-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="9f993-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9f993-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="9f993-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9f993-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="9f993-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9f993-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9f993-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f993-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9f993-145">Child elements</span></span>

|<span data-ttu-id="9f993-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f993-146">**Element**</span></span>|<span data-ttu-id="9f993-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f993-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f993-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="9f993-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9f993-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="9f993-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9f993-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="9f993-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9f993-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="9f993-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9f993-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="9f993-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9f993-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="9f993-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9f993-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="9f993-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9f993-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="9f993-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9f993-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="9f993-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9f993-157">синкстате</span><span class="sxs-lookup"><span data-stu-id="9f993-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9f993-158">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="9f993-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="9f993-159">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9f993-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="9f993-160">инклудесластфолдеринранже</span><span class="sxs-lookup"><span data-stu-id="9f993-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="9f993-161">Указывает, включен ли в ответ последний элемент для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9f993-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="9f993-162">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="9f993-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="9f993-163">Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f993-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f993-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9f993-164">Parent elements</span></span>

|<span data-ttu-id="9f993-165">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f993-165">**Element**</span></span>|<span data-ttu-id="9f993-166">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f993-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f993-167">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="9f993-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f993-168">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f993-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f993-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="9f993-169">Remarks</span></span>

<span data-ttu-id="9f993-170">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9f993-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f993-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9f993-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f993-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9f993-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f993-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9f993-173">Schema Name</span></span>  <br/> |<span data-ttu-id="9f993-174">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9f993-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f993-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9f993-175">Validation File</span></span>  <br/> |<span data-ttu-id="9f993-176">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9f993-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f993-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9f993-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f993-178">False</span><span class="sxs-lookup"><span data-stu-id="9f993-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f993-179">См. также</span><span class="sxs-lookup"><span data-stu-id="9f993-179">See also</span></span>

- [<span data-ttu-id="9f993-180">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="9f993-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="9f993-181">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9f993-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

