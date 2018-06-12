---
title: TentativelyAcceptItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TentativelyAcceptItem
api_type:
- schema
ms.assetid: ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0
description: Представляет элемент TentativelyAcceptItem, под вопросом ответ на приглашения на собрание.
ms.openlocfilehash: 203028aae2ec972e36209b2a97420e83d61ddd81
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840159"
---
# <a name="tentativelyacceptitem"></a><span data-ttu-id="15c74-103">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="15c74-103">TentativelyAcceptItem</span></span>

<span data-ttu-id="15c74-104">Представляет элемент **TentativelyAcceptItem** , под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="15c74-104">The **TentativelyAcceptItem** element represents a Tentative reply to a meeting request.</span></span> 
  
```xml
<TentativelyAcceptItem>
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
</TentativelyAcceptItem>
```

 <span data-ttu-id="15c74-105">**TentativelyAcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="15c74-105">**TentativelyAcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15c74-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15c74-106">Attributes and elements</span></span>

<span data-ttu-id="15c74-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="15c74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15c74-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15c74-108">Attributes</span></span>

<span data-ttu-id="15c74-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="15c74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15c74-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15c74-110">Child elements</span></span>

|<span data-ttu-id="15c74-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15c74-111">**Element**</span></span>|<span data-ttu-id="15c74-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15c74-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15c74-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="15c74-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="15c74-114">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="15c74-115">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="15c74-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="15c74-116">Определяет уровень конфиденциальности сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-116">Identifies the sensitivity of an item.</span></span>  <br/> |
|[<span data-ttu-id="15c74-117">Body</span><span class="sxs-lookup"><span data-stu-id="15c74-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="15c74-118">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="15c74-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="15c74-119">Вложения</span><span class="sxs-lookup"><span data-stu-id="15c74-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="15c74-120">Содержит элемент или файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15c74-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="15c74-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="15c74-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="15c74-122">Представляет имя заголовка сообщения Интернета для заданного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="15c74-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="15c74-123">Отправитель</span><span class="sxs-lookup"><span data-stu-id="15c74-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="15c74-124">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="15c74-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="15c74-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="15c74-126">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="15c74-127">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="15c74-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="15c74-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="15c74-129">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="15c74-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="15c74-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="15c74-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="15c74-131">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="15c74-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="15c74-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="15c74-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="15c74-133">Указывает, будет ли отправителя элемента о прочтении.</span><span class="sxs-lookup"><span data-stu-id="15c74-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="15c74-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="15c74-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="15c74-135">Указывает, требует ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="15c74-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="15c74-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="15c74-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="15c74-137">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="15c74-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="15c74-138">Получил</span><span class="sxs-lookup"><span data-stu-id="15c74-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="15c74-139">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="15c74-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="15c74-140">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="15c74-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="15c74-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="15c74-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="15c74-142">Идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="15c74-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="15c74-143">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="15c74-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="15c74-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="15c74-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="15c74-145">Указывает время начала предложенного приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="15c74-145">Specifies the proposed start time of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="15c74-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="15c74-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="15c74-147">Указывает время окончания предложенного приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="15c74-147">Specifies the proposed end time of the meeting request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15c74-148">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15c74-148">Parent elements</span></span>

|<span data-ttu-id="15c74-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15c74-149">**Element**</span></span>|<span data-ttu-id="15c74-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15c74-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15c74-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="15c74-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="15c74-152">Описание всех элементов, расположенных во время собрания.</span><span class="sxs-lookup"><span data-stu-id="15c74-152">Describes all items that are adjacent to a meeting time.</span></span>  <br/> <br/> <span data-ttu-id="15c74-153">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-153">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="15c74-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="15c74-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="15c74-155">Описание всех элементов, конфликтующие с время собрания.</span><span class="sxs-lookup"><span data-stu-id="15c74-155">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="15c74-156">Ниже приведены некоторые из выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="15c74-156">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="15c74-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="15c74-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="15c74-158">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15c74-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="15c74-159">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="15c74-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="15c74-160">Содержит массив элементов для создания в папку, указанную в элементе [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="15c74-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15c74-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="15c74-161">Remarks</span></span>

<span data-ttu-id="15c74-162">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="15c74-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15c74-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15c74-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15c74-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15c74-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15c74-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15c74-165">Schema Name</span></span>  <br/> |<span data-ttu-id="15c74-166">Схема Types</span><span class="sxs-lookup"><span data-stu-id="15c74-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="15c74-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15c74-167">Validation File</span></span>  <br/> |<span data-ttu-id="15c74-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15c74-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15c74-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15c74-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="15c74-170">False</span><span class="sxs-lookup"><span data-stu-id="15c74-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15c74-171">См. также</span><span class="sxs-lookup"><span data-stu-id="15c74-171">See also</span></span>

- [<span data-ttu-id="15c74-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="15c74-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

