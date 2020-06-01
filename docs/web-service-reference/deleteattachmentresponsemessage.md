---
title: делетеаттачментреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponseMessage
api_type:
- schema
ms.assetid: 1edb085f-1674-48e5-8ec3-42351adeac7d
description: Элемент Делетеаттачментреспонсемессаже содержит состояние и результат одного запроса операции DeleteAttachment.
ms.openlocfilehash: 3ff253a5c2b6cbd69b7b976f7f41ca8b83814a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464261"
---
# <a name="deleteattachmentresponsemessage"></a><span data-ttu-id="f0c33-103">делетеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f0c33-103">DeleteAttachmentResponseMessage</span></span>

<span data-ttu-id="f0c33-104">Элемент **делетеаттачментреспонсемессаже** содержит состояние и результат одного запроса [операции DeleteAttachment](deleteattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0c33-104">The **DeleteAttachmentResponseMessage** element contains the status and result of a single [DeleteAttachment operation](deleteattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f0c33-105">делетеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="f0c33-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)  
- [<span data-ttu-id="f0c33-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f0c33-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="f0c33-107">делетеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f0c33-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
```xml
<DeleteAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootItemId/>
</DeleteAttachmentResponseMessage>
```

<span data-ttu-id="f0c33-108">**делетеаттачментреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f0c33-108">**DeleteAttachmentResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f0c33-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0c33-109">Attributes and elements</span></span>

<span data-ttu-id="f0c33-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f0c33-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0c33-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0c33-111">Attributes</span></span>

|<span data-ttu-id="f0c33-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f0c33-112">**Attribute**</span></span>|<span data-ttu-id="f0c33-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0c33-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0c33-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="f0c33-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f0c33-115">Описывает состояние ответа [операции DeleteAttachment](deleteattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0c33-115">Describes the status of a [DeleteAttachment operation](deleteattachment-operation.md) response.</span></span><br/><br/><span data-ttu-id="f0c33-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f0c33-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="f0c33-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="f0c33-117">-  Success</span></span>  <br/><span data-ttu-id="f0c33-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f0c33-118">-  Warning</span></span>  <br/><span data-ttu-id="f0c33-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="f0c33-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f0c33-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="f0c33-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f0c33-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f0c33-121">**Value**</span></span>|<span data-ttu-id="f0c33-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0c33-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0c33-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f0c33-123">**Success**</span></span> <br/> |<span data-ttu-id="f0c33-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="f0c33-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f0c33-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f0c33-125">**Warning**</span></span> <br/> | <span data-ttu-id="f0c33-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f0c33-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f0c33-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f0c33-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="f0c33-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="f0c33-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="f0c33-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="f0c33-129">- The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f0c33-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0c33-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f0c33-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="f0c33-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f0c33-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0c33-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f0c33-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="f0c33-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f0c33-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="f0c33-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="f0c33-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f0c33-135">**Error**</span></span> <br/> | <span data-ttu-id="f0c33-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f0c33-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="f0c33-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="f0c33-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="f0c33-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="f0c33-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f0c33-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="f0c33-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f0c33-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f0c33-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="f0c33-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="f0c33-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f0c33-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="f0c33-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f0c33-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="f0c33-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="f0c33-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f0c33-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0c33-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0c33-145">Child elements</span></span>

|<span data-ttu-id="f0c33-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0c33-146">**Element**</span></span>|<span data-ttu-id="f0c33-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0c33-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0c33-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f0c33-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f0c33-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="f0c33-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f0c33-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f0c33-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f0c33-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="f0c33-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f0c33-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="f0c33-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f0c33-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="f0c33-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f0c33-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f0c33-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f0c33-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="f0c33-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f0c33-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f0c33-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f0c33-157">рутитемид</span><span class="sxs-lookup"><span data-stu-id="f0c33-157">RootItemId</span></span>](rootitemid.md) <br/> |<span data-ttu-id="f0c33-158">Определяет родительский элемент удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="f0c33-158">Identifies the parent item of a deleted attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0c33-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0c33-159">Parent elements</span></span>

|<span data-ttu-id="f0c33-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0c33-160">**Element**</span></span>|<span data-ttu-id="f0c33-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0c33-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0c33-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f0c33-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f0c33-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0c33-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0c33-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="f0c33-164">Remarks</span></span>

<span data-ttu-id="f0c33-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f0c33-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0c33-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0c33-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0c33-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0c33-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0c33-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0c33-168">Schema Name</span></span>  <br/> |<span data-ttu-id="f0c33-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f0c33-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0c33-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0c33-170">Validation File</span></span>  <br/> |<span data-ttu-id="f0c33-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f0c33-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0c33-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0c33-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0c33-173">False</span><span class="sxs-lookup"><span data-stu-id="f0c33-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0c33-174">См. также</span><span class="sxs-lookup"><span data-stu-id="f0c33-174">See also</span></span>

- [<span data-ttu-id="f0c33-175">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="f0c33-175">DeleteAttachment</span></span>](deleteattachment.md) 
- [<span data-ttu-id="f0c33-176">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="f0c33-176">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="f0c33-177">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="f0c33-177">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="f0c33-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f0c33-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

