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
description: Элемент ReplyTo определяет массив адресов, в который отправляются ответы.
ms.openlocfilehash: 08f9edce76fd01111922a2a07d1a63e288a0c1ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468329"
---
# <a name="replyto"></a><span data-ttu-id="6d20d-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="6d20d-103">ReplyTo</span></span>

<span data-ttu-id="6d20d-104">Элемент **ReplyTo** определяет массив адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="6d20d-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="6d20d-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="6d20d-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d20d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6d20d-106">Attributes and elements</span></span>

<span data-ttu-id="6d20d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6d20d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d20d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6d20d-108">Attributes</span></span>

<span data-ttu-id="6d20d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6d20d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d20d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6d20d-110">Child elements</span></span>

|<span data-ttu-id="6d20d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d20d-111">**Element**</span></span>|<span data-ttu-id="6d20d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d20d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d20d-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="6d20d-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="6d20d-114">Определяет объект службы каталогов Active Directory с включенной поддержкой почты, на который отправляется ответ.</span><span class="sxs-lookup"><span data-stu-id="6d20d-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d20d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6d20d-115">Parent elements</span></span>

|<span data-ttu-id="6d20d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d20d-116">**Element**</span></span>|<span data-ttu-id="6d20d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d20d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d20d-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="6d20d-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="6d20d-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-120">Message</span><span class="sxs-lookup"><span data-stu-id="6d20d-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6d20d-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-122">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="6d20d-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6d20d-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-124">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="6d20d-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6d20d-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="6d20d-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6d20d-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-128">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="6d20d-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6d20d-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-130">акцептитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="6d20d-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="6d20d-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-132">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="6d20d-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6d20d-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-134">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="6d20d-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6d20d-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-136">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="6d20d-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-138">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="6d20d-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d20d-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-140">форвардитем</span><span class="sxs-lookup"><span data-stu-id="6d20d-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="6d20d-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="6d20d-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="6d20d-142">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="6d20d-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="6d20d-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="6d20d-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d20d-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="6d20d-144">Remarks</span></span>

<span data-ttu-id="6d20d-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6d20d-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d20d-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6d20d-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d20d-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6d20d-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d20d-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6d20d-148">Schema Name</span></span>  <br/> |<span data-ttu-id="6d20d-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6d20d-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d20d-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6d20d-150">Validation File</span></span>  <br/> |<span data-ttu-id="6d20d-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6d20d-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d20d-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6d20d-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d20d-153">False</span><span class="sxs-lookup"><span data-stu-id="6d20d-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d20d-154">См. также</span><span class="sxs-lookup"><span data-stu-id="6d20d-154">See also</span></span>



- [<span data-ttu-id="6d20d-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6d20d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

