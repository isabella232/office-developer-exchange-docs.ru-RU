---
title: жетсервицеконфигуратионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfigurationResponse
api_type:
- schema
ms.assetid: 313dac99-0e5c-4198-bafa-89e749934ac7
description: Элемент Жетсервицеконфигуратионреспонсе определяет ответ на запрос GetServiceConfiguration.
ms.openlocfilehash: 7abc81222125334de2a6ab6e4a618b48fe0caf4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833668"
---
# <a name="getserviceconfigurationresponse"></a><span data-ttu-id="d4fce-103">жетсервицеконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="d4fce-103">GetServiceConfigurationResponse</span></span>

<span data-ttu-id="d4fce-104">Элемент **жетсервицеконфигуратионреспонсе** определяет ответ на запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d4fce-104">The **GetServiceConfigurationResponse** element defines a response to a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfigurationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResponseMessages/>
</GetServiceConfigurationResponse>
```

 <span data-ttu-id="d4fce-105">**жетсервицеконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="d4fce-105">**GetServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4fce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d4fce-106">Attributes and elements</span></span>

<span data-ttu-id="d4fce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d4fce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4fce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d4fce-108">Attributes</span></span>

|<span data-ttu-id="d4fce-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d4fce-109">**Attribute**</span></span>|<span data-ttu-id="d4fce-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4fce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4fce-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="d4fce-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d4fce-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="d4fce-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d4fce-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d4fce-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d4fce-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="d4fce-114">-  Success</span></span>  <br/><span data-ttu-id="d4fce-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d4fce-115">-  Warning</span></span>  <br/><span data-ttu-id="d4fce-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="d4fce-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d4fce-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="d4fce-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d4fce-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d4fce-118">**Value**</span></span>|<span data-ttu-id="d4fce-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4fce-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4fce-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="d4fce-120">**Success**</span></span> <br/> |<span data-ttu-id="d4fce-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="d4fce-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d4fce-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d4fce-122">**Warning**</span></span> <br/> | <span data-ttu-id="d4fce-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d4fce-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d4fce-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="d4fce-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d4fce-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="d4fce-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d4fce-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="d4fce-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d4fce-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d4fce-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d4fce-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="d4fce-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d4fce-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d4fce-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d4fce-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="d4fce-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d4fce-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="d4fce-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d4fce-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="d4fce-132">**Error**</span></span> <br/> | <span data-ttu-id="d4fce-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d4fce-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d4fce-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="d4fce-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d4fce-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="d4fce-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d4fce-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="d4fce-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d4fce-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d4fce-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d4fce-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d4fce-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d4fce-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="d4fce-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d4fce-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="d4fce-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d4fce-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d4fce-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4fce-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d4fce-142">Child elements</span></span>

|<span data-ttu-id="d4fce-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4fce-143">**Element**</span></span>|<span data-ttu-id="d4fce-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4fce-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fce-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="d4fce-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d4fce-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="d4fce-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d4fce-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d4fce-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d4fce-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="d4fce-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d4fce-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="d4fce-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d4fce-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d4fce-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d4fce-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d4fce-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d4fce-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="d4fce-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d4fce-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d4fce-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d4fce-154">Респонсемессажес (Аррайофсервицеконфигуратионреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="d4fce-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="d4fce-155">Содержит массив ответных сообщений конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="d4fce-155">Contains an array of service configuration response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4fce-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d4fce-156">Parent elements</span></span>

<span data-ttu-id="d4fce-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4fce-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d4fce-158">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d4fce-158">Text value</span></span>

<span data-ttu-id="d4fce-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4fce-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4fce-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="d4fce-160">Remarks</span></span>

<span data-ttu-id="d4fce-161">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4fce-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4fce-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d4fce-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4fce-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d4fce-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4fce-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d4fce-164">Schema Name</span></span>  <br/> |<span data-ttu-id="d4fce-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d4fce-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4fce-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d4fce-166">Validation File</span></span>  <br/> |<span data-ttu-id="d4fce-167">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d4fce-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4fce-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d4fce-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4fce-169">False</span><span class="sxs-lookup"><span data-stu-id="d4fce-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4fce-170">См. также</span><span class="sxs-lookup"><span data-stu-id="d4fce-170">See also</span></span>

- [<span data-ttu-id="d4fce-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d4fce-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

