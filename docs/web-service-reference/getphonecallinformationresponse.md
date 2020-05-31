---
title: жетфонекаллинформатионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformationResponse
api_type:
- schema
ms.assetid: 17f79875-46ec-4289-b974-b3c35af429cd
description: Элемент Жетфонекаллинформатионреспонсе определяет ответ на один запрос GetPhoneCallInformation.
ms.openlocfilehash: 5a03d63198cd00997b8975b18a5ae0eb5fca1af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762895"
---
# <a name="getphonecallinformationresponse"></a><span data-ttu-id="aa823-103">жетфонекаллинформатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="aa823-103">GetPhoneCallInformationResponse</span></span>

<span data-ttu-id="aa823-104">Элемент **жетфонекаллинформатионреспонсе** определяет ответ на один запрос GetPhoneCallInformation.</span><span class="sxs-lookup"><span data-stu-id="aa823-104">The **GetPhoneCallInformationResponse** element defines a response to a single GetPhoneCallInformation request.</span></span> 
  
```xml
<GetPhoneCallInformationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <PhoneCallInformation/>
</GetPhoneCallInformationResponse>
```

 <span data-ttu-id="aa823-105">**жетфонекаллинформатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="aa823-105">**GetPhoneCallInformationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa823-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa823-106">Attributes and elements</span></span>

<span data-ttu-id="aa823-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aa823-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa823-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa823-108">Attributes</span></span>

|<span data-ttu-id="aa823-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="aa823-109">**Attribute**</span></span>|<span data-ttu-id="aa823-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa823-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa823-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="aa823-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="aa823-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="aa823-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="aa823-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="aa823-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="aa823-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="aa823-114">-  Success</span></span>  <br/><span data-ttu-id="aa823-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="aa823-115">-  Warning</span></span>  <br/><span data-ttu-id="aa823-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="aa823-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="aa823-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="aa823-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="aa823-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="aa823-118">**Value**</span></span>|<span data-ttu-id="aa823-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa823-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa823-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="aa823-120">**Success**</span></span> <br/> |<span data-ttu-id="aa823-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="aa823-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="aa823-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="aa823-122">**Warning**</span></span> <br/> | <span data-ttu-id="aa823-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="aa823-123">Describes a request that was not processed.</span></span> <span data-ttu-id="aa823-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="aa823-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="aa823-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="aa823-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="aa823-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="aa823-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="aa823-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa823-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="aa823-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="aa823-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="aa823-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa823-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="aa823-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="aa823-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="aa823-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="aa823-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="aa823-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="aa823-132">**Error**</span></span> <br/> | <span data-ttu-id="aa823-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="aa823-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="aa823-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="aa823-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="aa823-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="aa823-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="aa823-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="aa823-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="aa823-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="aa823-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="aa823-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="aa823-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="aa823-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="aa823-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="aa823-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="aa823-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="aa823-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="aa823-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa823-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa823-142">Child elements</span></span>

|<span data-ttu-id="aa823-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa823-143">**Element**</span></span>|<span data-ttu-id="aa823-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa823-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa823-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="aa823-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aa823-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="aa823-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aa823-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="aa823-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aa823-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="aa823-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="aa823-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="aa823-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aa823-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="aa823-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="aa823-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="aa823-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="aa823-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="aa823-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aa823-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="aa823-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="aa823-154">фонекаллинформатион</span><span class="sxs-lookup"><span data-stu-id="aa823-154">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="aa823-155">Задает сведения о состоянии для телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="aa823-155">Specifies the state information for a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa823-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa823-156">Parent elements</span></span>

<span data-ttu-id="aa823-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa823-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aa823-158">Примечания</span><span class="sxs-lookup"><span data-stu-id="aa823-158">Remarks</span></span>

<span data-ttu-id="aa823-159">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aa823-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa823-160">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa823-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa823-161">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa823-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa823-162">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa823-162">Schema Name</span></span>  <br/> |<span data-ttu-id="aa823-163">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="aa823-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa823-164">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa823-164">Validation File</span></span>  <br/> |<span data-ttu-id="aa823-165">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aa823-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa823-166">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa823-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa823-167">False</span><span class="sxs-lookup"><span data-stu-id="aa823-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa823-168">См. также</span><span class="sxs-lookup"><span data-stu-id="aa823-168">See also</span></span>

- [<span data-ttu-id="aa823-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aa823-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

