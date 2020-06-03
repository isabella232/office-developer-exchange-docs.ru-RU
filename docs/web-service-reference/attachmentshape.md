---
title: аттачментшапе
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
description: Элемент Аттачментшапе определяет дополнительные свойства, возвращаемые в ответе на запрос GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529667"
---
# <a name="attachmentshape"></a><span data-ttu-id="9a4a9-103">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="9a4a9-103">AttachmentShape</span></span>

<span data-ttu-id="9a4a9-104">Элемент **аттачментшапе** определяет дополнительные свойства, возвращаемые в ответе на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4a9-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="9a4a9-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9a4a9-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="9a4a9-106">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="9a4a9-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="9a4a9-107">**аттачментреспонсешапетипе**</span><span class="sxs-lookup"><span data-stu-id="9a4a9-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a4a9-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9a4a9-108">Attributes and elements</span></span>

<span data-ttu-id="9a4a9-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a4a9-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9a4a9-110">Attributes</span></span>

<span data-ttu-id="9a4a9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a4a9-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9a4a9-112">Child elements</span></span>

|<span data-ttu-id="9a4a9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9a4a9-113">**Element**</span></span>|<span data-ttu-id="9a4a9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9a4a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a4a9-115">инклудемимеконтент</span><span class="sxs-lookup"><span data-stu-id="9a4a9-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="9a4a9-116">Указывает, возвращается ли в ответе MIME-контент элемента или вложения.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="9a4a9-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9a4a9-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="9a4a9-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="9a4a9-119">Определяет способ форматирования основного текста в отклике.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="9a4a9-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9a4a9-121">филтерхтмлконтент</span><span class="sxs-lookup"><span data-stu-id="9a4a9-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="9a4a9-122">Указывает, фильтруется ли потенциально небезопасное содержимое HTML из вложения.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="9a4a9-123">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9a4a9-124">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="9a4a9-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="9a4a9-125">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="9a4a9-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a4a9-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9a4a9-127">Parent elements</span></span>

|<span data-ttu-id="9a4a9-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9a4a9-128">**Element**</span></span>|<span data-ttu-id="9a4a9-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9a4a9-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a4a9-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9a4a9-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="9a4a9-131">Элемент, определяющий запрос на получение вложения из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="9a4a9-132">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9a4a9-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a4a9-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9a4a9-133">Text value</span></span>

<span data-ttu-id="9a4a9-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a4a9-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="9a4a9-135">Remarks</span></span>

<span data-ttu-id="9a4a9-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a4a9-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a4a9-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9a4a9-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a4a9-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9a4a9-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a4a9-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9a4a9-139">Schema Name</span></span>  <br/> |<span data-ttu-id="9a4a9-140">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9a4a9-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a4a9-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9a4a9-141">Validation File</span></span>  <br/> |<span data-ttu-id="9a4a9-142">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9a4a9-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a4a9-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9a4a9-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a4a9-144">False</span><span class="sxs-lookup"><span data-stu-id="9a4a9-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a4a9-145">См. также</span><span class="sxs-lookup"><span data-stu-id="9a4a9-145">See also</span></span>

- [<span data-ttu-id="9a4a9-146">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9a4a9-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="9a4a9-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9a4a9-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

