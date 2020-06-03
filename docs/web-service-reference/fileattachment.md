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
description: Элемент FileAttachment представляет файл, присоединенный к элементу в хранилище Exchange.
ms.openlocfilehash: db9b541fb2527ae3c09cbdb33bedea7fb215bd30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461018"
---
# <a name="fileattachment"></a><span data-ttu-id="93f6f-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="93f6f-103">FileAttachment</span></span>

<span data-ttu-id="93f6f-104">Элемент **FileAttachment** представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93f6f-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="93f6f-105">**филеаттачменттипе**</span><span class="sxs-lookup"><span data-stu-id="93f6f-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93f6f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93f6f-106">Attributes and elements</span></span>

<span data-ttu-id="93f6f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93f6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93f6f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93f6f-108">Attributes</span></span>

<span data-ttu-id="93f6f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93f6f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93f6f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93f6f-110">Child elements</span></span>

|<span data-ttu-id="93f6f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93f6f-111">**Element**</span></span>|<span data-ttu-id="93f6f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93f6f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93f6f-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="93f6f-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="93f6f-114">Определяет вложенный файл.</span><span class="sxs-lookup"><span data-stu-id="93f6f-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-115">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="93f6f-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="93f6f-116">Представляет имя вложения.</span><span class="sxs-lookup"><span data-stu-id="93f6f-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="93f6f-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="93f6f-118">Описание многоцелевого расширения почты в Интернете (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="93f6f-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="93f6f-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="93f6f-120">Представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="93f6f-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="93f6f-121">Идентификатору [ContentId](contentid.md) можно присвоить любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="93f6f-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="93f6f-122">Приложения могут использовать идентификаторы [ContentId](contentid.md) для реализации собственных механизмов идентификации.</span><span class="sxs-lookup"><span data-stu-id="93f6f-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="93f6f-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="93f6f-124">Содержит универсальный код ресурса (URI), соответствующий расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="93f6f-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-125">Размер</span><span class="sxs-lookup"><span data-stu-id="93f6f-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="93f6f-126">Представляет размер вложенного файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="93f6f-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="93f6f-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="93f6f-128">Представляет время последнего изменения вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="93f6f-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="93f6f-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="93f6f-130">Указывает, отображается ли вложение встроенным в элементе.</span><span class="sxs-lookup"><span data-stu-id="93f6f-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-131">исконтактфото</span><span class="sxs-lookup"><span data-stu-id="93f6f-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="93f6f-132">Указывает, является ли вложение изображением контакта.</span><span class="sxs-lookup"><span data-stu-id="93f6f-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="93f6f-133">Content</span><span class="sxs-lookup"><span data-stu-id="93f6f-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="93f6f-134">Содержит содержимое вложенного файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="93f6f-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93f6f-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93f6f-135">Parent elements</span></span>

|<span data-ttu-id="93f6f-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93f6f-136">**Element**</span></span>|<span data-ttu-id="93f6f-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93f6f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93f6f-138">Вложения</span><span class="sxs-lookup"><span data-stu-id="93f6f-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="93f6f-139">Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93f6f-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93f6f-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="93f6f-140">Text value</span></span>

<span data-ttu-id="93f6f-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="93f6f-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93f6f-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="93f6f-142">Remarks</span></span>

<span data-ttu-id="93f6f-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93f6f-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93f6f-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93f6f-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93f6f-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93f6f-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93f6f-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93f6f-146">Schema name</span></span>  <br/> |<span data-ttu-id="93f6f-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="93f6f-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="93f6f-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93f6f-148">Validation file</span></span>  <br/> |<span data-ttu-id="93f6f-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93f6f-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93f6f-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93f6f-150">Can be empty</span></span>  <br/> |<span data-ttu-id="93f6f-151">False</span><span class="sxs-lookup"><span data-stu-id="93f6f-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93f6f-152">См. также</span><span class="sxs-lookup"><span data-stu-id="93f6f-152">See also</span></span>



- [<span data-ttu-id="93f6f-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="93f6f-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

