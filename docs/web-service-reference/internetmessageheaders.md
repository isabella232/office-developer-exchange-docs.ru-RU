---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: Элемент InternetMessageHeaders содержит коллекцию заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике. Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Дополнительные сведения о веб-служб Exchange и заголовки сообщений Интернета, seeGetting Интернет сообщение headersin веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета.
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833954"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="ce0a8-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ce0a8-105">InternetMessageHeaders</span></span>

<span data-ttu-id="ce0a8-106">Элемент **InternetMessageHeaders** содержит коллекцию заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="ce0a8-107">Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="ce0a8-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="ce0a8-108">Дополнительные сведения о веб-служб Exchange и Интернет заголовки сообщений содержатся в разделе «Приступая к Интернету заголовки сообщений» в [веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce0a8-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="ce0a8-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="ce0a8-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce0a8-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ce0a8-110">Attributes and elements</span></span>

<span data-ttu-id="ce0a8-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce0a8-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ce0a8-112">Attributes</span></span>

<span data-ttu-id="ce0a8-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce0a8-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ce0a8-114">Child elements</span></span>

|<span data-ttu-id="ce0a8-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce0a8-115">**Element**</span></span>|<span data-ttu-id="ce0a8-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce0a8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce0a8-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="ce0a8-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="ce0a8-118">Представляет заголовок сообщения Интернета для заданного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce0a8-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ce0a8-119">Parent elements</span></span>

|<span data-ttu-id="ce0a8-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce0a8-120">**Element**</span></span>|<span data-ttu-id="ce0a8-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce0a8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce0a8-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="ce0a8-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="ce0a8-123">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-124">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="ce0a8-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ce0a8-125">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-126">Контакт</span><span class="sxs-lookup"><span data-stu-id="ce0a8-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ce0a8-127">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="ce0a8-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="ce0a8-129">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="ce0a8-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="ce0a8-131">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-132">Элемент</span><span class="sxs-lookup"><span data-stu-id="ce0a8-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="ce0a8-133">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ce0a8-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ce0a8-135">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ce0a8-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ce0a8-137">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ce0a8-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ce0a8-139">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ce0a8-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ce0a8-141">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-142">Message</span><span class="sxs-lookup"><span data-stu-id="ce0a8-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ce0a8-143">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="ce0a8-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="ce0a8-145">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-146">Задача</span><span class="sxs-lookup"><span data-stu-id="ce0a8-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="ce0a8-147">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0a8-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="ce0a8-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="ce0a8-149">Представляет под вопросом обслуживаемых ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce0a8-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="ce0a8-150">Remarks</span></span>

<span data-ttu-id="ce0a8-151">Ниже приведен управляемый API EWS расширенные определений для свойства **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="ce0a8-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="ce0a8-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce0a8-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce0a8-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ce0a8-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce0a8-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ce0a8-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce0a8-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ce0a8-155">Schema Name</span></span>  <br/> |<span data-ttu-id="ce0a8-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ce0a8-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce0a8-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ce0a8-157">Validation File</span></span>  <br/> |<span data-ttu-id="ce0a8-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce0a8-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce0a8-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ce0a8-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce0a8-160">False</span><span class="sxs-lookup"><span data-stu-id="ce0a8-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce0a8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="ce0a8-161">See also</span></span>



- [<span data-ttu-id="ce0a8-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce0a8-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ce0a8-163">Веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="ce0a8-163">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

