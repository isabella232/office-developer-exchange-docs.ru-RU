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
description: Элемент MailTipsResponseMessageType представляет параметры подсказок почты.
ms.openlocfilehash: 5244f26ef927a817a9087c299fd1124acb828aa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454038"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="6b989-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="6b989-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="6b989-104">Элемент **MailTipsResponseMessageType** представляет параметры подсказок почты.</span><span class="sxs-lookup"><span data-stu-id="6b989-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="6b989-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6b989-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b989-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b989-106">Attributes and elements</span></span>

<span data-ttu-id="6b989-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6b989-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b989-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b989-108">Attributes</span></span>

|<span data-ttu-id="6b989-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6b989-109">**Attribute**</span></span>|<span data-ttu-id="6b989-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b989-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b989-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6b989-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6b989-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="6b989-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="6b989-113">Для данного атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="6b989-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6b989-114">–  Success</span><span class="sxs-lookup"><span data-stu-id="6b989-114">-  Success</span></span>  <br/><span data-ttu-id="6b989-115">–  Warning</span><span class="sxs-lookup"><span data-stu-id="6b989-115">-  Warning</span></span>  <br/><span data-ttu-id="6b989-116">–  Error</span><span class="sxs-lookup"><span data-stu-id="6b989-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="6b989-117">Значения атрибута ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6b989-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="6b989-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6b989-118">**Value**</span></span>|<span data-ttu-id="6b989-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b989-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b989-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="6b989-120">**Success**</span></span> <br/> |<span data-ttu-id="6b989-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="6b989-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6b989-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="6b989-122">**Warning**</span></span> <br/> | <span data-ttu-id="6b989-123">Описывает необработанный запрос.</span><span class="sxs-lookup"><span data-stu-id="6b989-123">Describes a request that was not processed.</span></span> <span data-ttu-id="6b989-124">Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.</span><span class="sxs-lookup"><span data-stu-id="6b989-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="6b989-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="6b989-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="6b989-126">– Хранилище Exchange находится в автономном режиме при обработке пакета.</span><span class="sxs-lookup"><span data-stu-id="6b989-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6b989-127">– Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6b989-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6b989-128">- Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="6b989-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="6b989-129">– База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6b989-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6b989-130">– Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="6b989-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="6b989-131">- Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="6b989-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="6b989-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="6b989-132">**Error**</span></span> <br/> | <span data-ttu-id="6b989-133">Описывает запрос, который невозможно выполнить.</span><span class="sxs-lookup"><span data-stu-id="6b989-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6b989-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="6b989-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="6b989-135">– Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="6b989-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6b989-136">- Атрибуты или элементы, которые находятся вне диапазона</span><span class="sxs-lookup"><span data-stu-id="6b989-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="6b989-137">- Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="6b989-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="6b989-138">- Атрибут или элемент, не допустимый в контексте</span><span class="sxs-lookup"><span data-stu-id="6b989-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="6b989-139">- Несанкционированная попытка доступа со стороны любого клиента</span><span class="sxs-lookup"><span data-stu-id="6b989-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6b989-140">- Сбой на стороне сервера в ответ на допустимый вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="6b989-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="6b989-141">Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).</span><span class="sxs-lookup"><span data-stu-id="6b989-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6b989-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b989-142">Child elements</span></span>

|<span data-ttu-id="6b989-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b989-143">**Element**</span></span>|<span data-ttu-id="6b989-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b989-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b989-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="6b989-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6b989-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="6b989-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6b989-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6b989-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6b989-148">Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.</span><span class="sxs-lookup"><span data-stu-id="6b989-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6b989-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6b989-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6b989-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="6b989-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="6b989-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="6b989-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6b989-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6b989-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6b989-153">Предоставляет дополнительные сведения об отклике с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="6b989-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6b989-154">Подсказки</span><span class="sxs-lookup"><span data-stu-id="6b989-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="6b989-155">Представляет значения для различных типов подсказок.</span><span class="sxs-lookup"><span data-stu-id="6b989-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b989-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b989-156">Parent elements</span></span>

|<span data-ttu-id="6b989-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b989-157">**Element**</span></span>|<span data-ttu-id="6b989-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b989-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b989-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="6b989-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="6b989-160">Представляет список ответных сообщений с подсказками электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6b989-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b989-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6b989-161">Text value</span></span>

<span data-ttu-id="6b989-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b989-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b989-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="6b989-163">Remarks</span></span>

<span data-ttu-id="6b989-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b989-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b989-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b989-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b989-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b989-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b989-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b989-167">Schema Name</span></span>  <br/> |<span data-ttu-id="6b989-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6b989-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b989-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b989-169">Validation File</span></span>  <br/> |<span data-ttu-id="6b989-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b989-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b989-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b989-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b989-172">False</span><span class="sxs-lookup"><span data-stu-id="6b989-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b989-173">См. также</span><span class="sxs-lookup"><span data-stu-id="6b989-173">See also</span></span>

- [<span data-ttu-id="6b989-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6b989-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

