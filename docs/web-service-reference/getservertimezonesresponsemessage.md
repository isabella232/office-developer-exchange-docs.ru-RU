---
title: жетсервертимезонесреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponseMessage
api_type:
- schema
ms.assetid: eb2592b2-144f-4c33-8df7-8e70dce7ab55
description: Элемент Жетсервертимезонесреспонсемессаже содержит состояние и результат одного запроса операции GetServerTimeZones.
ms.openlocfilehash: 594b194f7c73e8880b83db6e20bb447e682a525c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833665"
---
# <a name="getservertimezonesresponsemessage"></a><span data-ttu-id="4935d-103">жетсервертимезонесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4935d-103">GetServerTimeZonesResponseMessage</span></span>

<span data-ttu-id="4935d-104">Элемент **жетсервертимезонесреспонсемессаже** содержит состояние и результат одного запроса [операции GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4935d-104">The **GetServerTimeZonesResponseMessage** element contains the status and result of a single [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <TimeZoneDefinitions/>
</GetServerTimeZonesResponseMessage>
```

 <span data-ttu-id="4935d-105">**жетсервертимезонесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4935d-105">**GetServerTimeZonesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4935d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4935d-106">Attributes and elements</span></span>

<span data-ttu-id="4935d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4935d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4935d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4935d-108">Attributes</span></span>

|<span data-ttu-id="4935d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4935d-109">**Attribute**</span></span>|<span data-ttu-id="4935d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4935d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4935d-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="4935d-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4935d-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="4935d-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="4935d-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4935d-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4935d-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="4935d-114">-  Success</span></span>  <br/><span data-ttu-id="4935d-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4935d-115">-  Warning</span></span>  <br/><span data-ttu-id="4935d-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="4935d-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4935d-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4935d-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="4935d-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4935d-118">**Value**</span></span>|<span data-ttu-id="4935d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4935d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4935d-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="4935d-120">**Success**</span></span> <br/> |<span data-ttu-id="4935d-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="4935d-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4935d-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4935d-122">**Warning**</span></span> <br/> | <span data-ttu-id="4935d-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4935d-123">Describes a request that was not processed.</span></span> <span data-ttu-id="4935d-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="4935d-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="4935d-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4935d-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="4935d-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="4935d-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4935d-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4935d-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4935d-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="4935d-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="4935d-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4935d-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4935d-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="4935d-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="4935d-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="4935d-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="4935d-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="4935d-132">**Error**</span></span> <br/> | <span data-ttu-id="4935d-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4935d-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4935d-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="4935d-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4935d-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="4935d-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4935d-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="4935d-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4935d-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4935d-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="4935d-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="4935d-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4935d-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="4935d-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4935d-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="4935d-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4935d-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4935d-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4935d-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4935d-142">Child elements</span></span>

|<span data-ttu-id="4935d-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4935d-143">**Element**</span></span>|<span data-ttu-id="4935d-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4935d-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4935d-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4935d-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4935d-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4935d-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4935d-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4935d-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4935d-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="4935d-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4935d-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4935d-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4935d-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="4935d-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="4935d-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4935d-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4935d-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4935d-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4935d-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4935d-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4935d-154">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="4935d-154">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="4935d-155">Содержит массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="4935d-155">Contains an array of time zone definitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4935d-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4935d-156">Parent elements</span></span>

|<span data-ttu-id="4935d-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4935d-157">**Element**</span></span>|<span data-ttu-id="4935d-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4935d-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4935d-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4935d-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4935d-160">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="4935d-160">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4935d-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="4935d-161">Remarks</span></span>

<span data-ttu-id="4935d-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4935d-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4935d-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4935d-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4935d-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4935d-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4935d-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4935d-165">Schema Name</span></span>  <br/> |<span data-ttu-id="4935d-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4935d-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4935d-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4935d-167">Validation File</span></span>  <br/> |<span data-ttu-id="4935d-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4935d-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4935d-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4935d-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="4935d-170">False</span><span class="sxs-lookup"><span data-stu-id="4935d-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4935d-171">См. также</span><span class="sxs-lookup"><span data-stu-id="4935d-171">See also</span></span>

- [<span data-ttu-id="4935d-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4935d-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

