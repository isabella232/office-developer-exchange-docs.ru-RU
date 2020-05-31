---
title: жетусерконфигуратионреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: f75e29eb-ae98-46fd-8da2-1c76a57f5458
description: Элемент Жетусерконфигуратионреспонсемессаже представляет ответ, который возвращает объект конфигурации пользователя.
ms.openlocfilehash: 28c14d11218294bd8dd64f70e755cda8f8335856
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833690"
---
# <a name="getuserconfigurationresponsemessage"></a><span data-ttu-id="77fd0-103">жетусерконфигуратионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="77fd0-103">GetUserConfigurationResponseMessage</span></span>

<span data-ttu-id="77fd0-104">Элемент **жетусерконфигуратионреспонсемессаже** представляет ответ, который возвращает объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="77fd0-104">The **GetUserConfigurationResponseMessage** element represents a response that returns a user configuration object.</span></span> 
  
```xml
<GetUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <UserConfiguration/>
</GetUserConfigurationResponseMessage>
```

 <span data-ttu-id="77fd0-105">**жетусерконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="77fd0-105">**GetUserConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77fd0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77fd0-106">Attributes and elements</span></span>

<span data-ttu-id="77fd0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="77fd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77fd0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77fd0-108">Attributes</span></span>

|<span data-ttu-id="77fd0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="77fd0-109">**Attribute**</span></span>|<span data-ttu-id="77fd0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77fd0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77fd0-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="77fd0-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="77fd0-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="77fd0-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="77fd0-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="77fd0-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="77fd0-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="77fd0-114">-  Success</span></span>  <br/><span data-ttu-id="77fd0-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="77fd0-115">-  Warning</span></span>  <br/><span data-ttu-id="77fd0-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="77fd0-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="77fd0-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="77fd0-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="77fd0-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="77fd0-118">**Value**</span></span>|<span data-ttu-id="77fd0-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77fd0-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77fd0-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="77fd0-120">**Success**</span></span> <br/> |<span data-ttu-id="77fd0-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="77fd0-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="77fd0-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="77fd0-122">**Warning**</span></span> <br/> | <span data-ttu-id="77fd0-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="77fd0-123">Describes a request that was not processed.</span></span> <span data-ttu-id="77fd0-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="77fd0-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="77fd0-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="77fd0-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="77fd0-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="77fd0-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="77fd0-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="77fd0-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="77fd0-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="77fd0-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="77fd0-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="77fd0-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="77fd0-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="77fd0-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="77fd0-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="77fd0-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="77fd0-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="77fd0-132">**Error**</span></span> <br/> | <span data-ttu-id="77fd0-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="77fd0-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="77fd0-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="77fd0-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="77fd0-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="77fd0-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="77fd0-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="77fd0-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="77fd0-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="77fd0-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="77fd0-138">— Недопустимый атрибут или элемент в контексте</span><span class="sxs-lookup"><span data-stu-id="77fd0-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="77fd0-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="77fd0-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="77fd0-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="77fd0-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="77fd0-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="77fd0-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="77fd0-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77fd0-142">Child elements</span></span>

|<span data-ttu-id="77fd0-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77fd0-143">**Element**</span></span>|<span data-ttu-id="77fd0-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77fd0-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77fd0-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="77fd0-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="77fd0-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="77fd0-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="77fd0-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="77fd0-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="77fd0-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="77fd0-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="77fd0-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="77fd0-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="77fd0-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="77fd0-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="77fd0-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="77fd0-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="77fd0-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="77fd0-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="77fd0-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="77fd0-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="77fd0-154">усерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="77fd0-154">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="77fd0-155">Содержит один объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="77fd0-155">Contains a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77fd0-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77fd0-156">Parent elements</span></span>

|<span data-ttu-id="77fd0-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77fd0-157">**Element**</span></span>|<span data-ttu-id="77fd0-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77fd0-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77fd0-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="77fd0-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="77fd0-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="77fd0-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77fd0-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="77fd0-161">Text value</span></span>

<span data-ttu-id="77fd0-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="77fd0-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77fd0-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="77fd0-163">Remarks</span></span>

<span data-ttu-id="77fd0-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77fd0-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77fd0-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77fd0-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77fd0-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77fd0-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77fd0-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77fd0-167">Schema Name</span></span>  <br/> |<span data-ttu-id="77fd0-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="77fd0-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77fd0-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77fd0-169">Validation File</span></span>  <br/> |<span data-ttu-id="77fd0-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="77fd0-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77fd0-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77fd0-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="77fd0-172">False</span><span class="sxs-lookup"><span data-stu-id="77fd0-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77fd0-173">См. также</span><span class="sxs-lookup"><span data-stu-id="77fd0-173">See also</span></span>

- [<span data-ttu-id="77fd0-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="77fd0-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

