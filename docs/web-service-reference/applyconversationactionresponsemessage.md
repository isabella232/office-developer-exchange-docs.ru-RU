---
title: аппликонверсатионактионреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: Элемент Аппликонверсатионактионреспонсемессаже содержит состояние и результаты запроса операции ApplyConversationAction.
ms.openlocfilehash: 377aee12d8cc7d6b4aff8d6fc2a6cb67b3bcd10b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464695"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="f1912-103">аппликонверсатионактионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f1912-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="f1912-104">Элемент **аппликонверсатионактионреспонсемессаже** содержит состояние и результаты запроса [операции ApplyConversationAction](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f1912-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="f1912-105">аппликонверсатионактионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f1912-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="f1912-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f1912-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="f1912-107">аппликонверсатионактионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f1912-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="f1912-108">**аппликонверсатионактионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f1912-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1912-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1912-109">Attributes and elements</span></span>

<span data-ttu-id="f1912-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f1912-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1912-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1912-111">Attributes</span></span>

|<span data-ttu-id="f1912-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f1912-112">**Attribute**</span></span>|<span data-ttu-id="f1912-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1912-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1912-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="f1912-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f1912-115">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="f1912-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="f1912-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f1912-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="f1912-117">Успешно</span><span class="sxs-lookup"><span data-stu-id="f1912-117">Success</span></span></li><li><span data-ttu-id="f1912-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f1912-118">Warning</span></span></li><li><span data-ttu-id="f1912-119">Ошибка</span><span class="sxs-lookup"><span data-stu-id="f1912-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f1912-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="f1912-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f1912-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f1912-121">**Value**</span></span>|<span data-ttu-id="f1912-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1912-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1912-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f1912-123">**Success**</span></span> <br/> |<span data-ttu-id="f1912-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="f1912-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f1912-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f1912-125">**Warning**</span></span> <br/> | <span data-ttu-id="f1912-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f1912-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f1912-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f1912-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="f1912-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="f1912-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="f1912-129">Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="f1912-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="f1912-130">Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f1912-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="f1912-131">Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="f1912-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="f1912-132">База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f1912-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="f1912-133">Истек срок действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f1912-133">A password is expired.</span></span></li><li><span data-ttu-id="f1912-134">Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="f1912-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="f1912-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f1912-135">**Error**</span></span> <br/> | <span data-ttu-id="f1912-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f1912-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="f1912-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="f1912-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="f1912-138">Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="f1912-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="f1912-139">Атрибуты или элементы, которые выходят за пределы диапазона</span><span class="sxs-lookup"><span data-stu-id="f1912-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="f1912-140">Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f1912-140">An unknown tag</span></span>  </li><li><span data-ttu-id="f1912-141">Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="f1912-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="f1912-142">Попытки несанкционированного доступа, выполняемые любым клиентом</span><span class="sxs-lookup"><span data-stu-id="f1912-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="f1912-143">Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="f1912-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="f1912-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f1912-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f1912-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1912-145">Child elements</span></span>

|<span data-ttu-id="f1912-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1912-146">**Element**</span></span>|<span data-ttu-id="f1912-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1912-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1912-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f1912-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f1912-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="f1912-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f1912-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f1912-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f1912-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="f1912-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f1912-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="f1912-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f1912-153">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f1912-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f1912-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f1912-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f1912-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="f1912-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f1912-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f1912-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1912-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1912-157">Parent elements</span></span>

|<span data-ttu-id="f1912-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1912-158">**Element**</span></span>|<span data-ttu-id="f1912-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1912-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1912-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f1912-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f1912-161">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1912-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1912-162">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f1912-162">Text value</span></span>

<span data-ttu-id="f1912-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1912-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1912-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="f1912-164">Remarks</span></span>

<span data-ttu-id="f1912-165">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f1912-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f1912-166">Различия версий</span><span class="sxs-lookup"><span data-stu-id="f1912-166">Version differences</span></span>

<span data-ttu-id="f1912-167">В версиях Exchange, начиная с сборки 15.00.0986.00, элемент **аппликонверсатионактионреспонсемессаже** имеет тип **аппликонверсатионактионреспонсемессажетипе**.</span><span class="sxs-lookup"><span data-stu-id="f1912-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="f1912-168">В предыдущих версиях элемент относится к типу **респонсемессажетипе**.</span><span class="sxs-lookup"><span data-stu-id="f1912-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1912-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1912-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1912-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1912-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1912-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1912-171">Schema Name</span></span>  <br/> |<span data-ttu-id="f1912-172">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="f1912-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="f1912-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1912-173">Validation File</span></span>  <br/> |<span data-ttu-id="f1912-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1912-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1912-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1912-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1912-176">False</span><span class="sxs-lookup"><span data-stu-id="f1912-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1912-177">См. также</span><span class="sxs-lookup"><span data-stu-id="f1912-177">See also</span></span>

- [<span data-ttu-id="f1912-178">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f1912-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f1912-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1912-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

