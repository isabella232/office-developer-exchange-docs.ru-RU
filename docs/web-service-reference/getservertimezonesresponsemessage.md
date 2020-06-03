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
ms.openlocfilehash: de032c961f6fffa5b4f0607a17fe48630510fda9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460920"
---
# <a name="getservertimezonesresponsemessage"></a><span data-ttu-id="f6cda-103">жетсервертимезонесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f6cda-103">GetServerTimeZonesResponseMessage</span></span>

<span data-ttu-id="f6cda-104">Элемент **жетсервертимезонесреспонсемессаже** содержит состояние и результат одного запроса [операции GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f6cda-104">The **GetServerTimeZonesResponseMessage** element contains the status and result of a single [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <TimeZoneDefinitions/>
</GetServerTimeZonesResponseMessage>
```

 <span data-ttu-id="f6cda-105">**жетсервертимезонесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f6cda-105">**GetServerTimeZonesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6cda-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6cda-106">Attributes and elements</span></span>

<span data-ttu-id="f6cda-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f6cda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6cda-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6cda-108">Attributes</span></span>

|<span data-ttu-id="f6cda-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f6cda-109">**Attribute**</span></span>|<span data-ttu-id="f6cda-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6cda-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cda-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="f6cda-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f6cda-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="f6cda-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f6cda-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f6cda-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f6cda-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="f6cda-114">-  Success</span></span>  <br/><span data-ttu-id="f6cda-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f6cda-115">-  Warning</span></span>  <br/><span data-ttu-id="f6cda-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="f6cda-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f6cda-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="f6cda-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f6cda-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f6cda-118">**Value**</span></span>|<span data-ttu-id="f6cda-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6cda-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cda-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f6cda-120">**Success**</span></span> <br/> |<span data-ttu-id="f6cda-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="f6cda-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f6cda-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f6cda-122">**Warning**</span></span> <br/> | <span data-ttu-id="f6cda-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f6cda-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f6cda-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f6cda-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="f6cda-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="f6cda-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="f6cda-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="f6cda-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f6cda-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6cda-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f6cda-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="f6cda-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f6cda-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6cda-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f6cda-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="f6cda-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f6cda-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="f6cda-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f6cda-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f6cda-132">**Error**</span></span> <br/> | <span data-ttu-id="f6cda-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f6cda-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f6cda-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="f6cda-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f6cda-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="f6cda-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f6cda-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="f6cda-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f6cda-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f6cda-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="f6cda-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="f6cda-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f6cda-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="f6cda-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f6cda-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="f6cda-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f6cda-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f6cda-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f6cda-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6cda-142">Child elements</span></span>

|<span data-ttu-id="f6cda-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6cda-143">**Element**</span></span>|<span data-ttu-id="f6cda-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6cda-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6cda-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f6cda-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f6cda-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="f6cda-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f6cda-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f6cda-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f6cda-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="f6cda-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f6cda-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="f6cda-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f6cda-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f6cda-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f6cda-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f6cda-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f6cda-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="f6cda-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f6cda-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f6cda-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f6cda-154">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="f6cda-154">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="f6cda-155">Содержит массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="f6cda-155">Contains an array of time zone definitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6cda-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6cda-156">Parent elements</span></span>

|<span data-ttu-id="f6cda-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6cda-157">**Element**</span></span>|<span data-ttu-id="f6cda-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6cda-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6cda-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f6cda-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f6cda-160">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="f6cda-160">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6cda-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="f6cda-161">Remarks</span></span>

<span data-ttu-id="f6cda-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6cda-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6cda-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6cda-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6cda-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6cda-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6cda-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6cda-165">Schema Name</span></span>  <br/> |<span data-ttu-id="f6cda-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f6cda-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6cda-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6cda-167">Validation File</span></span>  <br/> |<span data-ttu-id="f6cda-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f6cda-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6cda-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6cda-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6cda-170">False</span><span class="sxs-lookup"><span data-stu-id="f6cda-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6cda-171">См. также</span><span class="sxs-lookup"><span data-stu-id="f6cda-171">See also</span></span>

- [<span data-ttu-id="f6cda-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6cda-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

