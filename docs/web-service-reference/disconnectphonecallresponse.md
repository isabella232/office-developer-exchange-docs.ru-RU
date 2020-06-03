---
title: дисконнектфонекаллреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCallResponse
api_type:
- schema
ms.assetid: 05041799-5b81-4b87-ada8-ce6c506ffe01
description: Элемент Дисконнектфонекаллреспонсе содержит состояние и результат одного запроса DisconnectPhoneCall.
ms.openlocfilehash: 6c0696a1d9ab3242920d051b409105644a6b03aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458448"
---
# <a name="disconnectphonecallresponse"></a><span data-ttu-id="37ecc-103">дисконнектфонекаллреспонсе</span><span class="sxs-lookup"><span data-stu-id="37ecc-103">DisconnectPhoneCallResponse</span></span>

<span data-ttu-id="37ecc-104">Элемент **дисконнектфонекаллреспонсе** содержит состояние и результат одного запроса **DisconnectPhoneCall** .</span><span class="sxs-lookup"><span data-stu-id="37ecc-104">The **DisconnectPhoneCallResponse** element contains the status and result of a single **DisconnectPhoneCall** request.</span></span> 
  
```xml
<DisconnectPhoneCallResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DisconnectPhoneCallResponse>
```

 <span data-ttu-id="37ecc-105">**дисконнектфонекаллреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="37ecc-105">**DisconnectPhoneCallResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37ecc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="37ecc-106">Attributes and elements</span></span>

<span data-ttu-id="37ecc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="37ecc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37ecc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="37ecc-108">Attributes</span></span>

|<span data-ttu-id="37ecc-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="37ecc-109">**Attribute**</span></span>|<span data-ttu-id="37ecc-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37ecc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="37ecc-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="37ecc-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="37ecc-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="37ecc-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="37ecc-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="37ecc-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="37ecc-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="37ecc-114">-  Success</span></span>  <br/><span data-ttu-id="37ecc-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="37ecc-115">-  Warning</span></span>  <br/><span data-ttu-id="37ecc-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="37ecc-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="37ecc-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="37ecc-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="37ecc-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="37ecc-118">**Value**</span></span>|<span data-ttu-id="37ecc-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37ecc-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="37ecc-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="37ecc-120">**Success**</span></span> <br/> |<span data-ttu-id="37ecc-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="37ecc-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="37ecc-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="37ecc-122">**Warning**</span></span> <br/> | <span data-ttu-id="37ecc-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="37ecc-123">Describes a request that was not processed.</span></span> <span data-ttu-id="37ecc-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="37ecc-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="37ecc-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="37ecc-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="37ecc-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="37ecc-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="37ecc-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="37ecc-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="37ecc-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="37ecc-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="37ecc-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="37ecc-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="37ecc-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="37ecc-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="37ecc-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="37ecc-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="37ecc-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="37ecc-132">**Error**</span></span> <br/> | <span data-ttu-id="37ecc-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="37ecc-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="37ecc-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="37ecc-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="37ecc-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="37ecc-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="37ecc-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="37ecc-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="37ecc-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="37ecc-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="37ecc-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="37ecc-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="37ecc-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="37ecc-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="37ecc-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="37ecc-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="37ecc-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="37ecc-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="37ecc-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="37ecc-142">Child elements</span></span>

|<span data-ttu-id="37ecc-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="37ecc-143">**Element**</span></span>|<span data-ttu-id="37ecc-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37ecc-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37ecc-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="37ecc-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="37ecc-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="37ecc-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="37ecc-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="37ecc-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="37ecc-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="37ecc-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="37ecc-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="37ecc-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="37ecc-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="37ecc-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="37ecc-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="37ecc-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="37ecc-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="37ecc-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="37ecc-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="37ecc-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37ecc-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="37ecc-154">Parent elements</span></span>

<span data-ttu-id="37ecc-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="37ecc-155">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="37ecc-156">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="37ecc-156">Text value</span></span>

<span data-ttu-id="37ecc-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="37ecc-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37ecc-158">Примечания</span><span class="sxs-lookup"><span data-stu-id="37ecc-158">Remarks</span></span>

<span data-ttu-id="37ecc-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="37ecc-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37ecc-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="37ecc-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37ecc-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="37ecc-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="37ecc-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="37ecc-162">Schema Name</span></span>  <br/> |<span data-ttu-id="37ecc-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="37ecc-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="37ecc-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="37ecc-164">Validation File</span></span>  <br/> |<span data-ttu-id="37ecc-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="37ecc-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37ecc-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="37ecc-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="37ecc-167">False</span><span class="sxs-lookup"><span data-stu-id="37ecc-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37ecc-168">См. также</span><span class="sxs-lookup"><span data-stu-id="37ecc-168">See also</span></span>

- [<span data-ttu-id="37ecc-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37ecc-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

