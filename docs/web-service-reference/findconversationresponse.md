---
title: финдконверсатионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversationResponse
api_type:
- schema
ms.assetid: a689e29d-5f3d-4deb-81ee-8b6cc60f6dea
description: Элемент Финдконверсатионреспонсе определяет ответ на запрос операции FindConversation.
ms.openlocfilehash: 5754ea7540fa6daac8cd725386ca213d5bf05c8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762557"
---
# <a name="findconversationresponse"></a><span data-ttu-id="ee362-103">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="ee362-103">FindConversationResponse</span></span>

<span data-ttu-id="ee362-104">Элемент **финдконверсатионреспонсе** определяет ответ на запрос [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ee362-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="ee362-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="ee362-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="ee362-106">**финдконверсатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="ee362-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee362-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ee362-107">Attributes and elements</span></span>

<span data-ttu-id="ee362-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ee362-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee362-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ee362-109">Attributes</span></span>

|<span data-ttu-id="ee362-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ee362-110">**Attribute**</span></span>|<span data-ttu-id="ee362-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee362-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee362-112">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="ee362-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ee362-113">Описывает состояние ответа [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ee362-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="ee362-114">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ee362-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="ee362-115">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="ee362-115">-  Success</span></span>  <br/><span data-ttu-id="ee362-116">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="ee362-116">-  Warning</span></span>  <br/><span data-ttu-id="ee362-117">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="ee362-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ee362-118">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="ee362-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="ee362-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ee362-119">**Value**</span></span>|<span data-ttu-id="ee362-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee362-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee362-121">**Success**</span><span class="sxs-lookup"><span data-stu-id="ee362-121">**Success**</span></span> <br/> |<span data-ttu-id="ee362-122">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="ee362-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ee362-123">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ee362-123">**Warning**</span></span> <br/> | <span data-ttu-id="ee362-124">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="ee362-124">Describes a request that was not processed.</span></span> <span data-ttu-id="ee362-125">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="ee362-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="ee362-126">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="ee362-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ee362-127">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="ee362-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ee362-128">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ee362-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ee362-129">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="ee362-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ee362-130">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ee362-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ee362-131">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="ee362-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="ee362-132">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="ee362-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="ee362-133">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="ee362-133">**Error**</span></span> <br/> | <span data-ttu-id="ee362-134">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="ee362-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ee362-135">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="ee362-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ee362-136">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="ee362-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ee362-137">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="ee362-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="ee362-138">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="ee362-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="ee362-139">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="ee362-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ee362-140">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="ee362-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ee362-141">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="ee362-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ee362-142">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ee362-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ee362-143">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ee362-143">Child elements</span></span>

|<span data-ttu-id="ee362-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee362-144">**Element**</span></span>|<span data-ttu-id="ee362-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee362-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee362-146">Беседы</span><span class="sxs-lookup"><span data-stu-id="ee362-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ee362-147">Содержит массив бесед.</span><span class="sxs-lookup"><span data-stu-id="ee362-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="ee362-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ee362-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ee362-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="ee362-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ee362-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ee362-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ee362-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="ee362-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ee362-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ee362-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ee362-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="ee362-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ee362-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="ee362-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ee362-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="ee362-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ee362-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ee362-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee362-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ee362-157">Parent elements</span></span>

<span data-ttu-id="ee362-158">Нет.</span><span class="sxs-lookup"><span data-stu-id="ee362-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ee362-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ee362-159">Text value</span></span>

<span data-ttu-id="ee362-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="ee362-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ee362-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="ee362-161">Remarks</span></span>

<span data-ttu-id="ee362-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ee362-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee362-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ee362-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee362-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ee362-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee362-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ee362-165">Schema name</span></span>  <br/> |<span data-ttu-id="ee362-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ee362-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee362-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ee362-167">Validation file</span></span>  <br/> |<span data-ttu-id="ee362-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ee362-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee362-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ee362-169">Can be empty</span></span>  <br/> |<span data-ttu-id="ee362-170">False</span><span class="sxs-lookup"><span data-stu-id="ee362-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee362-171">См. также</span><span class="sxs-lookup"><span data-stu-id="ee362-171">See also</span></span>

- [<span data-ttu-id="ee362-172">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="ee362-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="ee362-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee362-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ee362-174">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="ee362-174">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

