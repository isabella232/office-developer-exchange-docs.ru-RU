---
title: тентативелякцептитем
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
description: Элемент Тентативелякцептитем представляет предварительный ответ на приглашение на собрание.
ms.openlocfilehash: 6d20ec2964c41dcbb786b1209b4597999e025609
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459499"
---
# <a name="tentativelyacceptitem"></a><span data-ttu-id="6336e-103">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="6336e-103">TentativelyAcceptItem</span></span>

<span data-ttu-id="6336e-104">Элемент **тентативелякцептитем** представляет предварительный ответ на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="6336e-104">The **TentativelyAcceptItem** element represents a Tentative reply to a meeting request.</span></span> 
  
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

 <span data-ttu-id="6336e-105">**тентативелякцептитемтипе**</span><span class="sxs-lookup"><span data-stu-id="6336e-105">**TentativelyAcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6336e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6336e-106">Attributes and elements</span></span>

<span data-ttu-id="6336e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6336e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6336e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6336e-108">Attributes</span></span>

<span data-ttu-id="6336e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6336e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6336e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6336e-110">Child elements</span></span>

|<span data-ttu-id="6336e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6336e-111">**Element**</span></span>|<span data-ttu-id="6336e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6336e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6336e-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6336e-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6336e-114">Представляет класс сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6336e-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6336e-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6336e-116">Определяет чувствительность элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-116">Identifies the sensitivity of an item.</span></span>  <br/> |
|[<span data-ttu-id="6336e-117">Body</span><span class="sxs-lookup"><span data-stu-id="6336e-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="6336e-118">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6336e-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6336e-119">Вложения</span><span class="sxs-lookup"><span data-stu-id="6336e-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6336e-120">Содержит элемент или файл, прикрепленный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6336e-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6336e-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6336e-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6336e-122">Представляет имя заголовка Интернет-сообщения для данного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="6336e-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="6336e-123">Sender</span><span class="sxs-lookup"><span data-stu-id="6336e-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="6336e-124">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="6336e-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6336e-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6336e-126">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="6336e-127">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="6336e-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6336e-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6336e-129">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="6336e-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6336e-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6336e-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6336e-131">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6336e-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="6336e-132">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="6336e-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6336e-133">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="6336e-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6336e-134">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="6336e-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6336e-135">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="6336e-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6336e-136">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="6336e-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="6336e-137">Определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="6336e-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="6336e-138">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="6336e-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6336e-139">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="6336e-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="6336e-140">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6336e-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6336e-141">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="6336e-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6336e-142">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="6336e-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="6336e-143">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6336e-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6336e-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="6336e-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="6336e-145">Указывает предполагаемое время начала приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6336e-145">Specifies the proposed start time of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6336e-146">пропоседенд</span><span class="sxs-lookup"><span data-stu-id="6336e-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="6336e-147">Указывает предполагаемое время окончания приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6336e-147">Specifies the proposed end time of the meeting request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6336e-148">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6336e-148">Parent elements</span></span>

|<span data-ttu-id="6336e-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6336e-149">**Element**</span></span>|<span data-ttu-id="6336e-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6336e-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6336e-151">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="6336e-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="6336e-152">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6336e-152">Describes all items that are adjacent to a meeting time.</span></span>  <br/> <br/> <span data-ttu-id="6336e-153">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-153">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="6336e-154">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="6336e-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="6336e-155">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="6336e-155">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="6336e-156">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="6336e-156">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="6336e-157">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="6336e-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6336e-158">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6336e-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6336e-159">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="6336e-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6336e-160">Содержит массив элементов для создания в папке, определенной элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6336e-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6336e-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="6336e-161">Remarks</span></span>

<span data-ttu-id="6336e-162">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6336e-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6336e-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6336e-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6336e-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6336e-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6336e-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6336e-165">Schema Name</span></span>  <br/> |<span data-ttu-id="6336e-166">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6336e-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="6336e-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6336e-167">Validation File</span></span>  <br/> |<span data-ttu-id="6336e-168">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6336e-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6336e-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6336e-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="6336e-170">False</span><span class="sxs-lookup"><span data-stu-id="6336e-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6336e-171">См. также</span><span class="sxs-lookup"><span data-stu-id="6336e-171">See also</span></span>

- [<span data-ttu-id="6336e-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6336e-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

