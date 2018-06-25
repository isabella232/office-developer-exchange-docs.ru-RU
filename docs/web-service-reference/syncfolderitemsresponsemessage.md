---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: Элемент SyncFolderItemsResponseMessage содержит состояние и результат одного запроса SyncFolderItems операции.
ms.openlocfilehash: 9bb32232143df56ad9de93480e10a5941e68025a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840132"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="0ffd3-103">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ffd3-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="0ffd3-104">Элемент **SyncFolderItemsResponseMessage** содержит состояние и результат одного запроса [SyncFolderItems операции](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ffd3-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0ffd3-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0ffd3-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="0ffd3-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ffd3-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0ffd3-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ffd3-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 <span data-ttu-id="0ffd3-108">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ffd3-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ffd3-109">Attributes and elements</span></span>

<span data-ttu-id="0ffd3-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ffd3-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ffd3-111">Attributes</span></span>

|<span data-ttu-id="0ffd3-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-112">**Attribute**</span></span>|<span data-ttu-id="0ffd3-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ffd3-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0ffd3-115">Описание состояния ответа [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ffd3-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0ffd3-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="0ffd3-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="0ffd3-117">-Success</span><span class="sxs-lookup"><span data-stu-id="0ffd3-117">-  Success</span></span>  <br/><span data-ttu-id="0ffd3-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="0ffd3-118">-  Warning</span></span>  <br/><span data-ttu-id="0ffd3-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="0ffd3-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="0ffd3-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0ffd3-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="0ffd3-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-121">**Value**</span></span>|<span data-ttu-id="0ffd3-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ffd3-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-123">**Success**</span></span> <br/> |<span data-ttu-id="0ffd3-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0ffd3-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-125">**Warning**</span></span> <br/> | <span data-ttu-id="0ffd3-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0ffd3-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента запроса и не может обработать последующие элементы.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="0ffd3-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="0ffd3-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0ffd3-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0ffd3-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0ffd3-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0ffd3-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0ffd3-133">-Истек срок действия пароль.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="0ffd3-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="0ffd3-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-135">**Error**</span></span> <br/> | <span data-ttu-id="0ffd3-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0ffd3-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="0ffd3-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0ffd3-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ffd3-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0ffd3-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="0ffd3-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0ffd3-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="0ffd3-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="0ffd3-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="0ffd3-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="0ffd3-142">-Любая попытка несанкционированного доступа любого клиента</span><span class="sxs-lookup"><span data-stu-id="0ffd3-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0ffd3-143">-Любые ошибки на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="0ffd3-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="0ffd3-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0ffd3-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ffd3-145">Child elements</span></span>

|<span data-ttu-id="0ffd3-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-146">**Element**</span></span>|<span data-ttu-id="0ffd3-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ffd3-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ffd3-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0ffd3-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ffd3-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0ffd3-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ffd3-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0ffd3-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0ffd3-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0ffd3-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0ffd3-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-157">Состояние</span><span class="sxs-lookup"><span data-stu-id="0ffd3-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ffd3-158">Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="0ffd3-159">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-160">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="0ffd3-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="0ffd3-161">Указывает, включены ли последнего элемента для синхронизации в ответе.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="0ffd3-162">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="0ffd3-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="0ffd3-163">Содержит массив последовательности типов изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ffd3-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ffd3-164">Parent elements</span></span>

|<span data-ttu-id="0ffd3-165">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-165">**Element**</span></span>|<span data-ttu-id="0ffd3-166">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ffd3-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ffd3-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ffd3-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0ffd3-168">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ffd3-169">Замечания</span><span class="sxs-lookup"><span data-stu-id="0ffd3-169">Remarks</span></span>

<span data-ttu-id="0ffd3-170">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0ffd3-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ffd3-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ffd3-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ffd3-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ffd3-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ffd3-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ffd3-173">Schema Name</span></span>  <br/> |<span data-ttu-id="0ffd3-174">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0ffd3-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ffd3-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ffd3-175">Validation File</span></span>  <br/> |<span data-ttu-id="0ffd3-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ffd3-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ffd3-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ffd3-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ffd3-178">False</span><span class="sxs-lookup"><span data-stu-id="0ffd3-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ffd3-179">См. также</span><span class="sxs-lookup"><span data-stu-id="0ffd3-179">See also</span></span>

- [<span data-ttu-id="0ffd3-180">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0ffd3-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="0ffd3-181">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0ffd3-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

