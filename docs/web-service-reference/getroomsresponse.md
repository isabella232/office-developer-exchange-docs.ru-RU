---
title: GetRoomsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomsResponse
api_type:
- schema
ms.assetid: a8c85f65-bb63-4e7a-b0ca-7c9a04560a58
description: Элемент GetRoomsResponse определяет ответ на запрос операции GetRooms.
ms.openlocfilehash: 7399ab910a99b39757eb752b11a4771ba81be46a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762907"
---
# <a name="getroomsresponse"></a><span data-ttu-id="f6e68-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="f6e68-103">GetRoomsResponse</span></span>

<span data-ttu-id="f6e68-104">Элемент **GetRoomsResponse** определяет ответ на запрос [GetRooms операции](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f6e68-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f6e68-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f6e68-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="f6e68-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="f6e68-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="f6e68-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f6e68-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6e68-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6e68-108">Attributes and elements</span></span>

<span data-ttu-id="f6e68-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f6e68-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6e68-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6e68-110">Attributes</span></span>

|<span data-ttu-id="f6e68-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f6e68-111">**Attribute**</span></span>|<span data-ttu-id="f6e68-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6e68-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6e68-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f6e68-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f6e68-114">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="f6e68-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f6e68-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f6e68-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f6e68-116">-Success</span><span class="sxs-lookup"><span data-stu-id="f6e68-116">-  Success</span></span>  <br/><span data-ttu-id="f6e68-117">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f6e68-117">-  Warning</span></span>  <br/><span data-ttu-id="f6e68-118">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="f6e68-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f6e68-119">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f6e68-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="f6e68-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f6e68-120">**Value**</span></span>|<span data-ttu-id="f6e68-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6e68-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6e68-122">**Успех**</span><span class="sxs-lookup"><span data-stu-id="f6e68-122">**Success**</span></span> <br/> |<span data-ttu-id="f6e68-123">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="f6e68-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f6e68-124">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="f6e68-124">**Warning**</span></span> <br/> | <span data-ttu-id="f6e68-125">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f6e68-125">Describes a request that was not processed.</span></span> <span data-ttu-id="f6e68-126">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="f6e68-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f6e68-127">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="f6e68-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="f6e68-128">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="f6e68-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f6e68-129">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6e68-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f6e68-130">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="f6e68-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f6e68-131">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6e68-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f6e68-132">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="f6e68-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="f6e68-133">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="f6e68-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f6e68-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="f6e68-134">**Error**</span></span> <br/> | <span data-ttu-id="f6e68-135">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f6e68-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f6e68-136">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="f6e68-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f6e68-137">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6e68-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f6e68-138">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="f6e68-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f6e68-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f6e68-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="f6e68-140">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="f6e68-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f6e68-141">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="f6e68-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f6e68-142">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="f6e68-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f6e68-143">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="f6e68-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f6e68-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6e68-144">Child elements</span></span>

|<span data-ttu-id="f6e68-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6e68-145">**Element**</span></span>|<span data-ttu-id="f6e68-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6e68-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6e68-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="f6e68-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f6e68-148">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="f6e68-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f6e68-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f6e68-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f6e68-150">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="f6e68-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f6e68-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f6e68-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f6e68-152">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f6e68-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f6e68-153">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f6e68-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f6e68-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f6e68-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f6e68-155">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="f6e68-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f6e68-156">Комнат</span><span class="sxs-lookup"><span data-stu-id="f6e68-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="f6e68-157">Предоставляет список адресов электронной почты и отображаемые имена, которые представляют комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="f6e68-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6e68-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6e68-158">Parent elements</span></span>

|<span data-ttu-id="f6e68-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6e68-159">**Element**</span></span>|<span data-ttu-id="f6e68-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6e68-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6e68-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f6e68-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f6e68-162">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6e68-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6e68-163">Замечания</span><span class="sxs-lookup"><span data-stu-id="f6e68-163">Remarks</span></span>

<span data-ttu-id="f6e68-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6e68-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6e68-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6e68-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6e68-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6e68-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6e68-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6e68-167">Schema Name</span></span>  <br/> |<span data-ttu-id="f6e68-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f6e68-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6e68-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6e68-169">Validation File</span></span>  <br/> |<span data-ttu-id="f6e68-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6e68-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6e68-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6e68-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6e68-172">False</span><span class="sxs-lookup"><span data-stu-id="f6e68-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6e68-173">См. также</span><span class="sxs-lookup"><span data-stu-id="f6e68-173">See also</span></span>

- [<span data-ttu-id="f6e68-174">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="f6e68-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="f6e68-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6e68-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

