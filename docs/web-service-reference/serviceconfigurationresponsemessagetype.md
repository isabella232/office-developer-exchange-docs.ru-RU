---
title: сервицеконфигуратионреспонсемессажетипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: Элемент Сервицеконфигуратионреспонсемессажетипе содержит параметры конфигурации службы.
ms.openlocfilehash: 4c84a49b2403343a1defd00696858489497d6214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44439107"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="841b4-103">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="841b4-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="841b4-104">Элемент **сервицеконфигуратионреспонсемессажетипе** содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="841b4-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="841b4-105">**сервицеконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="841b4-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="841b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="841b4-106">Attributes and elements</span></span>

<span data-ttu-id="841b4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="841b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="841b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="841b4-108">Attributes</span></span>

|<span data-ttu-id="841b4-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="841b4-109">**Attribute**</span></span>|<span data-ttu-id="841b4-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="841b4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="841b4-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="841b4-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="841b4-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="841b4-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="841b4-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="841b4-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="841b4-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="841b4-114">-  Success</span></span>  <br/><span data-ttu-id="841b4-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="841b4-115">-  Warning</span></span>  <br/><span data-ttu-id="841b4-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="841b4-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="841b4-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="841b4-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="841b4-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="841b4-118">**Value**</span></span>|<span data-ttu-id="841b4-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="841b4-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="841b4-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="841b4-120">**Success**</span></span> <br/> |<span data-ttu-id="841b4-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="841b4-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="841b4-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="841b4-122">**Warning**</span></span> <br/> | <span data-ttu-id="841b4-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="841b4-123">Describes a request that was not processed.</span></span> <span data-ttu-id="841b4-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="841b4-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="841b4-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="841b4-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="841b4-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="841b4-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="841b4-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="841b4-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="841b4-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="841b4-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="841b4-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="841b4-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="841b4-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="841b4-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="841b4-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="841b4-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="841b4-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="841b4-132">**Error**</span></span> <br/> | <span data-ttu-id="841b4-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="841b4-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="841b4-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="841b4-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="841b4-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="841b4-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="841b4-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="841b4-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="841b4-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="841b4-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="841b4-138">— Недопустимый атрибут или элемент в контексте</span><span class="sxs-lookup"><span data-stu-id="841b4-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="841b4-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="841b4-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="841b4-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="841b4-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="841b4-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="841b4-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="841b4-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="841b4-142">Child elements</span></span>

|<span data-ttu-id="841b4-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="841b4-143">**Element**</span></span>|<span data-ttu-id="841b4-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="841b4-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="841b4-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="841b4-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="841b4-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="841b4-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="841b4-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="841b4-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="841b4-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="841b4-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="841b4-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="841b4-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="841b4-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="841b4-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="841b4-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="841b4-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="841b4-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="841b4-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="841b4-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="841b4-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="841b4-154">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="841b4-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="841b4-155">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="841b4-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="841b4-156">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="841b4-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="841b4-157">Содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="841b4-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="841b4-158">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="841b4-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="841b4-159">Содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="841b4-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="841b4-160">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="841b4-160">Parent elements</span></span>

|<span data-ttu-id="841b4-161">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="841b4-161">**Element**</span></span>|<span data-ttu-id="841b4-162">**Описание**</span><span class="sxs-lookup"><span data-stu-id="841b4-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="841b4-163">Респонсемессажес (Аррайофсервицеконфигуратионреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="841b4-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="841b4-164">Содержит массив ответных сообщений конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="841b4-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="841b4-165">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="841b4-165">Text value</span></span>

<span data-ttu-id="841b4-166">Нет.</span><span class="sxs-lookup"><span data-stu-id="841b4-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="841b4-167">Примечания</span><span class="sxs-lookup"><span data-stu-id="841b4-167">Remarks</span></span>

<span data-ttu-id="841b4-168">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="841b4-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="841b4-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="841b4-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="841b4-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="841b4-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="841b4-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="841b4-171">Schema Name</span></span>  <br/> |<span data-ttu-id="841b4-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="841b4-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="841b4-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="841b4-173">Validation File</span></span>  <br/> |<span data-ttu-id="841b4-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="841b4-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="841b4-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="841b4-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="841b4-176">False</span><span class="sxs-lookup"><span data-stu-id="841b4-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="841b4-177">См. также</span><span class="sxs-lookup"><span data-stu-id="841b4-177">See also</span></span>

- [<span data-ttu-id="841b4-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="841b4-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

