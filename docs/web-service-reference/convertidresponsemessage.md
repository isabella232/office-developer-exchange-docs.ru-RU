---
title: конвертидреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: Элемент Конвертидреспонсемессаже содержит состояние и результат запроса операции ConvertId.
ms.openlocfilehash: 6668c0b3254191ca628413bae5ff957c3cb95b5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761837"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="80237-103">конвертидреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="80237-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="80237-104">Элемент **конвертидреспонсемессаже** содержит состояние и результат запроса [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="80237-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="80237-105">конвертидреспонсе</span><span class="sxs-lookup"><span data-stu-id="80237-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="80237-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="80237-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="80237-107">конвертидреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="80237-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="80237-108">**конвертидреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="80237-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80237-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80237-109">Attributes and elements</span></span>

<span data-ttu-id="80237-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80237-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80237-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80237-111">Attributes</span></span>

|<span data-ttu-id="80237-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="80237-112">**Attribute**</span></span>|<span data-ttu-id="80237-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80237-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="80237-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="80237-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="80237-115">Описывает состояние ответа [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="80237-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="80237-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="80237-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="80237-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="80237-117">- Success</span></span>  <br/><span data-ttu-id="80237-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="80237-118">-  Warning</span></span>  <br/><span data-ttu-id="80237-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="80237-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="80237-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="80237-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="80237-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="80237-121">**Value**</span></span>|<span data-ttu-id="80237-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80237-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="80237-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="80237-123">**Success**</span></span> <br/> |<span data-ttu-id="80237-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="80237-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="80237-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="80237-125">**Warning**</span></span> <br/> | <span data-ttu-id="80237-126">Описывает запрос, который не был полностью обработан или для которого возникл нежелательный результат.</span><span class="sxs-lookup"><span data-stu-id="80237-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="80237-127">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="80237-127">**Error**</span></span> <br/> | <span data-ttu-id="80237-128">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="80237-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="80237-129">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="80237-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="80237-130">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="80237-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="80237-131">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="80237-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="80237-132">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="80237-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="80237-133">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="80237-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="80237-134">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="80237-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="80237-135">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="80237-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="80237-136">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="80237-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="80237-137">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80237-137">Child elements</span></span>

|<span data-ttu-id="80237-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80237-138">**Element**</span></span>|<span data-ttu-id="80237-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80237-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80237-140">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="80237-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="80237-141">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="80237-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="80237-142">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="80237-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="80237-143">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="80237-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="80237-144">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="80237-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="80237-145">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="80237-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="80237-146">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="80237-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="80237-147">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="80237-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="80237-148">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="80237-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="80237-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="80237-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="80237-150">Описывает преобразованный идентификатор в отклике.</span><span class="sxs-lookup"><span data-stu-id="80237-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80237-151">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80237-151">Parent elements</span></span>

|<span data-ttu-id="80237-152">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80237-152">**Element**</span></span>|<span data-ttu-id="80237-153">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80237-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80237-154">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="80237-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="80237-155">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="80237-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="80237-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="80237-156">Remarks</span></span>

<span data-ttu-id="80237-157">Возвращается одно ответное сообщение на один преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="80237-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="80237-158">Элемент [AlternateId](alternateid.md) будет отсутствовать в ответе, если возвращается код ответа об ошибке,</span><span class="sxs-lookup"><span data-stu-id="80237-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="80237-159">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Exchange 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="80237-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80237-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80237-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80237-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80237-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80237-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80237-162">Schema Name</span></span>  <br/> |<span data-ttu-id="80237-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="80237-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="80237-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80237-164">Validation File</span></span>  <br/> |<span data-ttu-id="80237-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="80237-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80237-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80237-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="80237-167">False</span><span class="sxs-lookup"><span data-stu-id="80237-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80237-168">См. также</span><span class="sxs-lookup"><span data-stu-id="80237-168">See also</span></span>

- [<span data-ttu-id="80237-169">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="80237-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="80237-170">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80237-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

