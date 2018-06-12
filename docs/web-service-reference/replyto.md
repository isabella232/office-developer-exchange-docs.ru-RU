---
title: ReplyTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyTo
api_type:
- schema
ms.assetid: 6b6ae792-e2c4-4aa0-95cb-b49b446f1e08
description: Элемент ReplyTo определяет массив адресов, к которым будут отправляться ответы.
ms.openlocfilehash: 0ceb4f5edb75bbfe52a7a7156da3c2a328bea346
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835115"
---
# <a name="replyto"></a><span data-ttu-id="0f99b-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="0f99b-103">ReplyTo</span></span>

<span data-ttu-id="0f99b-104">Элемент **ReplyTo** определяет массив адресов, к которым будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="0f99b-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="0f99b-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="0f99b-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f99b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0f99b-106">Attributes and elements</span></span>

<span data-ttu-id="0f99b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0f99b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f99b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0f99b-108">Attributes</span></span>

<span data-ttu-id="0f99b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f99b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f99b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0f99b-110">Child elements</span></span>

|<span data-ttu-id="0f99b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f99b-111">**Element**</span></span>|<span data-ttu-id="0f99b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f99b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f99b-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="0f99b-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="0f99b-114">Идентифицирует почты Active Directory объект службы каталогов отправлен ответ.</span><span class="sxs-lookup"><span data-stu-id="0f99b-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f99b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0f99b-115">Parent elements</span></span>

|<span data-ttu-id="0f99b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f99b-116">**Element**</span></span>|<span data-ttu-id="0f99b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f99b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f99b-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0f99b-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-120">Message</span><span class="sxs-lookup"><span data-stu-id="0f99b-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0f99b-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0f99b-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0f99b-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0f99b-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0f99b-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0f99b-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0f99b-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0f99b-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0f99b-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0f99b-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="0f99b-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0f99b-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0f99b-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0f99b-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0f99b-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0f99b-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0f99b-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f99b-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0f99b-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="0f99b-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0f99b-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0f99b-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0f99b-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="0f99b-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f99b-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="0f99b-144">Remarks</span></span>

<span data-ttu-id="0f99b-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0f99b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f99b-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0f99b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f99b-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0f99b-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f99b-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0f99b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="0f99b-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0f99b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f99b-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0f99b-150">Validation File</span></span>  <br/> |<span data-ttu-id="0f99b-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f99b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f99b-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0f99b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f99b-153">False</span><span class="sxs-lookup"><span data-stu-id="0f99b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f99b-154">См. также</span><span class="sxs-lookup"><span data-stu-id="0f99b-154">See also</span></span>



- [<span data-ttu-id="0f99b-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0f99b-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

