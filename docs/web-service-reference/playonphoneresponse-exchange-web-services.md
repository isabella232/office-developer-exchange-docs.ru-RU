---
title: PlayOnPhoneResponse (веб-служб Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 578b70d1-dc9d-4bce-b859-0109b2d2bcec
description: Элемент PlayOnPhoneResponse указывает ответ на запрос для воспроизведения голосовой почты по телефону.
ms.openlocfilehash: 203309bdd6d17b1c78054e673f8a340c2f069b38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834831"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="24c01-103">PlayOnPhoneResponse (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="24c01-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="24c01-104">Элемент **PlayOnPhoneResponse** указывает ответ на запрос для воспроизведения голосовой почты по телефону.</span><span class="sxs-lookup"><span data-stu-id="24c01-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="24c01-105">**PlayOnPhoneResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="24c01-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24c01-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24c01-106">Attributes and elements</span></span>

<span data-ttu-id="24c01-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="24c01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24c01-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24c01-108">Attributes</span></span>

|<span data-ttu-id="24c01-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="24c01-109">**Attribute**</span></span>|<span data-ttu-id="24c01-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24c01-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24c01-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="24c01-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="24c01-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="24c01-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="24c01-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="24c01-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="24c01-114">-Success</span><span class="sxs-lookup"><span data-stu-id="24c01-114">-  Success</span></span>  <br/><span data-ttu-id="24c01-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="24c01-115">-  Warning</span></span>  <br/><span data-ttu-id="24c01-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="24c01-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="24c01-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="24c01-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="24c01-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="24c01-118">**Value**</span></span>|<span data-ttu-id="24c01-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24c01-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24c01-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="24c01-120">**Success**</span></span> <br/> |<span data-ttu-id="24c01-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="24c01-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="24c01-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="24c01-122">**Warning**</span></span> <br/> | <span data-ttu-id="24c01-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="24c01-123">Describes a request that was not processed.</span></span> <span data-ttu-id="24c01-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="24c01-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="24c01-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="24c01-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="24c01-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="24c01-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="24c01-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="24c01-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="24c01-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="24c01-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="24c01-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="24c01-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="24c01-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="24c01-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="24c01-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="24c01-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="24c01-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="24c01-132">**Error**</span></span> <br/> | <span data-ttu-id="24c01-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="24c01-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="24c01-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="24c01-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="24c01-135">-Недопустимых атрибутов и элементов.</span><span class="sxs-lookup"><span data-stu-id="24c01-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="24c01-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="24c01-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="24c01-137">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="24c01-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="24c01-138">-Атрибута или элемента, который не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="24c01-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="24c01-139">-При попытке несанкционированного доступа с любого клиента.</span><span class="sxs-lookup"><span data-stu-id="24c01-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="24c01-140">-На сервере сбой в ответ на допустимый вызовов со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="24c01-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="24c01-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элемент темы.</span><span class="sxs-lookup"><span data-stu-id="24c01-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="24c01-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24c01-142">Child elements</span></span>

|<span data-ttu-id="24c01-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24c01-143">**Element**</span></span>|<span data-ttu-id="24c01-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24c01-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24c01-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="24c01-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="24c01-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="24c01-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="24c01-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24c01-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="24c01-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="24c01-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="24c01-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="24c01-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="24c01-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="24c01-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="24c01-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="24c01-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="24c01-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="24c01-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="24c01-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="24c01-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="24c01-154">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="24c01-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="24c01-155">Задает идентификатор телефонный звонок.</span><span class="sxs-lookup"><span data-stu-id="24c01-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24c01-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24c01-156">Parent elements</span></span>

<span data-ttu-id="24c01-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="24c01-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24c01-158">Замечания</span><span class="sxs-lookup"><span data-stu-id="24c01-158">Remarks</span></span>

<span data-ttu-id="24c01-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="24c01-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24c01-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24c01-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24c01-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24c01-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24c01-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24c01-162">Schema Name</span></span>  <br/> |<span data-ttu-id="24c01-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="24c01-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="24c01-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24c01-164">Validation File</span></span>  <br/> |<span data-ttu-id="24c01-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="24c01-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24c01-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24c01-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="24c01-167">False</span><span class="sxs-lookup"><span data-stu-id="24c01-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24c01-168">См. также</span><span class="sxs-lookup"><span data-stu-id="24c01-168">See also</span></span>

- [<span data-ttu-id="24c01-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="24c01-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

