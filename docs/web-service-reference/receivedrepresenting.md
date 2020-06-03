---
title: рецеиведрепресентинг
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
description: Элемент Рецеиведрепресентинг идентифицирует участника в сценарии доступа делегата.
ms.openlocfilehash: f444fb88be9c0df174f0c1490cf7c499cc0c0539
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468224"
---
# <a name="receivedrepresenting"></a><span data-ttu-id="285ed-103">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="285ed-103">ReceivedRepresenting</span></span>

<span data-ttu-id="285ed-104">Элемент **рецеиведрепресентинг** идентифицирует участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="285ed-104">The **ReceivedRepresenting** element identifies the principal in a delegate access scenario.</span></span> 
  
```xml
<ReceivedRepresenting>
   <Mailbox/>
</ReceivedRepresenting>
```

 <span data-ttu-id="285ed-105">**синглереЦипиенттипе**</span><span class="sxs-lookup"><span data-stu-id="285ed-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="285ed-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="285ed-106">Attributes and elements</span></span>

<span data-ttu-id="285ed-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="285ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="285ed-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="285ed-108">Attributes</span></span>

<span data-ttu-id="285ed-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="285ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="285ed-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="285ed-110">Child elements</span></span>

|<span data-ttu-id="285ed-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="285ed-111">**Element**</span></span>|<span data-ttu-id="285ed-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="285ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="285ed-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="285ed-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="285ed-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="285ed-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="285ed-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="285ed-115">Parent elements</span></span>

|<span data-ttu-id="285ed-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="285ed-116">**Element**</span></span>|<span data-ttu-id="285ed-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="285ed-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="285ed-118">Message</span><span class="sxs-lookup"><span data-stu-id="285ed-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="285ed-119">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="285ed-120">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="285ed-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="285ed-121">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-122">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="285ed-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="285ed-123">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-124">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="285ed-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="285ed-125">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-126">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="285ed-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="285ed-127">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-128">акцептитем</span><span class="sxs-lookup"><span data-stu-id="285ed-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="285ed-129">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="285ed-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="285ed-130">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="285ed-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="285ed-131">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="285ed-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="285ed-132">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="285ed-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="285ed-133">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="285ed-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="285ed-134">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="285ed-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="285ed-135">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-136">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="285ed-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="285ed-137">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="285ed-138">форвардитем</span><span class="sxs-lookup"><span data-stu-id="285ed-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="285ed-139">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="285ed-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="285ed-140">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="285ed-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="285ed-141">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="285ed-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="285ed-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="285ed-142">Remarks</span></span>

<span data-ttu-id="285ed-143">Элемент **рецеиведрепресентинг** используется вместе с элементами **from** и **рецеиведби** в сценариях доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="285ed-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="285ed-144">В следующей таблице перечислены сущности, которые представляют эти элементы в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="285ed-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="285ed-145">**Элементы в сценарии доступа делегата**</span><span class="sxs-lookup"><span data-stu-id="285ed-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="285ed-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="285ed-146">**Element**</span></span>|<span data-ttu-id="285ed-147">**Объект, который представляет элемент**</span><span class="sxs-lookup"><span data-stu-id="285ed-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="285ed-148">From</span><span class="sxs-lookup"><span data-stu-id="285ed-148">From</span></span>](from.md) <br/> |<span data-ttu-id="285ed-149">ThirdParty</span><span class="sxs-lookup"><span data-stu-id="285ed-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="285ed-150">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="285ed-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="285ed-151">Делегат</span><span class="sxs-lookup"><span data-stu-id="285ed-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="285ed-152">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="285ed-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="285ed-153">Principal</span><span class="sxs-lookup"><span data-stu-id="285ed-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="285ed-154">Если в сценарии доступа делегата ThirdParty отправляет приглашение на собрание участнику с представителем, он увидит новое приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="285ed-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="285ed-155">Эти элементы позволяют представителям различать сообщения, отправленные непосредственно им, и сообщения, отправленные им из-за правила пересылки делегата.</span><span class="sxs-lookup"><span data-stu-id="285ed-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="285ed-156">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="285ed-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="285ed-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="285ed-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="285ed-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="285ed-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="285ed-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="285ed-159">Schema Name</span></span>  <br/> |<span data-ttu-id="285ed-160">Схема Types</span><span class="sxs-lookup"><span data-stu-id="285ed-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="285ed-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="285ed-161">Validation File</span></span>  <br/> |<span data-ttu-id="285ed-162">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="285ed-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="285ed-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="285ed-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="285ed-164">False</span><span class="sxs-lookup"><span data-stu-id="285ed-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="285ed-165">См. также</span><span class="sxs-lookup"><span data-stu-id="285ed-165">See also</span></span>



- [<span data-ttu-id="285ed-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="285ed-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

