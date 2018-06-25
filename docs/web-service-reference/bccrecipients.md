---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: Элемент BccRecipients представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.
ms.openlocfilehash: 858fe74c32cb7d1ed624888c06bba4ffe09d489e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761553"
---
# <a name="bccrecipients"></a><span data-ttu-id="fde2d-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="fde2d-103">BccRecipients</span></span>

<span data-ttu-id="fde2d-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **BccRecipients** представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fde2d-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="fde2d-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="fde2d-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fde2d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fde2d-106">Attributes and elements</span></span>

<span data-ttu-id="fde2d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fde2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fde2d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fde2d-108">Attributes</span></span>

<span data-ttu-id="fde2d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fde2d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fde2d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fde2d-110">Child elements</span></span>

|<span data-ttu-id="fde2d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fde2d-111">**Element**</span></span>|<span data-ttu-id="fde2d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fde2d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fde2d-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="fde2d-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="fde2d-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fde2d-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fde2d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fde2d-115">Parent elements</span></span>

|<span data-ttu-id="fde2d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fde2d-116">**Element**</span></span>|<span data-ttu-id="fde2d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fde2d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fde2d-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="fde2d-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-120">Message</span><span class="sxs-lookup"><span data-stu-id="fde2d-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fde2d-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="fde2d-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="fde2d-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="fde2d-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="fde2d-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="fde2d-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="fde2d-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="fde2d-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="fde2d-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="fde2d-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="fde2d-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="fde2d-133">Представляет под вопросом обслуживаемых ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="fde2d-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="fde2d-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="fde2d-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="fde2d-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="fde2d-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde2d-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="fde2d-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="fde2d-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="fde2d-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="fde2d-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="fde2d-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="fde2d-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fde2d-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="fde2d-144">Remarks</span></span>

<span data-ttu-id="fde2d-p101">Не удается получить **BccRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **BccRecipients**.</span><span class="sxs-lookup"><span data-stu-id="fde2d-p101">You cannot get **BccRecipients** by using a FindItem request. Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="fde2d-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fde2d-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fde2d-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fde2d-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fde2d-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fde2d-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fde2d-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fde2d-150">Schema Name</span></span>  <br/> |<span data-ttu-id="fde2d-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fde2d-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="fde2d-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fde2d-152">Validation File</span></span>  <br/> |<span data-ttu-id="fde2d-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fde2d-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fde2d-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fde2d-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="fde2d-155">False</span><span class="sxs-lookup"><span data-stu-id="fde2d-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fde2d-156">См. также</span><span class="sxs-lookup"><span data-stu-id="fde2d-156">See also</span></span>



- [<span data-ttu-id="fde2d-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fde2d-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

