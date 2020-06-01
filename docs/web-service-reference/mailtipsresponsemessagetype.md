---
title: маилтипсреспонсемессажетипе
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
description: Элемент Маилтипсреспонсемессажетипе представляет параметры советов по электронной почте.
ms.openlocfilehash: 5244f26ef927a817a9087c299fd1124acb828aa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454038"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="564de-103">маилтипсреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="564de-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="564de-104">Элемент **маилтипсреспонсемессажетипе** представляет параметры советов по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="564de-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="564de-105">**маилтипсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="564de-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="564de-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="564de-106">Attributes and elements</span></span>

<span data-ttu-id="564de-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="564de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="564de-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="564de-108">Attributes</span></span>

|<span data-ttu-id="564de-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="564de-109">**Attribute**</span></span>|<span data-ttu-id="564de-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="564de-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="564de-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="564de-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="564de-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="564de-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="564de-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="564de-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="564de-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="564de-114">-  Success</span></span>  <br/><span data-ttu-id="564de-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="564de-115">-  Warning</span></span>  <br/><span data-ttu-id="564de-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="564de-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="564de-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="564de-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="564de-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="564de-118">**Value**</span></span>|<span data-ttu-id="564de-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="564de-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="564de-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="564de-120">**Success**</span></span> <br/> |<span data-ttu-id="564de-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="564de-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="564de-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="564de-122">**Warning**</span></span> <br/> | <span data-ttu-id="564de-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="564de-123">Describes a request that was not processed.</span></span> <span data-ttu-id="564de-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="564de-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="564de-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="564de-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="564de-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="564de-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="564de-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="564de-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="564de-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="564de-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="564de-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="564de-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="564de-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="564de-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="564de-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="564de-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="564de-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="564de-132">**Error**</span></span> <br/> | <span data-ttu-id="564de-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="564de-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="564de-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="564de-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="564de-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="564de-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="564de-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="564de-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="564de-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="564de-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="564de-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="564de-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="564de-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="564de-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="564de-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="564de-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="564de-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="564de-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="564de-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="564de-142">Child elements</span></span>

|<span data-ttu-id="564de-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="564de-143">**Element**</span></span>|<span data-ttu-id="564de-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="564de-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="564de-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="564de-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="564de-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="564de-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="564de-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="564de-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="564de-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="564de-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="564de-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="564de-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="564de-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="564de-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="564de-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="564de-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="564de-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="564de-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="564de-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="564de-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="564de-154">Подсказки</span><span class="sxs-lookup"><span data-stu-id="564de-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="564de-155">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="564de-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="564de-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="564de-156">Parent elements</span></span>

|<span data-ttu-id="564de-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="564de-157">**Element**</span></span>|<span data-ttu-id="564de-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="564de-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="564de-159">Респонсемессажес (Аррайофмаилтипсреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="564de-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="564de-160">Представляет список ответных сообщений с советами по почте.</span><span class="sxs-lookup"><span data-stu-id="564de-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="564de-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="564de-161">Text value</span></span>

<span data-ttu-id="564de-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="564de-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="564de-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="564de-163">Remarks</span></span>

<span data-ttu-id="564de-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="564de-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="564de-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="564de-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="564de-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="564de-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="564de-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="564de-167">Schema Name</span></span>  <br/> |<span data-ttu-id="564de-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="564de-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="564de-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="564de-169">Validation File</span></span>  <br/> |<span data-ttu-id="564de-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="564de-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="564de-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="564de-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="564de-172">False</span><span class="sxs-lookup"><span data-stu-id="564de-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="564de-173">См. также</span><span class="sxs-lookup"><span data-stu-id="564de-173">See also</span></span>

- [<span data-ttu-id="564de-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="564de-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

