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
ms.openlocfilehash: c3a07fa091c05654a03cbff58fb20204c26c9061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526440"
---
# <a name="itemattachment"></a><span data-ttu-id="e03b8-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="e03b8-103">ItemAttachment</span></span>

<span data-ttu-id="e03b8-104">Элемент **ItemAttachment** представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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

<span data-ttu-id="e03b8-105">**итематтачменттипе**</span><span class="sxs-lookup"><span data-stu-id="e03b8-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e03b8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e03b8-106">Attributes and elements</span></span>

<span data-ttu-id="e03b8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e03b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e03b8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e03b8-108">Attributes</span></span>

<span data-ttu-id="e03b8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e03b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e03b8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e03b8-110">Child elements</span></span>

|<span data-ttu-id="e03b8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e03b8-111">**Element**</span></span>|<span data-ttu-id="e03b8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e03b8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e03b8-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="e03b8-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="e03b8-114">Определяет вложение.</span><span class="sxs-lookup"><span data-stu-id="e03b8-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-115">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="e03b8-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="e03b8-116">Представляет имя вложения.</span><span class="sxs-lookup"><span data-stu-id="e03b8-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="e03b8-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="e03b8-118">Описание многоцелевого расширения почты в Интернете (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="e03b8-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="e03b8-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="e03b8-120">Представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="e03b8-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="e03b8-121">Идентификатору [ContentId](contentid.md) можно присвоить любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="e03b8-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="e03b8-122">Приложения могут использовать идентификаторы [ContentId](contentid.md) для реализации собственных механизмов идентификации.</span><span class="sxs-lookup"><span data-stu-id="e03b8-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="e03b8-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="e03b8-124">Содержит универсальный код ресурса (URI), соответствующий расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="e03b8-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-125">Размер</span><span class="sxs-lookup"><span data-stu-id="e03b8-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="e03b8-126">Представляет размер вложенного файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="e03b8-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e03b8-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="e03b8-128">Представляет время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="e03b8-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="e03b8-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="e03b8-130">Указывает, отображается ли вложение встроенным в элементе.</span><span class="sxs-lookup"><span data-stu-id="e03b8-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-131">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e03b8-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="e03b8-132">Представляет вложение универсального элемента Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-133">Сообщение</span><span class="sxs-lookup"><span data-stu-id="e03b8-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e03b8-134">Представляет вложение сообщения электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-135">календаритем</span><span class="sxs-lookup"><span data-stu-id="e03b8-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e03b8-136">Представляет вложение элемента календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|<span data-ttu-id="e03b8-137">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="e03b8-137">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="e03b8-138">Представляет вложение элемента контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-139">Task</span><span class="sxs-lookup"><span data-stu-id="e03b8-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="e03b8-140">Представляет вложение задачи Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-141">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="e03b8-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e03b8-142">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-143">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="e03b8-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e03b8-144">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-145">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="e03b8-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e03b8-146">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e03b8-147">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="e03b8-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e03b8-148">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e03b8-149">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e03b8-149">Parent elements</span></span>

|<span data-ttu-id="e03b8-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e03b8-150">**Element**</span></span>|<span data-ttu-id="e03b8-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e03b8-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e03b8-152">Вложения</span><span class="sxs-lookup"><span data-stu-id="e03b8-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e03b8-153">Содержит элементы и/или файлы, вложенные в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e03b8-154">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e03b8-154">Text value</span></span>

<span data-ttu-id="e03b8-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="e03b8-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e03b8-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="e03b8-156">Remarks</span></span>

<span data-ttu-id="e03b8-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b8-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e03b8-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e03b8-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e03b8-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e03b8-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e03b8-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e03b8-160">Schema Name</span></span>  <br/> |<span data-ttu-id="e03b8-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e03b8-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="e03b8-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e03b8-162">Validation File</span></span>  <br/> |<span data-ttu-id="e03b8-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e03b8-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e03b8-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e03b8-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="e03b8-165">False</span><span class="sxs-lookup"><span data-stu-id="e03b8-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e03b8-166">См. также</span><span class="sxs-lookup"><span data-stu-id="e03b8-166">See also</span></span>

- [<span data-ttu-id="e03b8-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e03b8-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

