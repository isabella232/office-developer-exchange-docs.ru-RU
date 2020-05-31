---
title: жетшарингметадатареспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponse
api_type:
- schema
ms.assetid: 1acc2d8f-7104-4b36-9c04-dd4fc4f571bb
description: Элемент Жетшарингметадатареспонсе определяет ответ на запрос операции GetSharingMetadata.
ms.openlocfilehash: 820b5bf7aa5528b61aa6649e5b1886885b5f022e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833676"
---
# <a name="getsharingmetadataresponse"></a><span data-ttu-id="a2a43-103">жетшарингметадатареспонсе</span><span class="sxs-lookup"><span data-stu-id="a2a43-103">GetSharingMetadataResponse</span></span>

<span data-ttu-id="a2a43-104">Элемент **жетшарингметадатареспонсе** определяет ответ на запрос [операции GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a2a43-104">The **GetSharingMetadataResponse** element defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponse>
```

 <span data-ttu-id="a2a43-105">**жетшарингметадатареспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="a2a43-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2a43-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2a43-106">Attributes and elements</span></span>

<span data-ttu-id="a2a43-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a2a43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2a43-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2a43-108">Attributes</span></span>

|<span data-ttu-id="a2a43-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a2a43-109">**Attribute**</span></span>|<span data-ttu-id="a2a43-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2a43-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2a43-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="a2a43-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a2a43-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="a2a43-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="a2a43-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="a2a43-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a2a43-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="a2a43-114">-  Success</span></span>  <br/><span data-ttu-id="a2a43-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="a2a43-115">-  Warning</span></span>  <br/><span data-ttu-id="a2a43-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="a2a43-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a2a43-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="a2a43-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="a2a43-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a2a43-118">**Value**</span></span>|<span data-ttu-id="a2a43-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2a43-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2a43-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="a2a43-120">**Success**</span></span> <br/> |<span data-ttu-id="a2a43-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="a2a43-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a2a43-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="a2a43-122">**Warning**</span></span> <br/> | <span data-ttu-id="a2a43-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="a2a43-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a2a43-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="a2a43-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a2a43-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="a2a43-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a2a43-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="a2a43-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a2a43-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a2a43-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="a2a43-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="a2a43-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a2a43-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a2a43-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a2a43-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="a2a43-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a2a43-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="a2a43-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a2a43-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="a2a43-132">**Error**</span></span> <br/> | <span data-ttu-id="a2a43-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="a2a43-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a2a43-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="a2a43-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a2a43-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="a2a43-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a2a43-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="a2a43-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a2a43-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="a2a43-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="a2a43-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="a2a43-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a2a43-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="a2a43-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a2a43-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="a2a43-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="a2a43-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a2a43-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2a43-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2a43-142">Child elements</span></span>

|<span data-ttu-id="a2a43-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2a43-143">**Element**</span></span>|<span data-ttu-id="a2a43-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2a43-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2a43-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="a2a43-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a2a43-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="a2a43-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a2a43-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a2a43-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a2a43-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="a2a43-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a2a43-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="a2a43-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a2a43-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="a2a43-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a2a43-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="a2a43-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a2a43-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="a2a43-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a2a43-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a2a43-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a2a43-154">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="a2a43-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="a2a43-155">Содержит коллекцию структур данных, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="a2a43-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="a2a43-156">инвалидреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="a2a43-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="a2a43-157">Представляет недопустимые получатели запроса на общий доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="a2a43-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2a43-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2a43-158">Parent elements</span></span>

<span data-ttu-id="a2a43-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2a43-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2a43-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="a2a43-160">Remarks</span></span>

<span data-ttu-id="a2a43-161">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2a43-161">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2a43-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2a43-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2a43-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2a43-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2a43-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2a43-164">Schema Name</span></span>  <br/> |<span data-ttu-id="a2a43-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a2a43-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2a43-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2a43-166">Validation File</span></span>  <br/> |<span data-ttu-id="a2a43-167">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a2a43-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2a43-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2a43-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2a43-169">False</span><span class="sxs-lookup"><span data-stu-id="a2a43-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2a43-170">См. также</span><span class="sxs-lookup"><span data-stu-id="a2a43-170">See also</span></span>

- [<span data-ttu-id="a2a43-171">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a2a43-171">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="a2a43-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a43-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

