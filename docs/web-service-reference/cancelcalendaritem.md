---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: Элемент CancelCalendarItem представляет объект ответа, которая используется для отмены собрания.
ms.openlocfilehash: 262f60db33abac36156b069dc85e1fccb3522d5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761664"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="d7003-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="d7003-103">CancelCalendarItem</span></span>

<span data-ttu-id="d7003-104">Элемент **CancelCalendarItem** представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="d7003-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 <span data-ttu-id="d7003-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="d7003-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7003-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7003-106">Attributes and elements</span></span>

<span data-ttu-id="d7003-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d7003-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7003-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d7003-108">Attributes</span></span>

<span data-ttu-id="d7003-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d7003-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7003-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d7003-110">Child elements</span></span>

|<span data-ttu-id="d7003-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7003-111">**Element**</span></span>|<span data-ttu-id="d7003-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7003-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7003-113">Subject</span><span class="sxs-lookup"><span data-stu-id="d7003-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="d7003-114">Представляет свойство subject элементов хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7003-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="d7003-115">Body</span><span class="sxs-lookup"><span data-stu-id="d7003-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="d7003-116">Не используется с **CancelCalendarItem**.</span><span class="sxs-lookup"><span data-stu-id="d7003-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="d7003-117">Свойство [NewBodyContent](newbodycontent.md) используется для установки содержимое текста запроса.</span><span class="sxs-lookup"><span data-stu-id="d7003-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="d7003-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d7003-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="d7003-119">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="d7003-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="d7003-120">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="d7003-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="d7003-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="d7003-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="d7003-122">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="d7003-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="d7003-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d7003-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="d7003-124">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d7003-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="d7003-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d7003-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="d7003-126">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="d7003-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="d7003-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d7003-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="d7003-128">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="d7003-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="d7003-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="d7003-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="d7003-130">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="d7003-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="d7003-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="d7003-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="d7003-132">Представляет новое содержимое текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="d7003-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="d7003-133">Получил</span><span class="sxs-lookup"><span data-stu-id="d7003-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="d7003-134">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d7003-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="d7003-135">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d7003-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="d7003-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="d7003-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="d7003-137">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d7003-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="d7003-138">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d7003-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7003-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d7003-139">Parent elements</span></span>

|<span data-ttu-id="d7003-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7003-140">**Element**</span></span>|<span data-ttu-id="d7003-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7003-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7003-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="d7003-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="d7003-143">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="d7003-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="d7003-144">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d7003-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="d7003-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="d7003-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="d7003-146">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="d7003-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="d7003-147">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d7003-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="d7003-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="d7003-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="d7003-149">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7003-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d7003-150">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="d7003-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="d7003-151">Содержит массив элементов для создания в папку, указанную в элементе [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="d7003-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7003-152">Замечания</span><span class="sxs-lookup"><span data-stu-id="d7003-152">Remarks</span></span>

<span data-ttu-id="d7003-153">Элемент **CancelCalendarItem** только просматривать организатором.</span><span class="sxs-lookup"><span data-stu-id="d7003-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="d7003-154">Применяется только для организатора элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d7003-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="d7003-155">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d7003-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7003-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d7003-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7003-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d7003-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7003-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d7003-158">Schema Name</span></span>  <br/> |<span data-ttu-id="d7003-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d7003-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7003-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d7003-160">Validation File</span></span>  <br/> |<span data-ttu-id="d7003-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d7003-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7003-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d7003-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7003-163">False</span><span class="sxs-lookup"><span data-stu-id="d7003-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7003-164">См. также</span><span class="sxs-lookup"><span data-stu-id="d7003-164">See also</span></span>

- [<span data-ttu-id="d7003-165">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d7003-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

