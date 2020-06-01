---
title: жетаттачментреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponseMessage
api_type:
- schema
ms.assetid: f0a841af-422d-4c82-b710-41e2038dbee4
description: Элемент Жетаттачментреспонсемессаже содержит состояние и результат одного запроса операции GetAttachment.
ms.openlocfilehash: cfe36364431a8fe81c3f62e68356b634f00bee78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457797"
---
# <a name="getattachmentresponsemessage"></a><span data-ttu-id="6ff8f-103">жетаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6ff8f-103">GetAttachmentResponseMessage</span></span>

<span data-ttu-id="6ff8f-104">Элемент **жетаттачментреспонсемессаже** содержит состояние и результат одного запроса [операции GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff8f-104">The **GetAttachmentResponseMessage** element contains the status and result of a single [GetAttachment operation](getattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="6ff8f-105">жетаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="6ff8f-105">GetAttachmentResponse</span></span>](getattachmentresponse.md) 
- [<span data-ttu-id="6ff8f-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6ff8f-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="6ff8f-107">жетаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6ff8f-107">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
  
```xml
<GetAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</GetAttachmentResponseMessage>
```

 <span data-ttu-id="6ff8f-108">**аттачментинфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-108">**AttachmentInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ff8f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6ff8f-109">Attributes and elements</span></span>

<span data-ttu-id="6ff8f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ff8f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6ff8f-111">Attributes</span></span>

|<span data-ttu-id="6ff8f-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-112">**Attribute**</span></span>|<span data-ttu-id="6ff8f-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ff8f-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6ff8f-115">Описывает состояние ответа [операции GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff8f-115">Describes the status of a [GetAttachment operation](getattachment-operation.md) response.</span></span><br/><br/> <span data-ttu-id="6ff8f-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="6ff8f-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="6ff8f-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="6ff8f-117">-  Success</span></span>  <br/><span data-ttu-id="6ff8f-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="6ff8f-118">-  Warning</span></span>  <br/><span data-ttu-id="6ff8f-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="6ff8f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="6ff8f-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="6ff8f-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="6ff8f-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-121">**Value**</span></span>|<span data-ttu-id="6ff8f-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ff8f-123">Успешно</span><span class="sxs-lookup"><span data-stu-id="6ff8f-123">Success</span></span>  <br/> |<span data-ttu-id="6ff8f-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6ff8f-125">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="6ff8f-125">Warning</span></span>  <br/> | <span data-ttu-id="6ff8f-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-126">Describes a request that was not processed.</span></span> <span data-ttu-id="6ff8f-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="6ff8f-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="6ff8f-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6ff8f-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6ff8f-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="6ff8f-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6ff8f-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="6ff8f-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="6ff8f-135">Ошибка</span><span class="sxs-lookup"><span data-stu-id="6ff8f-135">Error</span></span>  <br/> | <span data-ttu-id="6ff8f-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6ff8f-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="6ff8f-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="6ff8f-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6ff8f-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="6ff8f-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6ff8f-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="6ff8f-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="6ff8f-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="6ff8f-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6ff8f-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="6ff8f-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6ff8f-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="6ff8f-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="6ff8f-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff8f-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6ff8f-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6ff8f-145">Child elements</span></span>

|<span data-ttu-id="6ff8f-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-146">**Element**</span></span>|<span data-ttu-id="6ff8f-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ff8f-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6ff8f-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6ff8f-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6ff8f-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6ff8f-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6ff8f-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6ff8f-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6ff8f-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6ff8f-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6ff8f-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6ff8f-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="6ff8f-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6ff8f-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6ff8f-157">Вложения</span><span class="sxs-lookup"><span data-stu-id="6ff8f-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6ff8f-158">Содержит элементы или файлы, которые ттачед с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-158">Contains the items or files that are ttached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ff8f-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6ff8f-159">Parent elements</span></span>

|<span data-ttu-id="6ff8f-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-160">**Element**</span></span>|<span data-ttu-id="6ff8f-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ff8f-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ff8f-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6ff8f-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6ff8f-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6ff8f-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="6ff8f-164">Remarks</span></span>

<span data-ttu-id="6ff8f-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6ff8f-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ff8f-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6ff8f-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ff8f-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6ff8f-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ff8f-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6ff8f-168">Schema Name</span></span>  <br/> |<span data-ttu-id="6ff8f-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6ff8f-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ff8f-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6ff8f-170">Validation File</span></span>  <br/> |<span data-ttu-id="6ff8f-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6ff8f-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ff8f-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6ff8f-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ff8f-173">False</span><span class="sxs-lookup"><span data-stu-id="6ff8f-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ff8f-174">См. также</span><span class="sxs-lookup"><span data-stu-id="6ff8f-174">See also</span></span>

- [<span data-ttu-id="6ff8f-175">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="6ff8f-175">GetAttachment</span></span>](getattachment.md) 
- [<span data-ttu-id="6ff8f-176">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="6ff8f-176">GetAttachment operation</span></span>](getattachment-operation.md)

