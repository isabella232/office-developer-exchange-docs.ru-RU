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
ms.openlocfilehash: 96070415c6d92a893f6c560884d9d191c7d5f15b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529506"
---
# <a name="bccrecipients"></a><span data-ttu-id="c9901-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="c9901-103">BccRecipients</span></span>

<span data-ttu-id="c9901-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **BccRecipients** представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c9901-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="c9901-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="c9901-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9901-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9901-106">Attributes and elements</span></span>

<span data-ttu-id="c9901-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c9901-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9901-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9901-108">Attributes</span></span>

<span data-ttu-id="c9901-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c9901-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9901-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9901-110">Child elements</span></span>

|<span data-ttu-id="c9901-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9901-111">**Element**</span></span>|<span data-ttu-id="c9901-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9901-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9901-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="c9901-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c9901-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9901-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9901-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9901-115">Parent elements</span></span>

|<span data-ttu-id="c9901-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9901-116">**Element**</span></span>|<span data-ttu-id="c9901-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9901-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9901-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c9901-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="c9901-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-120">Message</span><span class="sxs-lookup"><span data-stu-id="c9901-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c9901-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c9901-122">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="c9901-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c9901-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-124">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="c9901-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c9901-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="c9901-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c9901-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-128">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="c9901-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c9901-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-130">акцептитем</span><span class="sxs-lookup"><span data-stu-id="c9901-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="c9901-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="c9901-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9901-132">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="c9901-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="c9901-133">Представляет под вопросом обслуживаемых ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="c9901-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9901-134">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="c9901-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="c9901-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="c9901-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9901-136">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="c9901-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="c9901-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-138">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="c9901-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="c9901-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9901-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9901-140">форвардитем</span><span class="sxs-lookup"><span data-stu-id="c9901-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="c9901-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="c9901-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="c9901-142">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="c9901-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="c9901-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="c9901-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9901-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="c9901-144">Remarks</span></span>

<span data-ttu-id="c9901-p101">Не удается получить **BccRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **BccRecipients**.</span><span class="sxs-lookup"><span data-stu-id="c9901-p101">You cannot get **BccRecipients** by using a FindItem request. Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="c9901-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c9901-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9901-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9901-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9901-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9901-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9901-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9901-150">Schema Name</span></span>  <br/> |<span data-ttu-id="c9901-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c9901-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9901-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9901-152">Validation File</span></span>  <br/> |<span data-ttu-id="c9901-153">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9901-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9901-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9901-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9901-155">False</span><span class="sxs-lookup"><span data-stu-id="c9901-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9901-156">См. также</span><span class="sxs-lookup"><span data-stu-id="c9901-156">See also</span></span>



- [<span data-ttu-id="c9901-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9901-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

