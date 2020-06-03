---
title: жетрумлистсреспонсе
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
description: Элемент Жетрумлистсреспонсе определяет ответ на запрос операции GetRoomLists.
ms.openlocfilehash: b6d7c2baa2861309d72bcbf880eaed2ad0989175
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462945"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="d6408-103">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d6408-103">GetRoomListsResponse</span></span>

<span data-ttu-id="d6408-104">Элемент **жетрумлистсреспонсе** определяет ответ на запрос [операции GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d6408-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d6408-105">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="d6408-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d6408-106">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d6408-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="d6408-107">**жетрумлистсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="d6408-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6408-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d6408-108">Attributes and elements</span></span>

<span data-ttu-id="d6408-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d6408-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6408-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d6408-110">Attributes</span></span>

|<span data-ttu-id="d6408-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d6408-111">**Attribute**</span></span>|<span data-ttu-id="d6408-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6408-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6408-113">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="d6408-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d6408-114">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="d6408-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d6408-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d6408-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d6408-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="d6408-116">-  Success</span></span>  <br/><span data-ttu-id="d6408-117">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d6408-117">-  Warning</span></span>  <br/><span data-ttu-id="d6408-118">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="d6408-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d6408-119">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="d6408-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="d6408-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d6408-120">**Value**</span></span>|<span data-ttu-id="d6408-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6408-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6408-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="d6408-122">**Success**</span></span> <br/> |<span data-ttu-id="d6408-123">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="d6408-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d6408-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d6408-124">**Warning**</span></span> <br/> | <span data-ttu-id="d6408-125">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d6408-125">Describes a request that was not processed.</span></span> <span data-ttu-id="d6408-126">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="d6408-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d6408-127">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="d6408-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d6408-128">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="d6408-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d6408-129">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d6408-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="d6408-130">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="d6408-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d6408-131">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d6408-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d6408-132">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="d6408-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="d6408-133">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="d6408-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d6408-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="d6408-134">**Error**</span></span> <br/> | <span data-ttu-id="d6408-135">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d6408-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d6408-136">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="d6408-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d6408-137">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="d6408-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d6408-138">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="d6408-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d6408-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d6408-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="d6408-140">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d6408-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d6408-141">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="d6408-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d6408-142">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="d6408-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d6408-143">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d6408-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="d6408-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d6408-144">Child elements</span></span>

|<span data-ttu-id="d6408-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6408-145">**Element**</span></span>|<span data-ttu-id="d6408-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6408-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6408-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="d6408-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d6408-148">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="d6408-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d6408-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d6408-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d6408-150">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="d6408-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d6408-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="d6408-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d6408-152">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d6408-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d6408-153">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d6408-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d6408-154">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="d6408-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d6408-155">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d6408-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d6408-156">румлистс</span><span class="sxs-lookup"><span data-stu-id="d6408-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="d6408-157">Предоставляет список адресов электронной почты и отображаемых имен, представляющих списки комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="d6408-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6408-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d6408-158">Parent elements</span></span>

|<span data-ttu-id="d6408-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6408-159">**Element**</span></span>|<span data-ttu-id="d6408-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6408-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6408-161">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="d6408-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d6408-162">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6408-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d6408-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d6408-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6408-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d6408-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d6408-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d6408-165">Schema Name</span></span>  <br/> |<span data-ttu-id="d6408-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d6408-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d6408-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d6408-167">Validation File</span></span>  <br/> |<span data-ttu-id="d6408-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d6408-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6408-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d6408-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6408-170">False</span><span class="sxs-lookup"><span data-stu-id="d6408-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6408-171">См. также</span><span class="sxs-lookup"><span data-stu-id="d6408-171">See also</span></span>

- [<span data-ttu-id="d6408-172">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="d6408-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="d6408-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d6408-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

