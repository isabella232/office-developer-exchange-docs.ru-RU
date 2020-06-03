---
title: канцелкалендаритем
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
description: Элемент Канцелкалендаритем представляет объект Response, используемый для отмены собрания.
ms.openlocfilehash: 45ad76d19bd43e2081aa9b9eb63547e091014803
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462257"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="0b6e7-103">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="0b6e7-103">CancelCalendarItem</span></span>

<span data-ttu-id="0b6e7-104">Элемент **канцелкалендаритем** представляет объект Response, используемый для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
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

 <span data-ttu-id="0b6e7-105">**канцелкалендаритемтипе**</span><span class="sxs-lookup"><span data-stu-id="0b6e7-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b6e7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b6e7-106">Attributes and elements</span></span>

<span data-ttu-id="0b6e7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b6e7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b6e7-108">Attributes</span></span>

<span data-ttu-id="0b6e7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b6e7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b6e7-110">Child elements</span></span>

|<span data-ttu-id="0b6e7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b6e7-111">**Element**</span></span>|<span data-ttu-id="0b6e7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b6e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b6e7-113">Тема</span><span class="sxs-lookup"><span data-stu-id="0b6e7-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="0b6e7-114">Представляет свойство Subject элементов хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-115">Body</span><span class="sxs-lookup"><span data-stu-id="0b6e7-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="0b6e7-116">Не используется в **канцелкалендаритем**.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="0b6e7-117">Чтобы задать содержимое основного текста, используйте свойство [невбодиконтент](newbodycontent.md) .</span><span class="sxs-lookup"><span data-stu-id="0b6e7-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="0b6e7-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="0b6e7-119">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="0b6e7-120">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="0b6e7-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="0b6e7-122">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="0b6e7-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="0b6e7-124">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-125">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="0b6e7-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="0b6e7-126">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-127">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="0b6e7-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="0b6e7-128">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-129">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="0b6e7-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="0b6e7-130">Определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-131">невбодиконтент</span><span class="sxs-lookup"><span data-stu-id="0b6e7-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="0b6e7-132">Представляет новое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-133">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="0b6e7-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="0b6e7-134">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="0b6e7-135">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0b6e7-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-136">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="0b6e7-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="0b6e7-137">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="0b6e7-138">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0b6e7-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b6e7-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b6e7-139">Parent elements</span></span>

|<span data-ttu-id="0b6e7-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b6e7-140">**Element**</span></span>|<span data-ttu-id="0b6e7-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b6e7-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b6e7-142">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="0b6e7-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="0b6e7-143">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="0b6e7-144">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="0b6e7-145">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="0b6e7-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="0b6e7-146">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="0b6e7-147">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="0b6e7-148">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="0b6e7-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="0b6e7-149">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0b6e7-150">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="0b6e7-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="0b6e7-151">Содержит массив элементов для создания в папке, определенной элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="0b6e7-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b6e7-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="0b6e7-152">Remarks</span></span>

<span data-ttu-id="0b6e7-153">Элемент **канцелкалендаритем** отображается только организатором.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="0b6e7-154">Он применяется только к элементу календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="0b6e7-155">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0b6e7-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b6e7-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0b6e7-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b6e7-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0b6e7-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b6e7-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0b6e7-158">Schema Name</span></span>  <br/> |<span data-ttu-id="0b6e7-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0b6e7-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b6e7-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0b6e7-160">Validation File</span></span>  <br/> |<span data-ttu-id="0b6e7-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0b6e7-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b6e7-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0b6e7-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b6e7-163">False</span><span class="sxs-lookup"><span data-stu-id="0b6e7-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b6e7-164">См. также</span><span class="sxs-lookup"><span data-stu-id="0b6e7-164">See also</span></span>

- [<span data-ttu-id="0b6e7-165">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0b6e7-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

