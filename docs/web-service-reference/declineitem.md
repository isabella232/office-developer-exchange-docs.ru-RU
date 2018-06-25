---
title: DeclineItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeclineItem
api_type:
- schema
ms.assetid: 2d8d2389-924e-4d03-a324-35d56cf0d6b1
description: Элемент DeclineItem представляет отклонить ответ на приглашения на собрание.
ms.openlocfilehash: d7076708248bf1ddc0472b802e4de94a436dcde8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762009"
---
# <a name="declineitem"></a><span data-ttu-id="d77c2-103">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d77c2-103">DeclineItem</span></span>

<span data-ttu-id="d77c2-104">Элемент **DeclineItem** представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="d77c2-104">The **DeclineItem** element represents a Decline reply to a meeting request.</span></span> 
  
```xml
<DeclineItem>
   <ItemClass/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <InternetMessageHeaders/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <ProposedStart/>
   <ProposedEnd/>
</DeclineItem>
```

<span data-ttu-id="d77c2-105">**DeclineItemType**</span><span class="sxs-lookup"><span data-stu-id="d77c2-105">**DeclineItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d77c2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d77c2-106">Attributes and elements</span></span>

<span data-ttu-id="d77c2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d77c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d77c2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d77c2-108">Attributes</span></span>

<span data-ttu-id="d77c2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d77c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d77c2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d77c2-110">Child elements</span></span>

|<span data-ttu-id="d77c2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d77c2-111">**Element**</span></span>|<span data-ttu-id="d77c2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d77c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d77c2-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d77c2-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="d77c2-114">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-115">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="d77c2-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="d77c2-116">Указывает уровень конфиденциальности для элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-117">Body</span><span class="sxs-lookup"><span data-stu-id="d77c2-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="d77c2-118">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="d77c2-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-119">Вложения</span><span class="sxs-lookup"><span data-stu-id="d77c2-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d77c2-120">Содержит элемент или файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d77c2-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="d77c2-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="d77c2-122">Представляет имя заголовка сообщения Интернета для заданного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="d77c2-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-123">Отправитель</span><span class="sxs-lookup"><span data-stu-id="d77c2-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="d77c2-124">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d77c2-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="d77c2-126">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="d77c2-127">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="d77c2-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="d77c2-129">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="d77c2-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d77c2-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="d77c2-131">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d77c2-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d77c2-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="d77c2-133">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="d77c2-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d77c2-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="d77c2-135">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="d77c2-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="d77c2-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="d77c2-137">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="d77c2-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-138">Получил</span><span class="sxs-lookup"><span data-stu-id="d77c2-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="d77c2-139">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d77c2-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="d77c2-140">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d77c2-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="d77c2-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="d77c2-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="d77c2-142">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d77c2-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="d77c2-143">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="d77c2-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="d77c2-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="d77c2-145">Указывает время начала предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="d77c2-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="d77c2-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="d77c2-147">Указывает время окончания предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="d77c2-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d77c2-148">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d77c2-148">Parent elements</span></span>

|<span data-ttu-id="d77c2-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d77c2-149">**Element**</span></span>|<span data-ttu-id="d77c2-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d77c2-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d77c2-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="d77c2-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="d77c2-152">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="d77c2-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/><span data-ttu-id="d77c2-153">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="d77c2-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="d77c2-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="d77c2-155">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="d77c2-155">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="d77c2-156">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d77c2-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="d77c2-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="d77c2-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="d77c2-158">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d77c2-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d77c2-159">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="d77c2-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="d77c2-160">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="d77c2-160">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d77c2-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="d77c2-161">Remarks</span></span>

<span data-ttu-id="d77c2-162">Схема, описывающая этот элемент находится в виртуальном каталоге EWS сервера Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d77c2-162">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d77c2-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d77c2-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d77c2-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d77c2-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d77c2-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d77c2-165">Schema Name</span></span>  <br/> |<span data-ttu-id="d77c2-166">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d77c2-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="d77c2-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d77c2-167">Validation File</span></span>  <br/> |<span data-ttu-id="d77c2-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d77c2-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d77c2-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d77c2-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="d77c2-170">False</span><span class="sxs-lookup"><span data-stu-id="d77c2-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d77c2-171">См. также</span><span class="sxs-lookup"><span data-stu-id="d77c2-171">See also</span></span>

- [<span data-ttu-id="d77c2-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d77c2-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

