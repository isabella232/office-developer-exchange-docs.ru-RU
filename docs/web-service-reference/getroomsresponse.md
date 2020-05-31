---
title: жетрумсреспонсе
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
description: Элемент Жетрумсреспонсе определяет ответ на запрос операции с запросом на получение помещений.
ms.openlocfilehash: 7399ab910a99b39757eb752b11a4771ba81be46a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762907"
---
# <a name="getroomsresponse"></a><span data-ttu-id="cb5f2-103">жетрумсреспонсе</span><span class="sxs-lookup"><span data-stu-id="cb5f2-103">GetRoomsResponse</span></span>

<span data-ttu-id="cb5f2-104">Элемент **жетрумсреспонсе** определяет ответ на запрос операции с запросом на получение [помещений](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cb5f2-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="cb5f2-105">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="cb5f2-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="cb5f2-106">жетрумсреспонсе</span><span class="sxs-lookup"><span data-stu-id="cb5f2-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="cb5f2-107">**жетрумсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb5f2-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cb5f2-108">Attributes and elements</span></span>

<span data-ttu-id="cb5f2-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb5f2-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cb5f2-110">Attributes</span></span>

|<span data-ttu-id="cb5f2-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-111">**Attribute**</span></span>|<span data-ttu-id="cb5f2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb5f2-113">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="cb5f2-114">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="cb5f2-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="cb5f2-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="cb5f2-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="cb5f2-116">-  Success</span></span>  <br/><span data-ttu-id="cb5f2-117">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="cb5f2-117">-  Warning</span></span>  <br/><span data-ttu-id="cb5f2-118">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="cb5f2-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="cb5f2-119">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="cb5f2-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="cb5f2-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-120">**Value**</span></span>|<span data-ttu-id="cb5f2-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb5f2-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-122">**Success**</span></span> <br/> |<span data-ttu-id="cb5f2-123">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="cb5f2-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-124">**Warning**</span></span> <br/> | <span data-ttu-id="cb5f2-125">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-125">Describes a request that was not processed.</span></span> <span data-ttu-id="cb5f2-126">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="cb5f2-127">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="cb5f2-128">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="cb5f2-129">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="cb5f2-130">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="cb5f2-131">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="cb5f2-132">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="cb5f2-133">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="cb5f2-134">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-134">**Error**</span></span> <br/> | <span data-ttu-id="cb5f2-135">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="cb5f2-136">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="cb5f2-137">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="cb5f2-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="cb5f2-138">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="cb5f2-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="cb5f2-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="cb5f2-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="cb5f2-140">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="cb5f2-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="cb5f2-141">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="cb5f2-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="cb5f2-142">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="cb5f2-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="cb5f2-143">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="cb5f2-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cb5f2-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cb5f2-144">Child elements</span></span>

|<span data-ttu-id="cb5f2-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-145">**Element**</span></span>|<span data-ttu-id="cb5f2-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb5f2-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="cb5f2-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cb5f2-148">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cb5f2-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="cb5f2-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cb5f2-150">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cb5f2-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="cb5f2-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cb5f2-152">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="cb5f2-153">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cb5f2-154">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="cb5f2-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cb5f2-155">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="cb5f2-156">Комната</span><span class="sxs-lookup"><span data-stu-id="cb5f2-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="cb5f2-157">Предоставляет список адресов электронной почты и отображаемые имена, представляющие комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb5f2-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cb5f2-158">Parent elements</span></span>

|<span data-ttu-id="cb5f2-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-159">**Element**</span></span>|<span data-ttu-id="cb5f2-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb5f2-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb5f2-161">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="cb5f2-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cb5f2-162">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb5f2-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="cb5f2-163">Remarks</span></span>

<span data-ttu-id="cb5f2-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb5f2-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cb5f2-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb5f2-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cb5f2-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb5f2-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cb5f2-167">Schema Name</span></span>  <br/> |<span data-ttu-id="cb5f2-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cb5f2-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb5f2-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cb5f2-169">Validation File</span></span>  <br/> |<span data-ttu-id="cb5f2-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cb5f2-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb5f2-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cb5f2-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb5f2-172">False</span><span class="sxs-lookup"><span data-stu-id="cb5f2-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb5f2-173">См. также</span><span class="sxs-lookup"><span data-stu-id="cb5f2-173">See also</span></span>

- [<span data-ttu-id="cb5f2-174">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="cb5f2-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="cb5f2-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cb5f2-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

