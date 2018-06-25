---
title: Отправитель
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda
description: Элемент отправителя идентифицирует отправителя элемента.
ms.openlocfilehash: a7b06543fadd7cf7ae05f7ae8f86122138e11076
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835323"
---
# <a name="sender"></a><span data-ttu-id="2f154-103">Отправитель</span><span class="sxs-lookup"><span data-stu-id="2f154-103">Sender</span></span>

<span data-ttu-id="2f154-104">Элемент **отправителя** идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="2f154-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="2f154-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="2f154-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f154-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2f154-106">Attributes and elements</span></span>

<span data-ttu-id="2f154-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2f154-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f154-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2f154-108">Attributes</span></span>

<span data-ttu-id="2f154-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2f154-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f154-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2f154-110">Child elements</span></span>

|<span data-ttu-id="2f154-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f154-111">**Element**</span></span>|<span data-ttu-id="2f154-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f154-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f154-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="2f154-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="2f154-114">Определяет объект Active Directory включена поддержка почты, идентифицирующий отправителя.</span><span class="sxs-lookup"><span data-stu-id="2f154-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f154-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2f154-115">Parent elements</span></span>

|<span data-ttu-id="2f154-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f154-116">**Element**</span></span>|<span data-ttu-id="2f154-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f154-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f154-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2f154-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2f154-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-120">Message</span><span class="sxs-lookup"><span data-stu-id="2f154-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2f154-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2f154-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2f154-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2f154-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2f154-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2f154-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2f154-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2f154-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2f154-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2f154-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="2f154-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="2f154-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="2f154-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2f154-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="2f154-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="2f154-133">Представляет под вопросом обслуживаемых ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="2f154-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2f154-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="2f154-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="2f154-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="2f154-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2f154-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2f154-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="2f154-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="2f154-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="2f154-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f154-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="2f154-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="2f154-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="2f154-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="2f154-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="2f154-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="2f154-143">Представляет объект ответа, используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="2f154-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="2f154-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="2f154-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2f154-145">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f154-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="2f154-146">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2f154-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f154-147">Замечания</span><span class="sxs-lookup"><span data-stu-id="2f154-147">Remarks</span></span>

<span data-ttu-id="2f154-148">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2f154-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f154-149">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2f154-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f154-150">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2f154-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f154-151">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2f154-151">Schema Name</span></span>  <br/> |<span data-ttu-id="2f154-152">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2f154-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f154-153">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2f154-153">Validation File</span></span>  <br/> |<span data-ttu-id="2f154-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2f154-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f154-155">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2f154-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f154-156">False</span><span class="sxs-lookup"><span data-stu-id="2f154-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f154-157">См. также</span><span class="sxs-lookup"><span data-stu-id="2f154-157">See also</span></span>



- [<span data-ttu-id="2f154-158">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2f154-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

