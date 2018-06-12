---
title: ReplyToItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyToItem
api_type:
- schema
ms.assetid: 35ee751a-41c0-4216-ad8b-78f7ada43a2f
description: Элемент ReplyToItem содержит ответ отправителя элемента в хранилище Exchange.
ms.openlocfilehash: 561ddc3b64ad6d2fe0ea3a3583c41faea36a4a5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835120"
---
# <a name="replytoitem"></a><span data-ttu-id="a5082-103">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="a5082-103">ReplyToItem</span></span>

<span data-ttu-id="a5082-104">Элемент **ReplyToItem** содержит ответ отправителя элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5082-104">The **ReplyToItem** element contains a reply to the sender of an item in the Exchange store.</span></span> 
  
```xml
<ReplyToItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <From/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</ReplyToItem>
```

<span data-ttu-id="a5082-105">**ReplyToItemType**</span><span class="sxs-lookup"><span data-stu-id="a5082-105">**ReplyToItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a5082-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5082-106">Attributes and elements</span></span>

<span data-ttu-id="a5082-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5082-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5082-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5082-108">Attributes</span></span>

<span data-ttu-id="a5082-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5082-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5082-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5082-110">Child elements</span></span>

|<span data-ttu-id="a5082-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5082-111">**Element**</span></span>|<span data-ttu-id="a5082-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5082-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5082-113">Subject</span><span class="sxs-lookup"><span data-stu-id="a5082-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="a5082-114">Представляет свойство subject элементов хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5082-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="a5082-115">Body</span><span class="sxs-lookup"><span data-stu-id="a5082-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="a5082-116">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="a5082-116">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="a5082-117">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="a5082-117">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="a5082-118">Содержит массив получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="a5082-118">Contains an array of recipients of an item.</span></span> <span data-ttu-id="a5082-119">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="a5082-119">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="a5082-120">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="a5082-120">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="a5082-121">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="a5082-121">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="a5082-122">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="a5082-122">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="a5082-123">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a5082-123">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a5082-124">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a5082-124">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="a5082-125">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="a5082-125">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="a5082-126">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a5082-126">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="a5082-127">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="a5082-127">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="a5082-128">From</span><span class="sxs-lookup"><span data-stu-id="a5082-128">From</span></span>](from.md) <br/> |<span data-ttu-id="a5082-129">Представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="a5082-129">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="a5082-130">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="a5082-130">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="a5082-131">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="a5082-131">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="a5082-132">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="a5082-132">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="a5082-133">Представляет новое содержимое текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="a5082-133">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="a5082-134">Получил</span><span class="sxs-lookup"><span data-stu-id="a5082-134">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="a5082-135">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="a5082-135">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="a5082-136">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a5082-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="a5082-137">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="a5082-137">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="a5082-138">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="a5082-138">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="a5082-139">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a5082-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5082-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5082-140">Parent elements</span></span>

|<span data-ttu-id="a5082-141">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5082-141">**Element**</span></span>|<span data-ttu-id="a5082-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5082-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5082-143">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="a5082-143">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="a5082-144">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="a5082-144">Describes all items that are adjacent to a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="a5082-145">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5082-145">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="a5082-146">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="a5082-146">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="a5082-147">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="a5082-147">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="a5082-148">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5082-148">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="a5082-149">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="a5082-149">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="a5082-150">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5082-150">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a5082-151">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a5082-151">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="a5082-152">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="a5082-152">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5082-153">Замечания</span><span class="sxs-lookup"><span data-stu-id="a5082-153">Remarks</span></span>

<span data-ttu-id="a5082-154">Элемент [из](from.md) необходимо задать на адрес электронной почты субъекта Если элемент ответ с делегатом.</span><span class="sxs-lookup"><span data-stu-id="a5082-154">The [From](from.md) element should be set to the e-mail address of the principal if an item is a reply by a delegate.</span></span> <span data-ttu-id="a5082-155">Если делегат не задано свойство [из](from.md) элемента будет отображаться на сообщения непосредственно из почтового ящика делегата.</span><span class="sxs-lookup"><span data-stu-id="a5082-155">If the delegate does not set the [From](from.md) property, the item will appear to have been sent directly from the delegate's mailbox.</span></span> 
  
<span data-ttu-id="a5082-156">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a5082-156">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5082-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5082-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5082-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5082-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5082-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5082-159">Schema Name</span></span>  <br/> |<span data-ttu-id="a5082-160">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a5082-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5082-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5082-161">Validation File</span></span>  <br/> |<span data-ttu-id="a5082-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a5082-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5082-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5082-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5082-164">False</span><span class="sxs-lookup"><span data-stu-id="a5082-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5082-165">См. также</span><span class="sxs-lookup"><span data-stu-id="a5082-165">See also</span></span>

- [<span data-ttu-id="a5082-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5082-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

