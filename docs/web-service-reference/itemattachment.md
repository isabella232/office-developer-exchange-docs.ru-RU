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
description: Элемент ItemAttachment представляет элемент Exchange, присоединенный к другому элементу Exchange.
ms.openlocfilehash: 7bd3d22430fe04f1b28ae240102500609fe8d703
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353149"
---
# <a name="itemattachment"></a><span data-ttu-id="0c54b-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0c54b-103">ItemAttachment</span></span>

<span data-ttu-id="0c54b-104">Элемент **ItemAttachment** представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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
   <Message/>
</ItemAttachment>
```

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
   <CalendarItem/>
</ItemAttachment>
```

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
   <Contact/>
</ItemAttachment>
```

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
   <Task/>
</ItemAttachment>
```

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
   <MeetingMessage/>
</ItemAttachment>
```

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
   <MeetingRequest/>
</ItemAttachment>
```

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
   <MeetingResponse/>
</ItemAttachment>
```

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
   <MeetingCancellation/>
</ItemAttachment>
```

<span data-ttu-id="0c54b-105">**итематтачменттипе**</span><span class="sxs-lookup"><span data-stu-id="0c54b-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0c54b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c54b-106">Attributes and elements</span></span>

<span data-ttu-id="0c54b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0c54b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c54b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c54b-108">Attributes</span></span>

<span data-ttu-id="0c54b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c54b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c54b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c54b-110">Child elements</span></span>

|<span data-ttu-id="0c54b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c54b-111">**Element**</span></span>|<span data-ttu-id="0c54b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c54b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c54b-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="0c54b-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="0c54b-114">Определяет вложение.</span><span class="sxs-lookup"><span data-stu-id="0c54b-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-115">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="0c54b-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="0c54b-116">Представляет имя вложения.</span><span class="sxs-lookup"><span data-stu-id="0c54b-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="0c54b-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="0c54b-118">Описание многоцелевого расширения почты в Интернете (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0c54b-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="0c54b-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="0c54b-120">Представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0c54b-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="0c54b-121">Идентификатору [ContentId](contentid.md) можно присвоить любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="0c54b-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="0c54b-122">Приложения могут использовать идентификаторы [ContentId](contentid.md) для реализации собственных механизмов идентификации.</span><span class="sxs-lookup"><span data-stu-id="0c54b-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="0c54b-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="0c54b-124">Содержит универсальный код ресурса (URI), соответствующий расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="0c54b-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-125">Размер</span><span class="sxs-lookup"><span data-stu-id="0c54b-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="0c54b-126">Представляет размер вложенного файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="0c54b-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0c54b-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="0c54b-128">Представляет время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="0c54b-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="0c54b-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="0c54b-130">Указывает, отображается ли вложение встроенным в элементе.</span><span class="sxs-lookup"><span data-stu-id="0c54b-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-131">Элемент</span><span class="sxs-lookup"><span data-stu-id="0c54b-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="0c54b-132">Представляет вложение универсального элемента Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-133">Сообщение</span><span class="sxs-lookup"><span data-stu-id="0c54b-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0c54b-134">Представляет вложение сообщения электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-135">календаритем</span><span class="sxs-lookup"><span data-stu-id="0c54b-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0c54b-136">Представляет вложение элемента календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|<span data-ttu-id="0c54b-137">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="0c54b-137">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="0c54b-138">Представляет вложение элемента контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-139">Task</span><span class="sxs-lookup"><span data-stu-id="0c54b-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="0c54b-140">Представляет вложение задачи Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-141">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="0c54b-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0c54b-142">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-143">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0c54b-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0c54b-144">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-145">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="0c54b-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0c54b-146">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c54b-147">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="0c54b-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0c54b-148">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c54b-149">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c54b-149">Parent elements</span></span>

|<span data-ttu-id="0c54b-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c54b-150">**Element**</span></span>|<span data-ttu-id="0c54b-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c54b-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c54b-152">Вложения</span><span class="sxs-lookup"><span data-stu-id="0c54b-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0c54b-153">Содержит элементы и/или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0c54b-154">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0c54b-154">Text value</span></span>

<span data-ttu-id="0c54b-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c54b-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0c54b-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="0c54b-156">Remarks</span></span>

<span data-ttu-id="0c54b-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c54b-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c54b-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c54b-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c54b-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c54b-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c54b-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c54b-160">Schema Name</span></span>  <br/> |<span data-ttu-id="0c54b-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0c54b-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c54b-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c54b-162">Validation File</span></span>  <br/> |<span data-ttu-id="0c54b-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0c54b-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c54b-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c54b-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c54b-165">False</span><span class="sxs-lookup"><span data-stu-id="0c54b-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c54b-166">См. также</span><span class="sxs-lookup"><span data-stu-id="0c54b-166">See also</span></span>

- [<span data-ttu-id="0c54b-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0c54b-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

