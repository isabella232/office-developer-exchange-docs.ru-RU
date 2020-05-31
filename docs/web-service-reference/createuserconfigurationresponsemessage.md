---
title: креатеусерконфигуратионреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 9c11427c-74c9-4c6a-a0e7-7d5556670c1e
description: Элемент Креатеусерконфигуратионреспонсемессаже содержит состояние и результат одного запроса CreateUserConfiguration.
ms.openlocfilehash: 718d62d9f5b920eaf9481054b095958a9f44cbf8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761934"
---
# <a name="createuserconfigurationresponsemessage"></a><span data-ttu-id="30468-103">креатеусерконфигуратионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="30468-103">CreateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="30468-104">Элемент **креатеусерконфигуратионреспонсемессаже** содержит состояние и результат одного запроса **CreateUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="30468-104">The **CreateUserConfigurationResponseMessage** element contains the status and result of a single **CreateUserConfiguration** request.</span></span> 
  
```xml
<CreateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</CreateUserConfigurationResponseMessage>
```

<span data-ttu-id="30468-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="30468-105">**ResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="30468-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="30468-106">Attributes and elements</span></span>

<span data-ttu-id="30468-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="30468-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30468-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="30468-108">Attributes</span></span>

|<span data-ttu-id="30468-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="30468-109">**Attribute**</span></span>|<span data-ttu-id="30468-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30468-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30468-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="30468-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="30468-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="30468-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="30468-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="30468-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="30468-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="30468-114">-  Success</span></span>  <br/><span data-ttu-id="30468-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="30468-115">-  Warning</span></span>  <br/><span data-ttu-id="30468-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="30468-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="30468-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="30468-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="30468-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="30468-118">**Value**</span></span>|<span data-ttu-id="30468-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30468-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30468-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="30468-120">**Success**</span></span> <br/> |<span data-ttu-id="30468-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="30468-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="30468-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="30468-122">**Warning**</span></span> <br/> | <span data-ttu-id="30468-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="30468-123">Describes a request that was not processed.</span></span> <span data-ttu-id="30468-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="30468-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="30468-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="30468-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="30468-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="30468-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="30468-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="30468-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="30468-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="30468-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="30468-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="30468-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="30468-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="30468-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="30468-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="30468-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="30468-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="30468-132">**Error**</span></span> <br/> | <span data-ttu-id="30468-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="30468-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="30468-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="30468-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="30468-135">— Недопустимые атрибуты или элементы.</span><span class="sxs-lookup"><span data-stu-id="30468-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="30468-136">— Атрибуты или элементы, которые выходят за пределы диапазона.</span><span class="sxs-lookup"><span data-stu-id="30468-136">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="30468-137">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="30468-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="30468-138">— Атрибут или элемент не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="30468-138">-  The attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="30468-139">— Попытки несанкционированного доступа, выполняемые любым клиентом.</span><span class="sxs-lookup"><span data-stu-id="30468-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="30468-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="30468-140">-  A server-side failure in response to a valid client-side call.</span></span><br/><br/>  <span data-ttu-id="30468-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="30468-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="30468-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="30468-142">Child elements</span></span>

|<span data-ttu-id="30468-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="30468-143">**Element**</span></span>|<span data-ttu-id="30468-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30468-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30468-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="30468-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="30468-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="30468-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="30468-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="30468-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="30468-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="30468-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="30468-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="30468-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="30468-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="30468-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="30468-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="30468-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="30468-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="30468-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="30468-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="30468-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30468-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="30468-154">Parent elements</span></span>

|<span data-ttu-id="30468-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="30468-155">**Element**</span></span>|<span data-ttu-id="30468-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30468-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30468-157">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="30468-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="30468-158">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="30468-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30468-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="30468-159">Text value</span></span>

<span data-ttu-id="30468-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="30468-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30468-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="30468-161">Remarks</span></span>

<span data-ttu-id="30468-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="30468-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30468-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="30468-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30468-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="30468-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30468-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="30468-165">Schema Name</span></span>  <br/> |<span data-ttu-id="30468-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="30468-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30468-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="30468-167">Validation File</span></span>  <br/> |<span data-ttu-id="30468-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="30468-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30468-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="30468-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="30468-170">False</span><span class="sxs-lookup"><span data-stu-id="30468-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30468-171">См. также</span><span class="sxs-lookup"><span data-stu-id="30468-171">See also</span></span>

- [<span data-ttu-id="30468-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="30468-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

