---
title: ReceivedRepresenting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedRepresenting
api_type:
- schema
ms.assetid: 1157b042-6dce-4cdc-9700-e22b749da39f
description: Элемент ReceivedRepresenting определяет участника в сценарии доступа делегата.
ms.openlocfilehash: 1587fcae6975b986711e7223e50c60658833cc80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834973"
---
# <a name="receivedrepresenting"></a><span data-ttu-id="92ad4-103">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="92ad4-103">ReceivedRepresenting</span></span>

<span data-ttu-id="92ad4-104">Элемент **ReceivedRepresenting** определяет участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="92ad4-104">The **ReceivedRepresenting** element identifies the principal in a delegate access scenario.</span></span> 
  
```xml
<ReceivedRepresenting>
   <Mailbox/>
</ReceivedRepresenting>
```

 <span data-ttu-id="92ad4-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="92ad4-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92ad4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="92ad4-106">Attributes and elements</span></span>

<span data-ttu-id="92ad4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="92ad4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92ad4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="92ad4-108">Attributes</span></span>

<span data-ttu-id="92ad4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="92ad4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92ad4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="92ad4-110">Child elements</span></span>

|<span data-ttu-id="92ad4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92ad4-111">**Element**</span></span>|<span data-ttu-id="92ad4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92ad4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92ad4-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="92ad4-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="92ad4-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92ad4-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92ad4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="92ad4-115">Parent elements</span></span>

|<span data-ttu-id="92ad4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92ad4-116">**Element**</span></span>|<span data-ttu-id="92ad4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92ad4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92ad4-118">Message</span><span class="sxs-lookup"><span data-stu-id="92ad4-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="92ad4-119">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="92ad4-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="92ad4-121">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="92ad4-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="92ad4-123">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="92ad4-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="92ad4-125">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="92ad4-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="92ad4-127">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="92ad4-129">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="92ad4-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="92ad4-131">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="92ad4-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="92ad4-133">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="92ad4-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="92ad4-135">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="92ad4-137">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="92ad4-139">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="92ad4-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="92ad4-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="92ad4-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="92ad4-141">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="92ad4-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92ad4-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="92ad4-142">Remarks</span></span>

<span data-ttu-id="92ad4-143">Элемент **ReceivedRepresenting** используется вместе с **из** и **получил** элементы в Делегирование доступа сценариев.</span><span class="sxs-lookup"><span data-stu-id="92ad4-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="92ad4-144">В следующей таблице приведены объекты, которые представляют эти элементы в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="92ad4-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="92ad4-145">**Элементы в сценарии доступа делегата**</span><span class="sxs-lookup"><span data-stu-id="92ad4-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="92ad4-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92ad4-146">**Element**</span></span>|<span data-ttu-id="92ad4-147">**Объект, представляющий элемент**</span><span class="sxs-lookup"><span data-stu-id="92ad4-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92ad4-148">From</span><span class="sxs-lookup"><span data-stu-id="92ad4-148">From</span></span>](from.md) <br/> |<span data-ttu-id="92ad4-149">Сторонних</span><span class="sxs-lookup"><span data-stu-id="92ad4-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="92ad4-150">Получил</span><span class="sxs-lookup"><span data-stu-id="92ad4-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="92ad4-151">Делегат</span><span class="sxs-lookup"><span data-stu-id="92ad4-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="92ad4-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="92ad4-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="92ad4-153">Principal</span><span class="sxs-lookup"><span data-stu-id="92ad4-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="92ad4-154">В сценарии доступа делегата Если сторонних отправляет запрос на участника, имеющий делегата, делегат будет доступно нового приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="92ad4-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="92ad4-155">Эти элементы позволяют делегатов, которые будут различать сообщения, отправленные непосредственно к ним и сообщения, отправленные на них из-за переадресации правила делегата.</span><span class="sxs-lookup"><span data-stu-id="92ad4-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="92ad4-156">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ad4-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92ad4-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="92ad4-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92ad4-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="92ad4-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92ad4-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="92ad4-159">Schema Name</span></span>  <br/> |<span data-ttu-id="92ad4-160">Схема Types</span><span class="sxs-lookup"><span data-stu-id="92ad4-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="92ad4-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="92ad4-161">Validation File</span></span>  <br/> |<span data-ttu-id="92ad4-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92ad4-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92ad4-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="92ad4-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="92ad4-164">False</span><span class="sxs-lookup"><span data-stu-id="92ad4-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92ad4-165">См. также</span><span class="sxs-lookup"><span data-stu-id="92ad4-165">See also</span></span>



- [<span data-ttu-id="92ad4-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="92ad4-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

