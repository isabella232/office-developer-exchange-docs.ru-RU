---
title: форвардитем
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardItem
api_type:
- schema
ms.assetid: 97786086-8b91-4471-8af8-d21e8d66de87
description: Элемент Форвардитем содержит элемент хранилища Exchange для пересылки получателям.
ms.openlocfilehash: dcc9a3eb2bf1cdd80680ef9142d22f5281437922
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461319"
---
# <a name="forwarditem"></a><span data-ttu-id="9b0c5-103">форвардитем</span><span class="sxs-lookup"><span data-stu-id="9b0c5-103">ForwardItem</span></span>

<span data-ttu-id="9b0c5-104">Элемент **форвардитем** содержит элемент хранилища Exchange для пересылки получателям.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-104">The **ForwardItem** element contains an Exchange store item to forward to recipients.</span></span> 
  
```xml
<ForwardItem>
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
</ForwardItem>
```

<span data-ttu-id="9b0c5-105">**форвардитемтипе**</span><span class="sxs-lookup"><span data-stu-id="9b0c5-105">**ForwardItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9b0c5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b0c5-106">Attributes and elements</span></span>

<span data-ttu-id="9b0c5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b0c5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b0c5-108">Attributes</span></span>

<span data-ttu-id="9b0c5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b0c5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b0c5-110">Child elements</span></span>

|<span data-ttu-id="9b0c5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b0c5-111">**Element**</span></span>|<span data-ttu-id="9b0c5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b0c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b0c5-113">Тема</span><span class="sxs-lookup"><span data-stu-id="9b0c5-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="9b0c5-114">Представляет свойство Subject элементов хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-115">Body</span><span class="sxs-lookup"><span data-stu-id="9b0c5-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="9b0c5-116">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-116">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-117">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="9b0c5-117">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="9b0c5-118">Содержит набор получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-118">Contains a set of recipients of an item.</span></span> <span data-ttu-id="9b0c5-119">Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-119">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-120">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="9b0c5-120">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="9b0c5-121">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-121">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-122">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="9b0c5-122">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="9b0c5-123">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-123">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-124">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="9b0c5-124">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="9b0c5-125">Указывает, запрашивает ли отправитель элемента уведомление о прочтении.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-125">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-126">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="9b0c5-126">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="9b0c5-127">Указывает, запрашивает ли отправитель элемента уведомление о доставке.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-127">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-128">From</span><span class="sxs-lookup"><span data-stu-id="9b0c5-128">From</span></span>](from.md) <br/> |<span data-ttu-id="9b0c5-129">Представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-129">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-130">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="9b0c5-130">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="9b0c5-131">Определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-131">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-132">невбодиконтент</span><span class="sxs-lookup"><span data-stu-id="9b0c5-132">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="9b0c5-133">Представляет новое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-133">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-134">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="9b0c5-134">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="9b0c5-135">Определяет делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-135">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="9b0c5-136">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9b0c5-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-137">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="9b0c5-137">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="9b0c5-138">Определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-138">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="9b0c5-139">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b0c5-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b0c5-140">Parent elements</span></span>

|<span data-ttu-id="9b0c5-141">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b0c5-141">**Element**</span></span>|<span data-ttu-id="9b0c5-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b0c5-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b0c5-143">аджацентмитингс</span><span class="sxs-lookup"><span data-stu-id="9b0c5-143">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="9b0c5-144">Описывает все элементы, смежные с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-144">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="9b0c5-145">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-145">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="9b0c5-146">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="9b0c5-146">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="9b0c5-147">Описывает все элементы, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-147">Describes all items that conflict with a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="9b0c5-148">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-148">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="9b0c5-149">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="9b0c5-149">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9b0c5-150">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-150">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b0c5-151">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="9b0c5-151">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="9b0c5-152">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9b0c5-152">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b0c5-153">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b0c5-153">Remarks</span></span>

<span data-ttu-id="9b0c5-154">Элемент [from](from.md) должен быть установлен на адрес электронной почты субъекта, если элемент пересылается представителем.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-154">The [From](from.md) element should be set to the e-mail address of the principal if an item is forwarded by a delegate.</span></span> <span data-ttu-id="9b0c5-155">Если делегат не задает свойство [from](from.md) , элемент будет отправлен непосредственно из почтового ящика представителя.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-155">If the delegate does not set the [From](from.md) property, the item will appear to have been sent directly from the delegate's mailbox.</span></span> 
  
<span data-ttu-id="9b0c5-156">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9b0c5-156">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b0c5-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b0c5-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b0c5-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b0c5-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b0c5-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b0c5-159">Schema Name</span></span>  <br/> |<span data-ttu-id="9b0c5-160">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9b0c5-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b0c5-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b0c5-161">Validation File</span></span>  <br/> |<span data-ttu-id="9b0c5-162">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b0c5-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b0c5-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b0c5-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b0c5-164">False</span><span class="sxs-lookup"><span data-stu-id="9b0c5-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b0c5-165">См. также</span><span class="sxs-lookup"><span data-stu-id="9b0c5-165">See also</span></span>

- [<span data-ttu-id="9b0c5-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b0c5-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

