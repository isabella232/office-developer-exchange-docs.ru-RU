---
title: MailTipsResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsResponseMessageType
api_type:
- schema
ms.assetid: 532cb9d9-1232-4e88-80aa-4cf163eb05da
description: Элемент MailTipsResponseMessageType представляет советы параметры электронной почты.
ms.openlocfilehash: 76a1e33ae189b96a96a41d1bc7a8f79116761c4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834334"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="75b57-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="75b57-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="75b57-104">Элемент **MailTipsResponseMessageType** представляет советы параметры электронной почты.</span><span class="sxs-lookup"><span data-stu-id="75b57-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="75b57-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="75b57-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75b57-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75b57-106">Attributes and elements</span></span>

<span data-ttu-id="75b57-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="75b57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75b57-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75b57-108">Attributes</span></span>

|<span data-ttu-id="75b57-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="75b57-109">**Attribute**</span></span>|<span data-ttu-id="75b57-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75b57-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75b57-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="75b57-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="75b57-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="75b57-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="75b57-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="75b57-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="75b57-114">-Success</span><span class="sxs-lookup"><span data-stu-id="75b57-114">-  Success</span></span>  <br/><span data-ttu-id="75b57-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="75b57-115">-  Warning</span></span>  <br/><span data-ttu-id="75b57-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="75b57-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="75b57-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="75b57-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="75b57-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="75b57-118">**Value**</span></span>|<span data-ttu-id="75b57-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75b57-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75b57-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="75b57-120">**Success**</span></span> <br/> |<span data-ttu-id="75b57-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="75b57-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="75b57-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="75b57-122">**Warning**</span></span> <br/> | <span data-ttu-id="75b57-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="75b57-123">Describes a request that was not processed.</span></span> <span data-ttu-id="75b57-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="75b57-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="75b57-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="75b57-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="75b57-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="75b57-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="75b57-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="75b57-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="75b57-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="75b57-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="75b57-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="75b57-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="75b57-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="75b57-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="75b57-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="75b57-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="75b57-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="75b57-132">**Error**</span></span> <br/> | <span data-ttu-id="75b57-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="75b57-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="75b57-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="75b57-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="75b57-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75b57-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="75b57-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="75b57-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="75b57-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="75b57-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="75b57-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="75b57-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="75b57-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="75b57-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="75b57-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="75b57-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="75b57-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="75b57-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="75b57-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75b57-142">Child elements</span></span>

|<span data-ttu-id="75b57-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75b57-143">**Element**</span></span>|<span data-ttu-id="75b57-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75b57-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75b57-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="75b57-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="75b57-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="75b57-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="75b57-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="75b57-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="75b57-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="75b57-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="75b57-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="75b57-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="75b57-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="75b57-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="75b57-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="75b57-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="75b57-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="75b57-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="75b57-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="75b57-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="75b57-154">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="75b57-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="75b57-155">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="75b57-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="75b57-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75b57-156">Parent elements</span></span>

|<span data-ttu-id="75b57-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75b57-157">**Element**</span></span>|<span data-ttu-id="75b57-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75b57-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75b57-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="75b57-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="75b57-160">Представляет список ответа советы почтовых сообщений.</span><span class="sxs-lookup"><span data-stu-id="75b57-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75b57-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75b57-161">Text value</span></span>

<span data-ttu-id="75b57-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="75b57-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75b57-163">Замечания</span><span class="sxs-lookup"><span data-stu-id="75b57-163">Remarks</span></span>

<span data-ttu-id="75b57-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="75b57-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75b57-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="75b57-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75b57-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="75b57-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="75b57-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="75b57-167">Schema Name</span></span>  <br/> |<span data-ttu-id="75b57-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="75b57-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="75b57-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="75b57-169">Validation File</span></span>  <br/> |<span data-ttu-id="75b57-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="75b57-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="75b57-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="75b57-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="75b57-172">False</span><span class="sxs-lookup"><span data-stu-id="75b57-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75b57-173">См. также</span><span class="sxs-lookup"><span data-stu-id="75b57-173">See also</span></span>

- [<span data-ttu-id="75b57-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="75b57-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

