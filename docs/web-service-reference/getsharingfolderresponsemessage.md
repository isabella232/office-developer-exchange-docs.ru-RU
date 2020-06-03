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
ms.openlocfilehash: 85a78a23bac72942c6278b5d97e2bb4c2992ab46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463960"
---
# <a name="getsharingfolderresponsemessage"></a><span data-ttu-id="5e7ed-103">жетшарингфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5e7ed-103">GetSharingFolderResponseMessage</span></span>

<span data-ttu-id="5e7ed-104">Элемент **жетшарингфолдерреспонсемессаже** содержит состояние и результат одного запроса [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5e7ed-104">The **GetSharingFolderResponseMessage** element contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<GetSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponseMessage>
```

 <span data-ttu-id="5e7ed-105">**жетшарингфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e7ed-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5e7ed-106">Attributes and elements</span></span>

<span data-ttu-id="5e7ed-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e7ed-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5e7ed-108">Attributes</span></span>

|<span data-ttu-id="5e7ed-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-109">**Attribute**</span></span>|<span data-ttu-id="5e7ed-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e7ed-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5e7ed-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="5e7ed-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="5e7ed-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="5e7ed-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="5e7ed-114">-  Success</span></span>  <br/><span data-ttu-id="5e7ed-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="5e7ed-115">-  Warning</span></span>  <br/><span data-ttu-id="5e7ed-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="5e7ed-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5e7ed-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="5e7ed-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="5e7ed-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-118">**Value**</span></span>|<span data-ttu-id="5e7ed-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e7ed-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-120">**Success**</span></span> <br/> |<span data-ttu-id="5e7ed-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5e7ed-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-122">**Warning**</span></span> <br/> | <span data-ttu-id="5e7ed-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-123">Describes a request that was not processed.</span></span> <span data-ttu-id="5e7ed-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5e7ed-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5e7ed-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5e7ed-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="5e7ed-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="5e7ed-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5e7ed-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="5e7ed-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="5e7ed-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-132">**Error**</span></span> <br/> | <span data-ttu-id="5e7ed-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5e7ed-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5e7ed-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="5e7ed-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5e7ed-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="5e7ed-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="5e7ed-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="5e7ed-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="5e7ed-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="5e7ed-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="5e7ed-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="5e7ed-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5e7ed-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="5e7ed-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5e7ed-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5e7ed-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5e7ed-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5e7ed-142">Child elements</span></span>

|<span data-ttu-id="5e7ed-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-143">**Element**</span></span>|<span data-ttu-id="5e7ed-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e7ed-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="5e7ed-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5e7ed-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5e7ed-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5e7ed-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5e7ed-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5e7ed-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="5e7ed-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5e7ed-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="5e7ed-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5e7ed-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="5e7ed-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5e7ed-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5e7ed-154">шарингфолдерид</span><span class="sxs-lookup"><span data-stu-id="5e7ed-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="5e7ed-155">Представляет идентификатор локальной папки в отношении совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e7ed-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5e7ed-156">Parent elements</span></span>

|<span data-ttu-id="5e7ed-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-157">**Element**</span></span>|<span data-ttu-id="5e7ed-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e7ed-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e7ed-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="5e7ed-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5e7ed-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e7ed-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="5e7ed-161">Remarks</span></span>

<span data-ttu-id="5e7ed-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5e7ed-162">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e7ed-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5e7ed-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e7ed-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5e7ed-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5e7ed-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5e7ed-165">Schema Name</span></span>  <br/> |<span data-ttu-id="5e7ed-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5e7ed-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5e7ed-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5e7ed-167">Validation File</span></span>  <br/> |<span data-ttu-id="5e7ed-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5e7ed-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5e7ed-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5e7ed-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e7ed-170">False</span><span class="sxs-lookup"><span data-stu-id="5e7ed-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e7ed-171">См. также</span><span class="sxs-lookup"><span data-stu-id="5e7ed-171">See also</span></span>

- [<span data-ttu-id="5e7ed-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5e7ed-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

