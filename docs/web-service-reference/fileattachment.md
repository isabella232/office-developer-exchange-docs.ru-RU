---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: Элемент FileAttachment представляет файл, подключенный к элементу в хранилище Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762542"
---
# <a name="fileattachment"></a><span data-ttu-id="0455a-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="0455a-103">FileAttachment</span></span>

<span data-ttu-id="0455a-104">Элемент **FileAttachment** представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0455a-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 <span data-ttu-id="0455a-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="0455a-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0455a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0455a-106">Attributes and elements</span></span>

<span data-ttu-id="0455a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0455a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0455a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0455a-108">Attributes</span></span>

<span data-ttu-id="0455a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0455a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0455a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0455a-110">Child elements</span></span>

|<span data-ttu-id="0455a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0455a-111">**Element**</span></span>|<span data-ttu-id="0455a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0455a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0455a-113">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="0455a-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="0455a-114">Идентифицирует файла вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="0455a-115">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="0455a-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="0455a-116">Представляет имя вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="0455a-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="0455a-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="0455a-118">Описывает тип Multipurpose Internet Mail Extensions (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="0455a-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="0455a-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="0455a-120">Представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="0455a-121">[ContentId](contentid.md) может быть присвоено любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="0455a-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="0455a-122">Приложения могут использовать для реализации идентификации механизмы [ContentId](contentid.md) .</span><span class="sxs-lookup"><span data-stu-id="0455a-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="0455a-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="0455a-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="0455a-124">Содержит универсальный код ресурса (URI), соответствующий расположение содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="0455a-125">Размер</span><span class="sxs-lookup"><span data-stu-id="0455a-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="0455a-126">Представляет размер в байтах файла вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="0455a-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0455a-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0455a-128">Представляет после последнего изменения файла вложения.</span><span class="sxs-lookup"><span data-stu-id="0455a-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0455a-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="0455a-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="0455a-130">Представляет ли вложение встроенным в элемент.</span><span class="sxs-lookup"><span data-stu-id="0455a-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="0455a-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="0455a-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="0455a-132">Указывает, является ли вложение файла изображение контакта.</span><span class="sxs-lookup"><span data-stu-id="0455a-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="0455a-133">Контентная</span><span class="sxs-lookup"><span data-stu-id="0455a-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="0455a-134">Содержит содержимое файла вложения кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="0455a-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0455a-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0455a-135">Parent elements</span></span>

|<span data-ttu-id="0455a-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0455a-136">**Element**</span></span>|<span data-ttu-id="0455a-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0455a-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0455a-138">Вложения</span><span class="sxs-lookup"><span data-stu-id="0455a-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0455a-139">Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0455a-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0455a-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0455a-140">Text value</span></span>

<span data-ttu-id="0455a-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="0455a-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0455a-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="0455a-142">Remarks</span></span>

<span data-ttu-id="0455a-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0455a-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0455a-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0455a-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0455a-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0455a-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0455a-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0455a-146">Schema name</span></span>  <br/> |<span data-ttu-id="0455a-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0455a-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="0455a-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0455a-148">Validation file</span></span>  <br/> |<span data-ttu-id="0455a-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0455a-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0455a-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0455a-150">Can be empty</span></span>  <br/> |<span data-ttu-id="0455a-151">False</span><span class="sxs-lookup"><span data-stu-id="0455a-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0455a-152">См. также</span><span class="sxs-lookup"><span data-stu-id="0455a-152">See also</span></span>



- [<span data-ttu-id="0455a-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0455a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

