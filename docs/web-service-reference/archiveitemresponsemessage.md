---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: Элемент ArchiveItemResponseMessage указывает сообщение ответа на запрос ArchiveItem.
ms.openlocfilehash: a7832e2cb4ec91a0871de5979fd1b418c0626aa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761492"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="06cf8-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06cf8-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="06cf8-104">Элемент **ArchiveItemResponseMessage** указывает сообщение ответа на запрос **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="06cf8-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="06cf8-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="06cf8-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06cf8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="06cf8-106">Attributes and elements</span></span>

<span data-ttu-id="06cf8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="06cf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06cf8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="06cf8-108">Attributes</span></span>

|<span data-ttu-id="06cf8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="06cf8-109">**Attribute**</span></span>|<span data-ttu-id="06cf8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06cf8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="06cf8-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="06cf8-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="06cf8-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="06cf8-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="06cf8-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="06cf8-113">ResponseClass</span></span>

|<span data-ttu-id="06cf8-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="06cf8-114">**Value**</span></span>|<span data-ttu-id="06cf8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06cf8-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="06cf8-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="06cf8-116">Success</span></span>  <br/> |<span data-ttu-id="06cf8-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="06cf8-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="06cf8-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="06cf8-118">Warning</span></span>  <br/> |<span data-ttu-id="06cf8-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="06cf8-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="06cf8-120">Error</span><span class="sxs-lookup"><span data-stu-id="06cf8-120">Error</span></span>  <br/> |<span data-ttu-id="06cf8-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="06cf8-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="06cf8-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="06cf8-122">Child elements</span></span>

|<span data-ttu-id="06cf8-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06cf8-123">**Element**</span></span>|<span data-ttu-id="06cf8-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06cf8-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06cf8-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="06cf8-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="06cf8-126">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="06cf8-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="06cf8-127">Элементы</span><span class="sxs-lookup"><span data-stu-id="06cf8-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="06cf8-128">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="06cf8-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="06cf8-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="06cf8-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="06cf8-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="06cf8-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="06cf8-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="06cf8-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="06cf8-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="06cf8-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="06cf8-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="06cf8-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="06cf8-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="06cf8-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06cf8-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="06cf8-135">Parent elements</span></span>

|<span data-ttu-id="06cf8-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06cf8-136">**Element**</span></span>|<span data-ttu-id="06cf8-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06cf8-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06cf8-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="06cf8-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="06cf8-139">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="06cf8-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="06cf8-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="06cf8-140">Remarks</span></span>

<span data-ttu-id="06cf8-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="06cf8-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="06cf8-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="06cf8-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06cf8-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="06cf8-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06cf8-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="06cf8-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06cf8-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="06cf8-145">Schema Name</span></span>  <br/> |<span data-ttu-id="06cf8-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="06cf8-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="06cf8-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="06cf8-147">Validation File</span></span>  <br/> |<span data-ttu-id="06cf8-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06cf8-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06cf8-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="06cf8-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="06cf8-150">См. также</span><span class="sxs-lookup"><span data-stu-id="06cf8-150">See also</span></span>

- [<span data-ttu-id="06cf8-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="06cf8-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

