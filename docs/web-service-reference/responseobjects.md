---
title: респонсеобжектс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: Элемент Респонсеобжектс содержит коллекцию всех объектов Response, связанных с элементом в хранилище Exchange.
ms.openlocfilehash: 675bfda4addb38535736efc0c790577ff4739108
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457440"
---
# <a name="responseobjects"></a><span data-ttu-id="144b4-103">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="144b4-103">ResponseObjects</span></span>

<span data-ttu-id="144b4-104">Элемент **респонсеобжектс** содержит коллекцию всех объектов Response, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 <span data-ttu-id="144b4-105">**нонемптяррайофреспонсеобжектстипе**</span><span class="sxs-lookup"><span data-stu-id="144b4-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="144b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="144b4-106">Attributes and elements</span></span>

<span data-ttu-id="144b4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="144b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="144b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="144b4-108">Attributes</span></span>

<span data-ttu-id="144b4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="144b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="144b4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="144b4-110">Child elements</span></span>

|<span data-ttu-id="144b4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="144b4-111">**Element**</span></span>|<span data-ttu-id="144b4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="144b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="144b4-113">акцептитем</span><span class="sxs-lookup"><span data-stu-id="144b4-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="144b4-114">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="144b4-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="144b4-115">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="144b4-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="144b4-116">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="144b4-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="144b4-117">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="144b4-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="144b4-118">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="144b4-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="144b4-119">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="144b4-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="144b4-120">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-121">форвардитем</span><span class="sxs-lookup"><span data-stu-id="144b4-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="144b4-122">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="144b4-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="144b4-123">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="144b4-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="144b4-124">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-125">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="144b4-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="144b4-126">Представляет объект Response, используемый для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="144b4-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="144b4-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="144b4-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="144b4-128">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-129">постреплитем</span><span class="sxs-lookup"><span data-stu-id="144b4-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="144b4-130">Содержит ответ на элемент POST.</span><span class="sxs-lookup"><span data-stu-id="144b4-130">Contains a reply to a post item.</span></span> <span data-ttu-id="144b4-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="144b4-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="144b4-132">суппрессреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="144b4-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="144b4-133">Используется для подавления запросов уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="144b4-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="144b4-134">акцептшарингинвитатион</span><span class="sxs-lookup"><span data-stu-id="144b4-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="144b4-135">Используется для принятия приглашения, позволяющего получить доступ к данным календаря или контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="144b4-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="144b4-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="144b4-136">Parent elements</span></span>

|<span data-ttu-id="144b4-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="144b4-137">**Element**</span></span>|<span data-ttu-id="144b4-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="144b4-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="144b4-139">календаритем</span><span class="sxs-lookup"><span data-stu-id="144b4-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="144b4-140">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="144b4-141">Контакт</span><span class="sxs-lookup"><span data-stu-id="144b4-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="144b4-142">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="144b4-143">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="144b4-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="144b4-144">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="144b4-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="144b4-145">Элемент</span><span class="sxs-lookup"><span data-stu-id="144b4-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="144b4-146">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-147">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="144b4-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="144b4-148">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-149">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="144b4-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="144b4-150">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-151">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="144b4-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="144b4-152">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-153">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="144b4-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="144b4-154">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-155">Message</span><span class="sxs-lookup"><span data-stu-id="144b4-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="144b4-156">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="144b4-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="144b4-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="144b4-158">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="144b4-159">Задача</span><span class="sxs-lookup"><span data-stu-id="144b4-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="144b4-160">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="144b4-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="144b4-161">Remarks</span></span>

<span data-ttu-id="144b4-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="144b4-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="144b4-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="144b4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="144b4-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="144b4-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="144b4-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="144b4-165">Schema Name</span></span>  <br/> |<span data-ttu-id="144b4-166">Схема Types</span><span class="sxs-lookup"><span data-stu-id="144b4-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="144b4-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="144b4-167">Validation File</span></span>  <br/> |<span data-ttu-id="144b4-168">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="144b4-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="144b4-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="144b4-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="144b4-170">False</span><span class="sxs-lookup"><span data-stu-id="144b4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="144b4-171">См. также</span><span class="sxs-lookup"><span data-stu-id="144b4-171">See also</span></span>



- [<span data-ttu-id="144b4-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="144b4-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

