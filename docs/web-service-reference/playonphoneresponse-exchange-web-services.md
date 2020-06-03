---
title: PlayOnPhoneResponse (веб-службы Exchange)
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
description: Элемент PlayOnPhoneResponse указывает ответ на запрос на проигрывание голосовой почты по телефону.
ms.openlocfilehash: 907864d7fe669aac99b2ff6d1c5eba71b9ddf79f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459625"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="0eea6-103">PlayOnPhoneResponse (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="0eea6-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="0eea6-104">Элемент **PlayOnPhoneResponse** указывает ответ на запрос на проигрывание голосовой почты по телефону.</span><span class="sxs-lookup"><span data-stu-id="0eea6-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="0eea6-105">**плайонфонереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="0eea6-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0eea6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0eea6-106">Attributes and elements</span></span>

<span data-ttu-id="0eea6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0eea6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0eea6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0eea6-108">Attributes</span></span>

|<span data-ttu-id="0eea6-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0eea6-109">**Attribute**</span></span>|<span data-ttu-id="0eea6-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0eea6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0eea6-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="0eea6-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0eea6-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="0eea6-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0eea6-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="0eea6-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0eea6-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="0eea6-114">-  Success</span></span>  <br/><span data-ttu-id="0eea6-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="0eea6-115">-  Warning</span></span>  <br/><span data-ttu-id="0eea6-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="0eea6-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0eea6-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="0eea6-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="0eea6-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0eea6-118">**Value**</span></span>|<span data-ttu-id="0eea6-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0eea6-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0eea6-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="0eea6-120">**Success**</span></span> <br/> |<span data-ttu-id="0eea6-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="0eea6-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0eea6-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0eea6-122">**Warning**</span></span> <br/> | <span data-ttu-id="0eea6-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="0eea6-123">Describes a request that was not processed.</span></span> <span data-ttu-id="0eea6-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="0eea6-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="0eea6-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="0eea6-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="0eea6-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="0eea6-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0eea6-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0eea6-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0eea6-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="0eea6-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0eea6-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="0eea6-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0eea6-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="0eea6-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="0eea6-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="0eea6-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0eea6-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="0eea6-132">**Error**</span></span> <br/> | <span data-ttu-id="0eea6-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="0eea6-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0eea6-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="0eea6-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0eea6-135">— Недопустимые атрибуты или элементы.</span><span class="sxs-lookup"><span data-stu-id="0eea6-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="0eea6-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="0eea6-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0eea6-137">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="0eea6-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="0eea6-138">— Атрибут или элемент, который не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="0eea6-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="0eea6-139">— Попытки несанкционированного доступа, выполняемые любым клиентом.</span><span class="sxs-lookup"><span data-stu-id="0eea6-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="0eea6-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="0eea6-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="0eea6-141">Сведения об ошибке можно найти в разделах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0eea6-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0eea6-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0eea6-142">Child elements</span></span>

|<span data-ttu-id="0eea6-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0eea6-143">**Element**</span></span>|<span data-ttu-id="0eea6-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0eea6-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0eea6-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="0eea6-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0eea6-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="0eea6-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0eea6-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0eea6-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0eea6-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="0eea6-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0eea6-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="0eea6-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0eea6-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="0eea6-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="0eea6-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="0eea6-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0eea6-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="0eea6-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0eea6-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0eea6-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0eea6-154">фонекаллид</span><span class="sxs-lookup"><span data-stu-id="0eea6-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="0eea6-155">Задает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="0eea6-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0eea6-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0eea6-156">Parent elements</span></span>

<span data-ttu-id="0eea6-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="0eea6-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0eea6-158">Примечания</span><span class="sxs-lookup"><span data-stu-id="0eea6-158">Remarks</span></span>

<span data-ttu-id="0eea6-159">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0eea6-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0eea6-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0eea6-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0eea6-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0eea6-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0eea6-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0eea6-162">Schema Name</span></span>  <br/> |<span data-ttu-id="0eea6-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0eea6-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0eea6-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0eea6-164">Validation File</span></span>  <br/> |<span data-ttu-id="0eea6-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0eea6-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0eea6-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0eea6-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="0eea6-167">False</span><span class="sxs-lookup"><span data-stu-id="0eea6-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0eea6-168">См. также</span><span class="sxs-lookup"><span data-stu-id="0eea6-168">See also</span></span>

- [<span data-ttu-id="0eea6-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0eea6-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

