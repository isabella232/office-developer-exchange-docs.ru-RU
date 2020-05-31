---
title: жетшарингфолдерреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponse
api_type:
- schema
ms.assetid: fee90e84-3ad4-4c4b-831f-bbc95070aebf
description: Элемент Жетшарингфолдерреспонсе определяет ответ на запрос операции GetSharingFolder.
ms.openlocfilehash: 6d847f1bd80105d52d564770c65b342c89385dad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833675"
---
# <a name="getsharingfolderresponse"></a><span data-ttu-id="39bdb-103">жетшарингфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="39bdb-103">GetSharingFolderResponse</span></span>

<span data-ttu-id="39bdb-104">Элемент **жетшарингфолдерреспонсе** определяет ответ на запрос [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="39bdb-104">The **GetSharingFolderResponse** element defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```XML
<GetSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponse>
```

 <span data-ttu-id="39bdb-105">**жетшарингфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="39bdb-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39bdb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="39bdb-106">Attributes and elements</span></span>

<span data-ttu-id="39bdb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="39bdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39bdb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="39bdb-108">Attributes</span></span>

|<span data-ttu-id="39bdb-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="39bdb-109">**Attribute**</span></span>|<span data-ttu-id="39bdb-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39bdb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39bdb-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="39bdb-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="39bdb-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="39bdb-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="39bdb-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="39bdb-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="39bdb-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="39bdb-114">-  Success</span></span>  <br/><span data-ttu-id="39bdb-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="39bdb-115">-  Warning</span></span>  <br/><span data-ttu-id="39bdb-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="39bdb-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="39bdb-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="39bdb-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="39bdb-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="39bdb-118">**Value**</span></span>|<span data-ttu-id="39bdb-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39bdb-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39bdb-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="39bdb-120">**Success**</span></span> <br/> |<span data-ttu-id="39bdb-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="39bdb-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="39bdb-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="39bdb-122">**Warning**</span></span> <br/> | <span data-ttu-id="39bdb-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="39bdb-123">Describes a request that was not processed.</span></span> <span data-ttu-id="39bdb-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="39bdb-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="39bdb-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="39bdb-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="39bdb-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="39bdb-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="39bdb-127">-Служба каталогов Active Directory или доменные службы Active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="39bdb-127">-  The Active Directory directory service or Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="39bdb-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="39bdb-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="39bdb-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="39bdb-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="39bdb-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="39bdb-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="39bdb-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="39bdb-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="39bdb-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="39bdb-132">**Error**</span></span> <br/> | <span data-ttu-id="39bdb-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="39bdb-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="39bdb-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="39bdb-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="39bdb-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="39bdb-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="39bdb-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="39bdb-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="39bdb-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="39bdb-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="39bdb-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="39bdb-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="39bdb-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="39bdb-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="39bdb-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="39bdb-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="39bdb-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="39bdb-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="39bdb-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="39bdb-142">Child elements</span></span>

|<span data-ttu-id="39bdb-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39bdb-143">**Element**</span></span>|<span data-ttu-id="39bdb-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39bdb-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39bdb-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="39bdb-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="39bdb-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="39bdb-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="39bdb-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="39bdb-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="39bdb-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="39bdb-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="39bdb-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="39bdb-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="39bdb-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="39bdb-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="39bdb-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="39bdb-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="39bdb-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="39bdb-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="39bdb-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="39bdb-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="39bdb-154">шарингфолдерид</span><span class="sxs-lookup"><span data-stu-id="39bdb-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="39bdb-155">Представляет идентификатор локальной папки в отношении совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="39bdb-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39bdb-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="39bdb-156">Parent elements</span></span>

<span data-ttu-id="39bdb-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="39bdb-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39bdb-158">Примечания</span><span class="sxs-lookup"><span data-stu-id="39bdb-158">Remarks</span></span>

<span data-ttu-id="39bdb-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="39bdb-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39bdb-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="39bdb-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39bdb-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="39bdb-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39bdb-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="39bdb-162">Schema Name</span></span>  <br/> |<span data-ttu-id="39bdb-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="39bdb-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39bdb-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="39bdb-164">Validation File</span></span>  <br/> |<span data-ttu-id="39bdb-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="39bdb-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39bdb-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="39bdb-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="39bdb-167">False</span><span class="sxs-lookup"><span data-stu-id="39bdb-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39bdb-168">См. также</span><span class="sxs-lookup"><span data-stu-id="39bdb-168">See also</span></span>

- [<span data-ttu-id="39bdb-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39bdb-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

