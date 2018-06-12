---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: Элемент ItemAttachment представляет собой элемент Exchange, подключенный к другой элемент Exchange.
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834137"
---
# <a name="itemattachment"></a><span data-ttu-id="abeea-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="abeea-103">ItemAttachment</span></span>

<span data-ttu-id="abeea-104">Элемент **ItemAttachment** представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

 <span data-ttu-id="abeea-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="abeea-105">**ItemAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abeea-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="abeea-106">Attributes and elements</span></span>

<span data-ttu-id="abeea-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="abeea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abeea-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="abeea-108">Attributes</span></span>

<span data-ttu-id="abeea-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="abeea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abeea-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="abeea-110">Child elements</span></span>

|<span data-ttu-id="abeea-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abeea-111">**Element**</span></span>|<span data-ttu-id="abeea-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abeea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abeea-113">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="abeea-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="abeea-114">Идентифицирует вложение.</span><span class="sxs-lookup"><span data-stu-id="abeea-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-115">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="abeea-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="abeea-116">Представляет имя вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="abeea-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="abeea-118">Описывает тип Multipurpose Internet Mail Extensions (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="abeea-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="abeea-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="abeea-120">Представляет идентификатор содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="abeea-121">[ContentId](contentid.md) может быть присвоено любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="abeea-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="abeea-122">Приложения могут использовать для реализации идентификации механизмы [ContentId](contentid.md) .</span><span class="sxs-lookup"><span data-stu-id="abeea-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="abeea-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="abeea-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="abeea-124">Содержит универсальный код ресурса (URI), соответствующий расположение содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-125">Размер</span><span class="sxs-lookup"><span data-stu-id="abeea-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="abeea-126">Представляет размер в байтах файла вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="abeea-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="abeea-128">Представляет после последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="abeea-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="abeea-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="abeea-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="abeea-130">Представляет ли вложение встроенным в элемент.</span><span class="sxs-lookup"><span data-stu-id="abeea-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="abeea-131">Элемент</span><span class="sxs-lookup"><span data-stu-id="abeea-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="abeea-132">Представляет универсальный вложение элемента Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-133">Message</span><span class="sxs-lookup"><span data-stu-id="abeea-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="abeea-134">Представляет вложения сообщения электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-135">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="abeea-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="abeea-136">Представляет вложение элемента календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-137">Контакт</span><span class="sxs-lookup"><span data-stu-id="abeea-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="abeea-138">Представляет вложение элемента контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-139">Задача</span><span class="sxs-lookup"><span data-stu-id="abeea-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="abeea-140">Представляет вложение задач Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="abeea-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="abeea-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="abeea-142">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abeea-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="abeea-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="abeea-144">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abeea-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="abeea-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="abeea-146">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="abeea-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="abeea-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="abeea-148">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abeea-149">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="abeea-149">Parent elements</span></span>

|<span data-ttu-id="abeea-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abeea-150">**Element**</span></span>|<span data-ttu-id="abeea-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abeea-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abeea-152">Вложения</span><span class="sxs-lookup"><span data-stu-id="abeea-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="abeea-153">Содержит элементы и/или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="abeea-154">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="abeea-154">Text value</span></span>

<span data-ttu-id="abeea-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="abeea-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="abeea-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="abeea-156">Remarks</span></span>

<span data-ttu-id="abeea-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="abeea-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abeea-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="abeea-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abeea-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="abeea-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abeea-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="abeea-160">Schema Name</span></span>  <br/> |<span data-ttu-id="abeea-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="abeea-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="abeea-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="abeea-162">Validation File</span></span>  <br/> |<span data-ttu-id="abeea-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abeea-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abeea-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="abeea-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="abeea-165">False</span><span class="sxs-lookup"><span data-stu-id="abeea-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abeea-166">См. также</span><span class="sxs-lookup"><span data-stu-id="abeea-166">See also</span></span>



- [<span data-ttu-id="abeea-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="abeea-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

