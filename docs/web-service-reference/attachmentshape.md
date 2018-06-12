---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: Элемент AttachmentShape определяет дополнительные свойства, возвращаемые в ответ на запрос GetAttachment.
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761513"
---
# <a name="attachmentshape"></a><span data-ttu-id="9e9a1-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="9e9a1-103">AttachmentShape</span></span>

<span data-ttu-id="9e9a1-104">Элемент **AttachmentShape** определяет дополнительные свойства, возвращаемые в ответ на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="9e9a1-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="9e9a1-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9e9a1-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="9e9a1-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="9e9a1-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="9e9a1-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="9e9a1-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e9a1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e9a1-108">Attributes and elements</span></span>

<span data-ttu-id="9e9a1-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e9a1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e9a1-110">Attributes</span></span>

<span data-ttu-id="9e9a1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e9a1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e9a1-112">Child elements</span></span>

|<span data-ttu-id="9e9a1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e9a1-113">**Element**</span></span>|<span data-ttu-id="9e9a1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e9a1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e9a1-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="9e9a1-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="9e9a1-116">Указывает, возвращается ли содержимое Multipurpose Internet Mail Extensions (MIME) элемента или вложения в ответе.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="9e9a1-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9e9a1-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="9e9a1-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="9e9a1-119">Определяет способ форматирования основного текста в ответе.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="9e9a1-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9e9a1-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="9e9a1-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="9e9a1-122">Указывает, фильтруются ли потенциально небезопасных HTML-контент из вложения.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="9e9a1-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9e9a1-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="9e9a1-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="9e9a1-125">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="9e9a1-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e9a1-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e9a1-127">Parent elements</span></span>

|<span data-ttu-id="9e9a1-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e9a1-128">**Element**</span></span>|<span data-ttu-id="9e9a1-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e9a1-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e9a1-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9e9a1-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="9e9a1-131">Элемент, который определяет запрос на получение вложений из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="9e9a1-132">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e9a1-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9e9a1-133">Text value</span></span>

<span data-ttu-id="9e9a1-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e9a1-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="9e9a1-135">Remarks</span></span>

<span data-ttu-id="9e9a1-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e9a1-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e9a1-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e9a1-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e9a1-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e9a1-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e9a1-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e9a1-139">Schema Name</span></span>  <br/> |<span data-ttu-id="9e9a1-140">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9e9a1-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e9a1-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e9a1-141">Validation File</span></span>  <br/> |<span data-ttu-id="9e9a1-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e9a1-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e9a1-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e9a1-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e9a1-144">False</span><span class="sxs-lookup"><span data-stu-id="9e9a1-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e9a1-145">См. также</span><span class="sxs-lookup"><span data-stu-id="9e9a1-145">See also</span></span>

- [<span data-ttu-id="9e9a1-146">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9e9a1-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="9e9a1-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9e9a1-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
