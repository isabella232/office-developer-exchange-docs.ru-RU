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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468329"
---
# <a name="replyto"></a><span data-ttu-id="4f924-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="4f924-103">ReplyTo</span></span>

<span data-ttu-id="4f924-104">Элемент **ReplyTo** определяет массив адресов, в который отправляются ответы.</span><span class="sxs-lookup"><span data-stu-id="4f924-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="4f924-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="4f924-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f924-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f924-106">Attributes and elements</span></span>

<span data-ttu-id="4f924-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f924-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f924-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f924-108">Attributes</span></span>

<span data-ttu-id="4f924-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f924-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f924-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f924-110">Child elements</span></span>

|<span data-ttu-id="4f924-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f924-111">**Element**</span></span>|<span data-ttu-id="4f924-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f924-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f924-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4f924-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="4f924-114">Определяет объект службы каталогов Active Directory с включенной поддержкой почты, на который отправляется ответ.</span><span class="sxs-lookup"><span data-stu-id="4f924-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f924-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f924-115">Parent elements</span></span>

|<span data-ttu-id="4f924-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f924-116">**Element**</span></span>|<span data-ttu-id="4f924-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f924-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f924-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="4f924-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="4f924-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-120">Message</span><span class="sxs-lookup"><span data-stu-id="4f924-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4f924-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="4f924-122">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="4f924-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="4f924-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-124">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="4f924-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4f924-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="4f924-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4f924-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-128">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="4f924-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4f924-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-130">акцептитем</span><span class="sxs-lookup"><span data-stu-id="4f924-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="4f924-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="4f924-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4f924-132">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="4f924-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="4f924-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="4f924-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4f924-134">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="4f924-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="4f924-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="4f924-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4f924-136">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="4f924-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="4f924-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-138">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="4f924-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="4f924-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f924-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4f924-140">форвардитем</span><span class="sxs-lookup"><span data-stu-id="4f924-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="4f924-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="4f924-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="4f924-142">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="4f924-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="4f924-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="4f924-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f924-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f924-144">Remarks</span></span>

<span data-ttu-id="4f924-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4f924-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f924-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f924-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f924-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f924-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f924-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f924-148">Schema Name</span></span>  <br/> |<span data-ttu-id="4f924-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4f924-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f924-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f924-150">Validation File</span></span>  <br/> |<span data-ttu-id="4f924-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4f924-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f924-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f924-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f924-153">False</span><span class="sxs-lookup"><span data-stu-id="4f924-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f924-154">См. также</span><span class="sxs-lookup"><span data-stu-id="4f924-154">See also</span></span>



- [<span data-ttu-id="4f924-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f924-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

