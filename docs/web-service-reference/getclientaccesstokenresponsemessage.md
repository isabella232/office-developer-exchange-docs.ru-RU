---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: Элемент GetClientAccessTokenResponseMessage указывает сообщение ответа на запрос GetClientAccessToken.
ms.openlocfilehash: 16fe684dd48f77156ed88d02a6ae7b8f3312cd87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762714"
---
# <a name="getclientaccesstokenresponsemessage"></a><span data-ttu-id="fb3d0-103">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fb3d0-103">GetClientAccessTokenResponseMessage</span></span>

<span data-ttu-id="fb3d0-104">Элемент **GetClientAccessTokenResponseMessage** указывает сообщение ответа на запрос **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="fb3d0-104">The **GetClientAccessTokenResponseMessage** element specifies the response message for a **GetClientAccessToken** request.</span></span> 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 <span data-ttu-id="fb3d0-105">**GetClientAccessTokenResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-105">**GetClientAccessTokenResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb3d0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fb3d0-106">Attributes and elements</span></span>

<span data-ttu-id="fb3d0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb3d0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fb3d0-108">Attributes</span></span>

|<span data-ttu-id="fb3d0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-109">**Attribute**</span></span>|<span data-ttu-id="fb3d0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb3d0-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fb3d0-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="fb3d0-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="fb3d0-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fb3d0-113">ResponseClass</span></span>

|<span data-ttu-id="fb3d0-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-114">**Value**</span></span>|<span data-ttu-id="fb3d0-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb3d0-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="fb3d0-116">Success</span></span>  <br/> |<span data-ttu-id="fb3d0-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="fb3d0-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="fb3d0-118">Warning</span></span>  <br/> |<span data-ttu-id="fb3d0-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="fb3d0-120">Error</span><span class="sxs-lookup"><span data-stu-id="fb3d0-120">Error</span></span>  <br/> |<span data-ttu-id="fb3d0-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fb3d0-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fb3d0-122">Child elements</span></span>

|<span data-ttu-id="fb3d0-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-123">**Element**</span></span>|<span data-ttu-id="fb3d0-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3d0-125">Маркер (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="fb3d0-125">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md) <br/> |<span data-ttu-id="fb3d0-126">Задает маркер доступа клиентов.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-126">Specifies a client access token.</span></span>  <br/> |
|[<span data-ttu-id="fb3d0-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fb3d0-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fb3d0-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="fb3d0-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="fb3d0-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fb3d0-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fb3d0-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fb3d0-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fb3d0-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fb3d0-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fb3d0-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fb3d0-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb3d0-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fb3d0-135">Parent elements</span></span>

|<span data-ttu-id="fb3d0-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-136">**Element**</span></span>|<span data-ttu-id="fb3d0-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3d0-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3d0-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fb3d0-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fb3d0-139">Содержит сообщения ответа на запрос веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="fb3d0-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb3d0-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="fb3d0-140">Remarks</span></span>

<span data-ttu-id="fb3d0-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fb3d0-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb3d0-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb3d0-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fb3d0-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb3d0-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fb3d0-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb3d0-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fb3d0-145">Schema Name</span></span>  <br/> |<span data-ttu-id="fb3d0-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="fb3d0-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="fb3d0-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fb3d0-147">Validation File</span></span>  <br/> |<span data-ttu-id="fb3d0-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fb3d0-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb3d0-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fb3d0-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fb3d0-150">См. также</span><span class="sxs-lookup"><span data-stu-id="fb3d0-150">See also</span></span>



- [<span data-ttu-id="fb3d0-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fb3d0-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

