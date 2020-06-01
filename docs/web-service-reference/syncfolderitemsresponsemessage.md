---
title: синкфолдеритемсреспонсемессаже
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
description: Элемент Синкфолдеритемсреспонсемессаже содержит состояние и результат одного запроса операции SyncFolderItems.
ms.openlocfilehash: 87de1b679fad4affa29a6dfdea72f5312b9191d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463043"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="e0853-103">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e0853-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="e0853-104">Элемент **синкфолдеритемсреспонсемессаже** содержит состояние и результат одного запроса [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e0853-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e0853-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e0853-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="e0853-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e0853-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="e0853-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e0853-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
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

 <span data-ttu-id="e0853-108">**синкфолдеритемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e0853-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0853-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0853-109">Attributes and elements</span></span>

<span data-ttu-id="e0853-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e0853-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0853-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0853-111">Attributes</span></span>

|<span data-ttu-id="e0853-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e0853-112">**Attribute**</span></span>|<span data-ttu-id="e0853-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0853-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0853-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="e0853-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e0853-115">Описывает состояние ответа [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e0853-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="e0853-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e0853-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="e0853-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e0853-117">-  Success</span></span>  <br/><span data-ttu-id="e0853-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e0853-118">-  Warning</span></span>  <br/><span data-ttu-id="e0853-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="e0853-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="e0853-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e0853-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="e0853-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e0853-121">**Value**</span></span>|<span data-ttu-id="e0853-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0853-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0853-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="e0853-123">**Success**</span></span> <br/> |<span data-ttu-id="e0853-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="e0853-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e0853-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e0853-125">**Warning**</span></span> <br/> | <span data-ttu-id="e0853-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e0853-126">Describes a request that was not processed.</span></span> <span data-ttu-id="e0853-127">Если при обработке элемента в запросе возникла ошибка, и последующие элементы не могут быть обработаны, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e0853-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="e0853-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="e0853-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e0853-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="e0853-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e0853-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e0853-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e0853-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="e0853-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e0853-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e0853-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e0853-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="e0853-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="e0853-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="e0853-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="e0853-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="e0853-135">**Error**</span></span> <br/> | <span data-ttu-id="e0853-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e0853-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e0853-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="e0853-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e0853-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="e0853-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e0853-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="e0853-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="e0853-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e0853-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="e0853-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="e0853-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="e0853-142">— Любой клиент пытается получить любой несанкционированный доступ.</span><span class="sxs-lookup"><span data-stu-id="e0853-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e0853-143">— Любой сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="e0853-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="e0853-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e0853-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e0853-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0853-145">Child elements</span></span>

|<span data-ttu-id="e0853-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0853-146">**Element**</span></span>|<span data-ttu-id="e0853-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0853-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0853-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e0853-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e0853-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e0853-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e0853-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e0853-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e0853-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="e0853-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e0853-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e0853-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e0853-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="e0853-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e0853-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e0853-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e0853-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e0853-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e0853-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e0853-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e0853-157">синкстате</span><span class="sxs-lookup"><span data-stu-id="e0853-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e0853-158">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="e0853-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="e0853-159">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e0853-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="e0853-160">инклудесластитеминранже</span><span class="sxs-lookup"><span data-stu-id="e0853-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="e0853-161">Указывает, включен ли в ответ последний элемент для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e0853-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="e0853-162">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="e0853-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="e0853-163">Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0853-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0853-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0853-164">Parent elements</span></span>

|<span data-ttu-id="e0853-165">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0853-165">**Element**</span></span>|<span data-ttu-id="e0853-166">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0853-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0853-167">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e0853-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e0853-168">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0853-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e0853-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="e0853-169">Remarks</span></span>

<span data-ttu-id="e0853-170">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e0853-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0853-171">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0853-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0853-172">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0853-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e0853-173">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0853-173">Schema Name</span></span>  <br/> |<span data-ttu-id="e0853-174">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e0853-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e0853-175">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0853-175">Validation File</span></span>  <br/> |<span data-ttu-id="e0853-176">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e0853-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e0853-177">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0853-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0853-178">False</span><span class="sxs-lookup"><span data-stu-id="e0853-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0853-179">См. также</span><span class="sxs-lookup"><span data-stu-id="e0853-179">See also</span></span>

- [<span data-ttu-id="e0853-180">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="e0853-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="e0853-181">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0853-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

