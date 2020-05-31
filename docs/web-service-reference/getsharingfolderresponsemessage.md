---
title: жетшарингфолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponseMessage
api_type:
- schema
ms.assetid: b6f5fd09-09f3-4e34-84b4-2f6c1f10f28f
description: Элемент Жетшарингфолдерреспонсемессаже содержит состояние и результат одного запроса операции GetSharingFolder.
ms.openlocfilehash: 13ce3f628ff125140fc7459df5d567a67ddf7bc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833672"
---
# <a name="getsharingfolderresponsemessage"></a><span data-ttu-id="b08aa-103">жетшарингфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b08aa-103">GetSharingFolderResponseMessage</span></span>

<span data-ttu-id="b08aa-104">Элемент **жетшарингфолдерреспонсемессаже** содержит состояние и результат одного запроса [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b08aa-104">The **GetSharingFolderResponseMessage** element contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<GetSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponseMessage>
```

 <span data-ttu-id="b08aa-105">**жетшарингфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="b08aa-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b08aa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b08aa-106">Attributes and elements</span></span>

<span data-ttu-id="b08aa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b08aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b08aa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b08aa-108">Attributes</span></span>

|<span data-ttu-id="b08aa-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b08aa-109">**Attribute**</span></span>|<span data-ttu-id="b08aa-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b08aa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b08aa-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="b08aa-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b08aa-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="b08aa-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b08aa-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="b08aa-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b08aa-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="b08aa-114">-  Success</span></span>  <br/><span data-ttu-id="b08aa-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="b08aa-115">-  Warning</span></span>  <br/><span data-ttu-id="b08aa-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="b08aa-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b08aa-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="b08aa-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b08aa-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b08aa-118">**Value**</span></span>|<span data-ttu-id="b08aa-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b08aa-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b08aa-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="b08aa-120">**Success**</span></span> <br/> |<span data-ttu-id="b08aa-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="b08aa-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b08aa-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b08aa-122">**Warning**</span></span> <br/> | <span data-ttu-id="b08aa-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="b08aa-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b08aa-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="b08aa-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b08aa-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="b08aa-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b08aa-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="b08aa-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b08aa-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b08aa-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="b08aa-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="b08aa-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b08aa-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b08aa-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b08aa-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="b08aa-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b08aa-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="b08aa-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b08aa-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="b08aa-132">**Error**</span></span> <br/> | <span data-ttu-id="b08aa-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="b08aa-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b08aa-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="b08aa-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b08aa-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="b08aa-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b08aa-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="b08aa-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b08aa-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="b08aa-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="b08aa-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="b08aa-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b08aa-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="b08aa-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b08aa-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="b08aa-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b08aa-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b08aa-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b08aa-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b08aa-142">Child elements</span></span>

|<span data-ttu-id="b08aa-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b08aa-143">**Element**</span></span>|<span data-ttu-id="b08aa-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b08aa-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b08aa-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b08aa-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b08aa-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="b08aa-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b08aa-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b08aa-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b08aa-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="b08aa-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b08aa-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b08aa-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b08aa-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="b08aa-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b08aa-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="b08aa-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b08aa-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="b08aa-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b08aa-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b08aa-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b08aa-154">шарингфолдерид</span><span class="sxs-lookup"><span data-stu-id="b08aa-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="b08aa-155">Представляет идентификатор локальной папки в отношении совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="b08aa-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b08aa-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b08aa-156">Parent elements</span></span>

|<span data-ttu-id="b08aa-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b08aa-157">**Element**</span></span>|<span data-ttu-id="b08aa-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b08aa-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b08aa-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b08aa-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b08aa-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b08aa-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b08aa-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="b08aa-161">Remarks</span></span>

<span data-ttu-id="b08aa-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b08aa-162">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b08aa-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b08aa-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b08aa-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b08aa-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b08aa-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b08aa-165">Schema Name</span></span>  <br/> |<span data-ttu-id="b08aa-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b08aa-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b08aa-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b08aa-167">Validation File</span></span>  <br/> |<span data-ttu-id="b08aa-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b08aa-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b08aa-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b08aa-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="b08aa-170">False</span><span class="sxs-lookup"><span data-stu-id="b08aa-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b08aa-171">См. также</span><span class="sxs-lookup"><span data-stu-id="b08aa-171">See also</span></span>

- [<span data-ttu-id="b08aa-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b08aa-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

