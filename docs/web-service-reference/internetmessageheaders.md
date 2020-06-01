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
description: Элемент InternetMessageHeaders содержит коллекцию некоторых заголовков Интернет-сообщений, содержащихся в элементе почтового ящика. Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Для получения дополнительных сведений о службах EWS и заголовках сообщений Интернета Сижеттинг заголовки сообщений Интернета EWS, MIME и отсутствующие заголовки сообщений Интернета.
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467328"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="920e8-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="920e8-105">InternetMessageHeaders</span></span>

<span data-ttu-id="920e8-106">Элемент **InternetMessageHeaders** содержит коллекцию некоторых заголовков Интернет-сообщений, содержащихся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="920e8-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="920e8-107">Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="920e8-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="920e8-108">Дополнительные сведения о службах EWS и заголовках сообщений в Интернете можно найти в статье "сведения о заголовках сообщений Интернета" в [EWS, MIME и отсутствующих заголовках сообщений Интернета](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="920e8-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="920e8-109">**нонемптяррайофинтернесеадерстипе**</span><span class="sxs-lookup"><span data-stu-id="920e8-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="920e8-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="920e8-110">Attributes and elements</span></span>

<span data-ttu-id="920e8-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="920e8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="920e8-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="920e8-112">Attributes</span></span>

<span data-ttu-id="920e8-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="920e8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="920e8-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="920e8-114">Child elements</span></span>

|<span data-ttu-id="920e8-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="920e8-115">**Element**</span></span>|<span data-ttu-id="920e8-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="920e8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="920e8-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="920e8-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="920e8-118">Представляет заголовок Интернет-сообщения для определенного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="920e8-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="920e8-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="920e8-119">Parent elements</span></span>

|<span data-ttu-id="920e8-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="920e8-120">**Element**</span></span>|<span data-ttu-id="920e8-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="920e8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="920e8-122">акцептитем</span><span class="sxs-lookup"><span data-stu-id="920e8-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="920e8-123">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="920e8-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="920e8-124">календаритем</span><span class="sxs-lookup"><span data-stu-id="920e8-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="920e8-125">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="920e8-126">Контакт</span><span class="sxs-lookup"><span data-stu-id="920e8-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="920e8-127">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="920e8-128">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="920e8-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="920e8-129">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="920e8-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="920e8-130">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="920e8-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="920e8-131">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="920e8-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="920e8-132">Элемент</span><span class="sxs-lookup"><span data-stu-id="920e8-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="920e8-133">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-134">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="920e8-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="920e8-135">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-136">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="920e8-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="920e8-137">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-138">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="920e8-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="920e8-139">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-140">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="920e8-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="920e8-141">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-142">Message</span><span class="sxs-lookup"><span data-stu-id="920e8-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="920e8-143">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="920e8-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="920e8-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="920e8-145">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-146">Задача</span><span class="sxs-lookup"><span data-stu-id="920e8-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="920e8-147">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="920e8-148">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="920e8-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="920e8-149">Представляет под вопросом обслуживаемых ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="920e8-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="920e8-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="920e8-150">Remarks</span></span>

<span data-ttu-id="920e8-151">Ниже приведено определение расширенного свойства управляемого API EWS для свойства **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="920e8-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="920e8-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="920e8-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="920e8-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="920e8-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="920e8-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="920e8-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="920e8-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="920e8-155">Schema Name</span></span>  <br/> |<span data-ttu-id="920e8-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="920e8-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="920e8-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="920e8-157">Validation File</span></span>  <br/> |<span data-ttu-id="920e8-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="920e8-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="920e8-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="920e8-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="920e8-160">False</span><span class="sxs-lookup"><span data-stu-id="920e8-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="920e8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="920e8-161">See also</span></span>



- [<span data-ttu-id="920e8-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="920e8-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="920e8-163">EWS, MIME и отсутствующие заголовки сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="920e8-163">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

