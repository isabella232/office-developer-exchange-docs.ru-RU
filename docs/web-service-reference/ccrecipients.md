---
title: CcRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CcRecipients
api_type:
- schema
ms.assetid: 5c20ec3a-0bee-4e67-b220-586ed0d601c9
description: Элемент CcRecipients представляет коллекцию получателей, которые будут получать копии сообщения.
ms.openlocfilehash: 0afe19cfae49dbf48c685296a83ab1330b631d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761672"
---
# <a name="ccrecipients"></a><span data-ttu-id="aa51a-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="aa51a-103">CcRecipients</span></span>

<span data-ttu-id="aa51a-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **CcRecipients** представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="aa51a-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="aa51a-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="aa51a-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa51a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa51a-106">Attributes and elements</span></span>

<span data-ttu-id="aa51a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aa51a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa51a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa51a-108">Attributes</span></span>

<span data-ttu-id="aa51a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa51a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa51a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa51a-110">Child elements</span></span>

|<span data-ttu-id="aa51a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa51a-111">**Element**</span></span>|<span data-ttu-id="aa51a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa51a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa51a-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="aa51a-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="aa51a-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa51a-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa51a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa51a-115">Parent elements</span></span>

|<span data-ttu-id="aa51a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa51a-116">**Element**</span></span>|<span data-ttu-id="aa51a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa51a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa51a-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="aa51a-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-120">Message</span><span class="sxs-lookup"><span data-stu-id="aa51a-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aa51a-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="aa51a-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="aa51a-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="aa51a-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="aa51a-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="aa51a-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="aa51a-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="aa51a-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="aa51a-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="aa51a-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="aa51a-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="aa51a-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="aa51a-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="aa51a-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="aa51a-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="aa51a-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="aa51a-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa51a-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="aa51a-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="aa51a-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="aa51a-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="aa51a-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="aa51a-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="aa51a-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa51a-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="aa51a-144">Remarks</span></span>

<span data-ttu-id="aa51a-p101">Не удается получить **CcRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **CcRecipients**.</span><span class="sxs-lookup"><span data-stu-id="aa51a-p101">You cannot get **CcRecipients** by using a FindItem request. Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="aa51a-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aa51a-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa51a-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa51a-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa51a-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa51a-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa51a-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa51a-150">Schema Name</span></span>  <br/> |<span data-ttu-id="aa51a-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aa51a-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa51a-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa51a-152">Validation File</span></span>  <br/> |<span data-ttu-id="aa51a-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa51a-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa51a-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa51a-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa51a-155">False</span><span class="sxs-lookup"><span data-stu-id="aa51a-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa51a-156">См. также</span><span class="sxs-lookup"><span data-stu-id="aa51a-156">See also</span></span>



- [<span data-ttu-id="aa51a-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aa51a-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

