---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: Элемент GetAppMarketplaceUrlResponse указывает ответ на запрос GetAppMarketplaceUrl.
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762692"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="e3f98-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="e3f98-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="e3f98-104">Элемент **GetAppMarketplaceUrlResponse** указывает ответ на запрос **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="e3f98-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="e3f98-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e3f98-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3f98-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e3f98-106">Attributes and elements</span></span>

<span data-ttu-id="e3f98-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e3f98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3f98-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e3f98-108">Attributes</span></span>

|<span data-ttu-id="e3f98-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e3f98-109">**Attribute**</span></span>|<span data-ttu-id="e3f98-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f98-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3f98-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e3f98-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e3f98-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="e3f98-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e3f98-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e3f98-113">ResponseClass</span></span>

|<span data-ttu-id="e3f98-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e3f98-114">**Value**</span></span>|<span data-ttu-id="e3f98-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f98-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3f98-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e3f98-116">Success</span></span>  <br/> |<span data-ttu-id="e3f98-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e3f98-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e3f98-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="e3f98-118">Warning</span></span>  <br/> |<span data-ttu-id="e3f98-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e3f98-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e3f98-120">Error</span><span class="sxs-lookup"><span data-stu-id="e3f98-120">Error</span></span>  <br/> |<span data-ttu-id="e3f98-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e3f98-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e3f98-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e3f98-122">Child elements</span></span>

|<span data-ttu-id="e3f98-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3f98-123">**Element**</span></span>|<span data-ttu-id="e3f98-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f98-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f98-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="e3f98-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="e3f98-126">Задает URL-адрес для приложения.</span><span class="sxs-lookup"><span data-stu-id="e3f98-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="e3f98-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e3f98-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e3f98-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e3f98-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e3f98-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="e3f98-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e3f98-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e3f98-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e3f98-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e3f98-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e3f98-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e3f98-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e3f98-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e3f98-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e3f98-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="e3f98-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3f98-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e3f98-135">Parent elements</span></span>

|<span data-ttu-id="e3f98-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3f98-136">**Element**</span></span>|<span data-ttu-id="e3f98-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f98-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f98-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e3f98-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e3f98-139">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3f98-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3f98-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="e3f98-140">Remarks</span></span>

<span data-ttu-id="e3f98-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e3f98-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e3f98-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3f98-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3f98-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e3f98-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3f98-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e3f98-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3f98-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e3f98-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e3f98-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e3f98-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e3f98-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e3f98-147">Validation File</span></span>  <br/> |<span data-ttu-id="e3f98-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e3f98-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3f98-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e3f98-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e3f98-150">См. также</span><span class="sxs-lookup"><span data-stu-id="e3f98-150">See also</span></span>



- [<span data-ttu-id="e3f98-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e3f98-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

