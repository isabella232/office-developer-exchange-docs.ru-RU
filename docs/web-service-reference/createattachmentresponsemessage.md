---
title: креатеаттачментреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: Элемент Креатеаттачментреспонсемессаже содержит состояние и результат одного запроса операции CreateAttachment.
ms.openlocfilehash: 14d8d1936b3cfd52bdb816343c86606cb8ccf76f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458924"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="7812c-103">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7812c-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="7812c-104">Элемент **креатеаттачментреспонсемессаже** содержит состояние и результат одного запроса [операции CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7812c-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="7812c-105">креатеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="7812c-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="7812c-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7812c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="7812c-107">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7812c-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="7812c-108">**аттачментинфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="7812c-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7812c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7812c-109">Attributes and elements</span></span>

<span data-ttu-id="7812c-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7812c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7812c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7812c-111">Attributes</span></span>

|<span data-ttu-id="7812c-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7812c-112">**Attribute**</span></span>|<span data-ttu-id="7812c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7812c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7812c-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="7812c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7812c-115">Описывает состояние ответа [операции CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7812c-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7812c-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="7812c-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="7812c-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="7812c-117">-  Success</span></span>  <br/><span data-ttu-id="7812c-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="7812c-118">-  Warning</span></span>  <br/><span data-ttu-id="7812c-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="7812c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7812c-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="7812c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="7812c-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7812c-121">**Value**</span></span>|<span data-ttu-id="7812c-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7812c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7812c-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="7812c-123">**Success**</span></span> <br/> |<span data-ttu-id="7812c-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="7812c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7812c-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7812c-125">**Warning**</span></span> <br/> | <span data-ttu-id="7812c-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="7812c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="7812c-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="7812c-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="7812c-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="7812c-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="7812c-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="7812c-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7812c-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7812c-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7812c-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="7812c-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7812c-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7812c-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7812c-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="7812c-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="7812c-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="7812c-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7812c-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="7812c-135">**Error**</span></span> <br/> | <span data-ttu-id="7812c-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="7812c-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="7812c-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="7812c-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7812c-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="7812c-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7812c-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="7812c-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7812c-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="7812c-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="7812c-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="7812c-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7812c-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="7812c-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7812c-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="7812c-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="7812c-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7812c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7812c-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7812c-145">Child elements</span></span>

|<span data-ttu-id="7812c-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7812c-146">**Element**</span></span>|<span data-ttu-id="7812c-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7812c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7812c-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7812c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7812c-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="7812c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7812c-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7812c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7812c-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="7812c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7812c-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7812c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7812c-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="7812c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7812c-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="7812c-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7812c-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="7812c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7812c-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7812c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7812c-157">Вложения</span><span class="sxs-lookup"><span data-stu-id="7812c-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7812c-158">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7812c-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7812c-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7812c-159">Parent elements</span></span>

|<span data-ttu-id="7812c-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7812c-160">**Element**</span></span>|<span data-ttu-id="7812c-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7812c-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7812c-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7812c-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7812c-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7812c-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7812c-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="7812c-164">Remarks</span></span>

<span data-ttu-id="7812c-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7812c-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7812c-166">Если к элементу присоединяется несколько вложений, в последнем ответе используется атрибут **рутитемчанжекэй** , представляющий новый ключ изменения элемента с вложениями.</span><span class="sxs-lookup"><span data-stu-id="7812c-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7812c-167">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7812c-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7812c-168">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7812c-168">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7812c-169">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7812c-169">Schema Name</span></span>  <br/> |<span data-ttu-id="7812c-170">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7812c-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7812c-171">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7812c-171">Validation File</span></span>  <br/> |<span data-ttu-id="7812c-172">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7812c-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7812c-173">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7812c-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="7812c-174">False</span><span class="sxs-lookup"><span data-stu-id="7812c-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7812c-175">См. также</span><span class="sxs-lookup"><span data-stu-id="7812c-175">See also</span></span>

- [<span data-ttu-id="7812c-176">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7812c-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="7812c-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7812c-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="7812c-178">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="7812c-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="7812c-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7812c-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

