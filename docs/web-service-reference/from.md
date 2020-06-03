---
title: From
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: Элемент From представляет адрес, с которого было отправлено сообщение.
ms.openlocfilehash: c0d655731677e56cc02c7c029264ffc96f0a18c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459555"
---
# <a name="from"></a><span data-ttu-id="46f61-103">From</span><span class="sxs-lookup"><span data-stu-id="46f61-103">From</span></span>

<span data-ttu-id="46f61-104">Элемент **from** представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="46f61-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="46f61-105">**синглереЦипиенттипе**</span><span class="sxs-lookup"><span data-stu-id="46f61-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46f61-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46f61-106">Attributes and elements</span></span>

<span data-ttu-id="46f61-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="46f61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46f61-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46f61-108">Attributes</span></span>

<span data-ttu-id="46f61-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46f61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46f61-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46f61-110">Child elements</span></span>

|<span data-ttu-id="46f61-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46f61-111">**Element**</span></span>|<span data-ttu-id="46f61-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46f61-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46f61-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="46f61-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="46f61-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="46f61-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46f61-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46f61-115">Parent elements</span></span>

|<span data-ttu-id="46f61-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46f61-116">**Element**</span></span>|<span data-ttu-id="46f61-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46f61-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46f61-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="46f61-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="46f61-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-120">Message</span><span class="sxs-lookup"><span data-stu-id="46f61-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="46f61-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="46f61-122">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="46f61-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="46f61-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-124">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="46f61-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="46f61-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="46f61-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="46f61-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-128">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="46f61-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="46f61-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-130">акцептитем</span><span class="sxs-lookup"><span data-stu-id="46f61-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="46f61-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="46f61-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="46f61-132">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="46f61-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="46f61-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="46f61-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="46f61-134">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="46f61-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="46f61-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="46f61-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="46f61-136">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="46f61-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="46f61-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-138">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="46f61-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="46f61-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="46f61-140">форвардитем</span><span class="sxs-lookup"><span data-stu-id="46f61-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="46f61-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="46f61-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="46f61-142">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="46f61-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="46f61-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="46f61-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="46f61-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="46f61-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="46f61-145">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46f61-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="46f61-146">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="46f61-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46f61-147">Примечания</span><span class="sxs-lookup"><span data-stu-id="46f61-147">Remarks</span></span>

<span data-ttu-id="46f61-148">Этот элемент используется для сообщений электронной почты "Отправить от имени".</span><span class="sxs-lookup"><span data-stu-id="46f61-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="46f61-149">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46f61-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46f61-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46f61-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46f61-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46f61-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46f61-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46f61-152">Schema Name</span></span>  <br/> |<span data-ttu-id="46f61-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46f61-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="46f61-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46f61-154">Validation File</span></span>  <br/> |<span data-ttu-id="46f61-155">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="46f61-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46f61-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46f61-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="46f61-157">False</span><span class="sxs-lookup"><span data-stu-id="46f61-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46f61-158">См. также</span><span class="sxs-lookup"><span data-stu-id="46f61-158">See also</span></span>



- [<span data-ttu-id="46f61-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46f61-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

