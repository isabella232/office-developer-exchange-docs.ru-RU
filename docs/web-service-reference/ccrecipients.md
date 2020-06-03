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
ms.openlocfilehash: 57d0e2d3b2c44fbd7bb30696002b27e83d1e274e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462208"
---
# <a name="ccrecipients"></a><span data-ttu-id="9b141-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="9b141-103">CcRecipients</span></span>

<span data-ttu-id="9b141-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **CcRecipients** представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="9b141-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="9b141-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="9b141-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b141-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b141-106">Attributes and elements</span></span>

<span data-ttu-id="9b141-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b141-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b141-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b141-108">Attributes</span></span>

<span data-ttu-id="9b141-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b141-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b141-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b141-110">Child elements</span></span>

|<span data-ttu-id="9b141-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b141-111">**Element**</span></span>|<span data-ttu-id="9b141-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b141-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b141-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="9b141-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9b141-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9b141-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b141-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b141-115">Parent elements</span></span>

|<span data-ttu-id="9b141-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b141-116">**Element**</span></span>|<span data-ttu-id="9b141-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b141-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b141-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9b141-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9b141-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-120">Message</span><span class="sxs-lookup"><span data-stu-id="9b141-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9b141-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9b141-122">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="9b141-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9b141-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-124">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9b141-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9b141-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-126">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="9b141-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9b141-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-128">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="9b141-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9b141-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-130">акцептитем</span><span class="sxs-lookup"><span data-stu-id="9b141-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="9b141-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="9b141-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9b141-132">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="9b141-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="9b141-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="9b141-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9b141-134">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="9b141-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="9b141-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="9b141-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9b141-136">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="9b141-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="9b141-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-138">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="9b141-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="9b141-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b141-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b141-140">форвардитем</span><span class="sxs-lookup"><span data-stu-id="9b141-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="9b141-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="9b141-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="9b141-142">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="9b141-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="9b141-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="9b141-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b141-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b141-144">Remarks</span></span>

<span data-ttu-id="9b141-p101">Не удается получить **CcRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **CcRecipients**.</span><span class="sxs-lookup"><span data-stu-id="9b141-p101">You cannot get **CcRecipients** by using a FindItem request. Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="9b141-147">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9b141-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b141-148">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b141-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b141-149">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b141-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b141-150">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b141-150">Schema Name</span></span>  <br/> |<span data-ttu-id="9b141-151">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9b141-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b141-152">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b141-152">Validation File</span></span>  <br/> |<span data-ttu-id="9b141-153">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b141-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b141-154">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b141-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b141-155">False</span><span class="sxs-lookup"><span data-stu-id="9b141-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b141-156">См. также</span><span class="sxs-lookup"><span data-stu-id="9b141-156">See also</span></span>



- [<span data-ttu-id="9b141-157">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b141-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

