---
title: Вложения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: Элемент вложения содержит элементы или файлы, подключенные к элементу в хранилище Exchange.
ms.openlocfilehash: 8aa5c0849122f5ca83485459fce5d0fea449c974
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761514"
---
# <a name="attachments"></a><span data-ttu-id="e252d-103">Attachments</span><span class="sxs-lookup"><span data-stu-id="e252d-103">Attachments</span></span>

<span data-ttu-id="e252d-104">Элемент **вложения** содержит элементы или файлы, подключенные к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="e252d-105">**ArrayOfAttachmentsType** и **NonEmptyArrayOfAttachmentsType**</span><span class="sxs-lookup"><span data-stu-id="e252d-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e252d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e252d-106">Attributes and elements</span></span>

<span data-ttu-id="e252d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e252d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e252d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e252d-108">Attributes</span></span>

<span data-ttu-id="e252d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e252d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e252d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e252d-110">Child elements</span></span>

|<span data-ttu-id="e252d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e252d-111">**Element**</span></span>|<span data-ttu-id="e252d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e252d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e252d-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="e252d-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="e252d-114">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="e252d-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="e252d-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="e252d-116">Представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e252d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e252d-117">Parent elements</span></span>

|<span data-ttu-id="e252d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e252d-118">**Element**</span></span>|<span data-ttu-id="e252d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e252d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e252d-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="e252d-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="e252d-121">Определяет запрос на создание вложения в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="e252d-122">Ниже приведен выражение XPath для этого элемента.`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="e252d-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="e252d-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="e252d-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="e252d-124">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="e252d-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="e252d-125">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e252d-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="e252d-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="e252d-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="e252d-127">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="e252d-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e252d-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e252d-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="e252d-129">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="e252d-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e252d-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e252d-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e252d-131">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-132">Элемент</span><span class="sxs-lookup"><span data-stu-id="e252d-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="e252d-133">Представляет универсальный элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="e252d-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e252d-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e252d-135">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-136">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e252d-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e252d-137">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e252d-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e252d-139">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e252d-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e252d-141">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-142">Message</span><span class="sxs-lookup"><span data-stu-id="e252d-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e252d-143">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e252d-144">Задача</span><span class="sxs-lookup"><span data-stu-id="e252d-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="e252d-145">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e252d-146">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="e252d-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e252d-147">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e252d-148">Контакт</span><span class="sxs-lookup"><span data-stu-id="e252d-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e252d-149">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="e252d-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e252d-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e252d-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e252d-151">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="e252d-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e252d-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e252d-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="e252d-153">Содержит состояние и результат одного запроса CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="e252d-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="e252d-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e252d-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="e252d-155">Содержит состояние и результат запроса GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="e252d-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e252d-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="e252d-156">Remarks</span></span>

<span data-ttu-id="e252d-157">Элементы **вложения** имеют те же дочерние элементы, но основаны на различных типов: **ArrayOfAttachmentsType** и **NonEmptyArrayOfAttachmentsType**.</span><span class="sxs-lookup"><span data-stu-id="e252d-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="e252d-158">Типы определить, необходима ли дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="e252d-158">The types define whether a child element is required.</span></span> <span data-ttu-id="e252d-159">**ArrayOfAttachmentsType** используется только в сообщении ответа.</span><span class="sxs-lookup"><span data-stu-id="e252d-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="e252d-160">Также важно отметить, что эти элементы выполняться в сообщения и типы пространства имен.</span><span class="sxs-lookup"><span data-stu-id="e252d-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="e252d-161">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e252d-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e252d-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e252d-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e252d-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e252d-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e252d-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e252d-164">Schema Name</span></span>  <br/> |<span data-ttu-id="e252d-165">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e252d-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="e252d-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e252d-166">Validation File</span></span>  <br/> |<span data-ttu-id="e252d-167">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e252d-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e252d-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e252d-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="e252d-169">False</span><span class="sxs-lookup"><span data-stu-id="e252d-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e252d-170">См. также</span><span class="sxs-lookup"><span data-stu-id="e252d-170">See also</span></span>

- [<span data-ttu-id="e252d-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e252d-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

