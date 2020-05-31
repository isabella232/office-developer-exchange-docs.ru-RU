---
title: жетшарингметадатареспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponseMessage
api_type:
- schema
ms.assetid: d81b8708-ebb2-45c2-861f-b9a814eee6ba
description: Элемент Жетшарингметадатареспонсемессаже содержит состояние и результат одного запроса операции GetSharingMetadata.
ms.openlocfilehash: 24da0a78870b2c92e0751eba0631d58076b96eae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833674"
---
# <a name="getsharingmetadataresponsemessage"></a><span data-ttu-id="9241b-103">жетшарингметадатареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9241b-103">GetSharingMetadataResponseMessage</span></span>

<span data-ttu-id="9241b-104">Элемент **жетшарингметадатареспонсемессаже** содержит состояние и результат одного запроса [операции GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9241b-104">The **GetSharingMetadataResponseMessage** element contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponseMessage>
```

 <span data-ttu-id="9241b-105">**жетшарингметадатареспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="9241b-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9241b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9241b-106">Attributes and elements</span></span>

<span data-ttu-id="9241b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9241b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9241b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9241b-108">Attributes</span></span>

|<span data-ttu-id="9241b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9241b-109">**Attribute**</span></span>|<span data-ttu-id="9241b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9241b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9241b-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="9241b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9241b-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="9241b-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="9241b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="9241b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="9241b-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="9241b-114">-  Success</span></span>  <br/><span data-ttu-id="9241b-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="9241b-115">-  Warning</span></span>  <br/><span data-ttu-id="9241b-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="9241b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9241b-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="9241b-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9241b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9241b-118">**Value**</span></span>|<span data-ttu-id="9241b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9241b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9241b-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="9241b-120">**Success**</span></span> <br/> |<span data-ttu-id="9241b-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="9241b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9241b-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9241b-122">**Warning**</span></span> <br/> | <span data-ttu-id="9241b-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="9241b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9241b-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="9241b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9241b-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="9241b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9241b-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="9241b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9241b-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="9241b-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="9241b-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="9241b-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9241b-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="9241b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9241b-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="9241b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9241b-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="9241b-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9241b-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="9241b-132">**Error**</span></span> <br/> | <span data-ttu-id="9241b-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="9241b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9241b-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="9241b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9241b-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="9241b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9241b-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="9241b-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="9241b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="9241b-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="9241b-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="9241b-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="9241b-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="9241b-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9241b-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="9241b-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9241b-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9241b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9241b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9241b-142">Child elements</span></span>

|<span data-ttu-id="9241b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9241b-143">**Element**</span></span>|<span data-ttu-id="9241b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9241b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9241b-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="9241b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9241b-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="9241b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9241b-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="9241b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9241b-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="9241b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9241b-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="9241b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9241b-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="9241b-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="9241b-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="9241b-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9241b-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="9241b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9241b-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="9241b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9241b-154">енкриптедшаредфолдердатаколлектион</span><span class="sxs-lookup"><span data-stu-id="9241b-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="9241b-155">Содержит коллекцию структур данных, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.</span><span class="sxs-lookup"><span data-stu-id="9241b-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="9241b-156">инвалидреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="9241b-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="9241b-157">Представляет недопустимые получатели запроса на общий доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="9241b-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9241b-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9241b-158">Parent elements</span></span>

|<span data-ttu-id="9241b-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9241b-159">**Element**</span></span>|<span data-ttu-id="9241b-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9241b-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9241b-161">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="9241b-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9241b-162">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="9241b-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9241b-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="9241b-163">Remarks</span></span>

<span data-ttu-id="9241b-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9241b-164">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9241b-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9241b-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9241b-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9241b-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9241b-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9241b-167">Schema Name</span></span>  <br/> |<span data-ttu-id="9241b-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9241b-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9241b-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9241b-169">Validation File</span></span>  <br/> |<span data-ttu-id="9241b-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9241b-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9241b-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9241b-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="9241b-172">False</span><span class="sxs-lookup"><span data-stu-id="9241b-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9241b-173">См. также</span><span class="sxs-lookup"><span data-stu-id="9241b-173">See also</span></span>

- [<span data-ttu-id="9241b-174">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="9241b-174">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="9241b-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9241b-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

