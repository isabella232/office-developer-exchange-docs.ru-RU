---
title: GetRoomListsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomListsResponse
api_type:
- schema
ms.assetid: 8c736f68-1026-496a-b12f-c169c078abd0
description: Элемент GetRoomListsResponse определяет ответа от GetRoomLists операции.
ms.openlocfilehash: 8231435f7dc348a070852f57d6152550326b5df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762913"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="f6694-103">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="f6694-103">GetRoomListsResponse</span></span>

<span data-ttu-id="f6694-104">Элемент **GetRoomListsResponse** определяет ответа от [GetRoomLists операции](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f6694-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f6694-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f6694-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="f6694-106">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="f6694-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="f6694-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f6694-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6694-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6694-108">Attributes and elements</span></span>

<span data-ttu-id="f6694-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f6694-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6694-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6694-110">Attributes</span></span>

|<span data-ttu-id="f6694-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f6694-111">**Attribute**</span></span>|<span data-ttu-id="f6694-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6694-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6694-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f6694-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f6694-114">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="f6694-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f6694-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f6694-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f6694-116">-Success</span><span class="sxs-lookup"><span data-stu-id="f6694-116">-  Success</span></span>  <br/><span data-ttu-id="f6694-117">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f6694-117">-  Warning</span></span>  <br/><span data-ttu-id="f6694-118">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="f6694-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f6694-119">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f6694-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="f6694-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f6694-120">**Value**</span></span>|<span data-ttu-id="f6694-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6694-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6694-122">**Успех**</span><span class="sxs-lookup"><span data-stu-id="f6694-122">**Success**</span></span> <br/> |<span data-ttu-id="f6694-123">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="f6694-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f6694-124">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="f6694-124">**Warning**</span></span> <br/> | <span data-ttu-id="f6694-125">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f6694-125">Describes a request that was not processed.</span></span> <span data-ttu-id="f6694-126">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="f6694-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f6694-127">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="f6694-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f6694-128">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="f6694-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f6694-129">-К службе каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6694-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="f6694-130">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="f6694-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f6694-131">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6694-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f6694-132">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="f6694-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="f6694-133">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="f6694-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f6694-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="f6694-134">**Error**</span></span> <br/> | <span data-ttu-id="f6694-135">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f6694-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f6694-136">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="f6694-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f6694-137">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6694-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f6694-138">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="f6694-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f6694-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f6694-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="f6694-140">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="f6694-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f6694-141">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="f6694-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f6694-142">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="f6694-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f6694-143">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="f6694-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="f6694-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6694-144">Child elements</span></span>

|<span data-ttu-id="f6694-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6694-145">**Element**</span></span>|<span data-ttu-id="f6694-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6694-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6694-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="f6694-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f6694-148">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="f6694-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f6694-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f6694-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f6694-150">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="f6694-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f6694-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f6694-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f6694-152">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f6694-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f6694-153">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f6694-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f6694-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f6694-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f6694-155">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="f6694-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f6694-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="f6694-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="f6694-157">Предоставляет список адресов электронной почты и отображаемые имена, которые представляют списки конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="f6694-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6694-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6694-158">Parent elements</span></span>

|<span data-ttu-id="f6694-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6694-159">**Element**</span></span>|<span data-ttu-id="f6694-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6694-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6694-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f6694-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f6694-162">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6694-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="f6694-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6694-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6694-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6694-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6694-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6694-165">Schema Name</span></span>  <br/> |<span data-ttu-id="f6694-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f6694-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6694-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6694-167">Validation File</span></span>  <br/> |<span data-ttu-id="f6694-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f6694-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6694-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6694-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6694-170">False</span><span class="sxs-lookup"><span data-stu-id="f6694-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6694-171">См. также</span><span class="sxs-lookup"><span data-stu-id="f6694-171">See also</span></span>

- [<span data-ttu-id="f6694-172">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="f6694-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="f6694-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6694-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

