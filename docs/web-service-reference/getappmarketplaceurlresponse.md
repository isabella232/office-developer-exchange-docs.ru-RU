---
title: жетаппмаркетплацеурлреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: Элемент Жетаппмаркетплацеурлреспонсе указывает ответ на запрос GetAppMarketplaceUrl.
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762692"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="89a58-103">жетаппмаркетплацеурлреспонсе</span><span class="sxs-lookup"><span data-stu-id="89a58-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="89a58-104">Элемент **жетаппмаркетплацеурлреспонсе** указывает ответ на запрос **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="89a58-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="89a58-105">**жетаппмаркетплацеурлреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="89a58-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89a58-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89a58-106">Attributes and elements</span></span>

<span data-ttu-id="89a58-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="89a58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89a58-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89a58-108">Attributes</span></span>

|<span data-ttu-id="89a58-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="89a58-109">**Attribute**</span></span>|<span data-ttu-id="89a58-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89a58-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89a58-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="89a58-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="89a58-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="89a58-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="89a58-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="89a58-113">ResponseClass</span></span>

|<span data-ttu-id="89a58-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="89a58-114">**Value**</span></span>|<span data-ttu-id="89a58-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89a58-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89a58-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="89a58-116">Success</span></span>  <br/> |<span data-ttu-id="89a58-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="89a58-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="89a58-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="89a58-118">Warning</span></span>  <br/> |<span data-ttu-id="89a58-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="89a58-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="89a58-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="89a58-120">Error</span></span>  <br/> |<span data-ttu-id="89a58-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="89a58-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="89a58-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89a58-122">Child elements</span></span>

|<span data-ttu-id="89a58-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89a58-123">**Element**</span></span>|<span data-ttu-id="89a58-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89a58-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89a58-125">аппмаркетплацеурл</span><span class="sxs-lookup"><span data-stu-id="89a58-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="89a58-126">Задает URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="89a58-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="89a58-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="89a58-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="89a58-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="89a58-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="89a58-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="89a58-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="89a58-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="89a58-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="89a58-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="89a58-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="89a58-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="89a58-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="89a58-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="89a58-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="89a58-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="89a58-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89a58-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89a58-135">Parent elements</span></span>

|<span data-ttu-id="89a58-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89a58-136">**Element**</span></span>|<span data-ttu-id="89a58-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89a58-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89a58-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="89a58-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="89a58-139">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="89a58-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89a58-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="89a58-140">Remarks</span></span>

<span data-ttu-id="89a58-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89a58-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89a58-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="89a58-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89a58-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89a58-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89a58-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89a58-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89a58-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89a58-145">Schema Name</span></span>  <br/> |<span data-ttu-id="89a58-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="89a58-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="89a58-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89a58-147">Validation File</span></span>  <br/> |<span data-ttu-id="89a58-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="89a58-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89a58-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89a58-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="89a58-150">См. также</span><span class="sxs-lookup"><span data-stu-id="89a58-150">See also</span></span>



- [<span data-ttu-id="89a58-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="89a58-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

