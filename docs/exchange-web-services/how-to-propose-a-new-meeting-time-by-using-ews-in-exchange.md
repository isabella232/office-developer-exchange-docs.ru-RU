---
title: Предложение нового времени проведения собрания с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Сведения о том, как предлагать новое время проведения собрания из клиентского приложения Exchange с помощью EWS в Exchange.
ms.openlocfilehash: 4f001bb82d2325624b567412620283619b51f25b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456814"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a><span data-ttu-id="2d8bb-103">Предложение нового времени проведения собрания с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8bb-103">Propose a new meeting time by using EWS in Exchange</span></span>

<span data-ttu-id="2d8bb-104">Сведения о том, как предлагать новое время проведения собрания из клиентского приложения Exchange с помощью EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-104">Find out how to propose new meeting times from your Exchange client application by using EWS in Exchange.</span></span>
  
<span data-ttu-id="2d8bb-105">Функция "предложить новое время" позволяет участникам предлагать новое время проведения собрания организатору собрания в рамках рабочего процесса календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-105">The propose new time feature enables attendees to propose new meeting times to the meeting organizer as part of the Exchange calendar workflow.</span></span> <span data-ttu-id="2d8bb-106">Когда участник предлагает новое собрание, организатор может использовать предложенное новое время собрания для обновления собрания и отправки обновлений всем участникам.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-106">When an attendee proposes a new meeting, the organizer can use the proposed new meeting time to update the meeting and send updates to all attendees.</span></span> <span data-ttu-id="2d8bb-107">Прежде чем разрешить участникам предлагать новое время проведения собрания, необходимо определить, разрешает ли организатор новые предложения времени.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-107">Before you can enable attendees to propose new meeting times, you need to determine whether the organizer allows for new time proposals.</span></span> <span data-ttu-id="2d8bb-108">В этой статье описывается, как определить, можно ли предложить новое время и как использовать EWS для предложения нового времени.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-108">This article describes how to determine whether you can propose a new time and how to use EWS to propose a new time.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2d8bb-109">Управляемый API EWS не реализует эту функцию.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-109">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a><span data-ttu-id="2d8bb-110">Определите, можно ли предложить новое время для собрания с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-110">Determine whether you can propose a new time for a meeting by using EWS</span></span>
<span data-ttu-id="2d8bb-111"><a name="bk_Determine"> </a></span><span class="sxs-lookup"><span data-stu-id="2d8bb-111"><a name="bk_Determine"> </a></span></span>

<span data-ttu-id="2d8bb-112">Прежде чем можно будет предложить новое время собрания, необходимо найти ссылку на это собрание и определить, будет ли организатор собрания настроил собрание для поддержки новых предложений времени.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-112">Before you can propose a new time for a meeting, you need to find a reference to that meeting and determine whether the meeting organizer configured the meeting to support new time proposals.</span></span> <span data-ttu-id="2d8bb-113">Ссылку на собрание можно получить, выполнив одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-113">You can get a reference to a meeting by doing either of the following:</span></span> 
  
- <span data-ttu-id="2d8bb-114">Поиск приглашения на собрание в папке "Входящие"</span><span class="sxs-lookup"><span data-stu-id="2d8bb-114">Finding the meeting request in the Inbox</span></span>
    
- <span data-ttu-id="2d8bb-115">Поиск встречи в календаре</span><span class="sxs-lookup"><span data-stu-id="2d8bb-115">Finding the appointment in the calendar</span></span>
    
<span data-ttu-id="2d8bb-116">Чтобы найти ссылку на собрание, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-116">Use the following steps to find a meeting reference:</span></span>
  
1. <span data-ttu-id="2d8bb-117">Используйте операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (или метод [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) , управляемый API EWS), чтобы найти целевое приглашение на собрание или элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-117">Use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation (or the [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API method) to find the target meeting request or calendar item.</span></span> <span data-ttu-id="2d8bb-118">Кроме того, вы можете использовать операцию [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS, чтобы получить идентификатор целевого приглашения на собрание или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-118">Alternatively, you can use the [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS operation to get the identifier of the target meeting request or calendar item.</span></span> 
    
2. <span data-ttu-id="2d8bb-119">Выполните синтаксический анализ результатов операции **FindItem** (или метода **Folder. FindItems** ), чтобы получить идентификатор элемента собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-119">Parse the results of the **FindItem** operation (or **Folder.FindItems** method) to get the item identifier of the meeting item.</span></span> 
    
3. <span data-ttu-id="2d8bb-120">Используйте операцию [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения объектов Response для собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-120">Use the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get the response objects for the meeting.</span></span> 
    
<span data-ttu-id="2d8bb-121">В следующем XML-коде показано, что отправляется, чтобы запросить объекты ответа для элемента.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-121">The following XML shows what is sent to request the response objects on an item.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2d8bb-122">Отклик операции **GetItem** будет выглядеть аналогично следующему XML-коду, если вы запрашиваете идентификатор элемента, время начала и окончания собрания, коллекцию объектов Response и, если организатор допускает предложенные изменения времени собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-122">The **GetItem** operation response will look similar to the following XML if you request the item identifier, the meeting start and end time, the response object collection, and if the organizer allows for proposed changes to the meeting time.</span></span> <span data-ttu-id="2d8bb-123">Коллекция объектов Response, представленная элементом [респонсеобжектс](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , содержит набор ответов, допустимых для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-123">The response object collection, which is represented by the [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) element, contains the set of responses that are valid for the calendar item.</span></span> <span data-ttu-id="2d8bb-124">Элемент **пропосеневтиме** — это объект Response, указывающий на то, что пользователь может предложить новое время собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-124">The **ProposeNewTime** element is a response object that indicates that the user can propose a new time for the meeting.</span></span> <span data-ttu-id="2d8bb-125">Элементы [акцептитем](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [тентативелякцептитем](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)и [деклинеитем](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) представляют объекты ответа, которые можно использовать для предложения нового времени собрания организатору собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-125">The [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx), and [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) elements represent the response objects that you can use to propose a new meeting time to the meeting organizer.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a><span data-ttu-id="2d8bb-126">Предложение нового времени проведения собрания с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2d8bb-126">Propose a new meeting time by using EWS</span></span>
<span data-ttu-id="2d8bb-127"><a name="bk_Propose"> </a></span><span class="sxs-lookup"><span data-stu-id="2d8bb-127"><a name="bk_Propose"> </a></span></span>

<span data-ttu-id="2d8bb-128">Если вы получили объект Response **пропосеневтиме** при **использовании операции GetItem** для получения элемента календаря или приглашения на собрание, вы можете ответить на новое время собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-128">If you received a **ProposeNewTime** response object when you used the **GetItem** operation to get a calendar item or meeting request, you can respond with a proposed new meeting time.</span></span> <span data-ttu-id="2d8bb-129">Если вы не получили объект ответа **пропосеневтиме** , вы не сможете предложить новое время проведения собрания в рамках рабочего процесса календаря.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-129">If you didn't receive a **ProposeNewTime** response object, you won't be able to propose a new meeting time as part of the calendar workflow.</span></span> <span data-ttu-id="2d8bb-130">Тем не менее, вы можете ответить организатору, чтобы запросить новое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-130">You can, however, reply to the organizer to request a new meeting time.</span></span> <span data-ttu-id="2d8bb-131">Если получен объект ответа **пропосеневтиме** , вы можете ответить на собрание, обратившись к его идентификатору, и предложить новому времени проведения собрания организатору.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-131">If you receive a **ProposeNewTime** response object, you can respond to the meeting by referencing its identifier, and propose a new meeting time to the organizer.</span></span> <span data-ttu-id="2d8bb-132">В этом случае объект ответа **пропосеневтиме** отличается от типичного шаблона объекта ответа, в котором вы не отвечаете на объект отклика **пропосеневтиме** .</span><span class="sxs-lookup"><span data-stu-id="2d8bb-132">This is where the **ProposeNewTime** response object is different than the typical response object pattern in that you don't respond with a **ProposeNewTime** response object.</span></span> <span data-ttu-id="2d8bb-133">Для предложения нового собрания используется один из других объектов ответа на приглашение, например **акцептитем**, **тентативелякцептитем**или **деклинеитем**.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-133">You use one of the other meeting response objects, such as **AcceptItem**, **TentativelyAcceptItem**, or **DeclineItem**, to propose a new meeting.</span></span> <span data-ttu-id="2d8bb-134">В этом примере используется объект Response **акцептитем** .</span><span class="sxs-lookup"><span data-stu-id="2d8bb-134">This example uses the **AcceptItem** response object.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2d8bb-135">Ответ на этот запрос содержит идентификатор элемента календаря, который был добавлен в календарь участника, и копию приглашения на собрание, которое было размещено в папке "Удаленные" участника.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-135">The response to this request contains the identifier of the calendar item that was added to the attendee's calendar and a copy of the meeting request that was placed in the attendee's Deleted Items folder.</span></span> <span data-ttu-id="2d8bb-136">Ответное сообщение с новым предложением времени также было сохранено в папке "Отправленные" участника (вам потребуется найти ответное сообщение о собрании, чтобы получить его дескриптор).</span><span class="sxs-lookup"><span data-stu-id="2d8bb-136">The response message with the new time proposal was also saved in the attendee's Sent Items folder (you will need to find the meeting response message to get a handle on it).</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="2d8bb-137">Организатор получит сообщение [митингреспонсе](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) , когда участник ответит на новое время собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-137">The organizer will receive a [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) message when the attendee responds with a proposed new meeting time.</span></span> <span data-ttu-id="2d8bb-138">Сообщение **митингреспонсе** содержит предложенное новое время начала собрания и время окончания, а также идентификатор связанного элемента календаря в календаре организатора.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-138">The **MeetingResponse** message contains the proposed new meeting start time and end time, and the identifier of the associated calendar item in the organizer's calendar.</span></span> <span data-ttu-id="2d8bb-139">Организатор может использовать эти сведения для обновления существующего элемента календаря для собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-139">The organizer can use that information to update their existing calendar item for the meeting.</span></span> <span data-ttu-id="2d8bb-140">Ниже приведен рабочий процесс для ответа организатора на сообщение **митингреспонсе** , которое предлагает новое время проведения собрания:</span><span class="sxs-lookup"><span data-stu-id="2d8bb-140">The following is the workflow for the organizer to respond to a **MeetingResponse** message that proposes a new meeting time:</span></span> 
  
1. <span data-ttu-id="2d8bb-141">Определите, были ли заданы элементы **ProposedStart** или **пропоседенд** в **митингреспонсе**.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-141">Determine whether the **ProposedStart** or **ProposedEnd** elements have been set in the **MeetingResponse**.</span></span> <span data-ttu-id="2d8bb-142">Если это так, перейдите к шагу 2.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-142">If so, go to step 2.</span></span> <span data-ttu-id="2d8bb-143">В противном случае сообщение **митингреспонсе** только указывает, принял ли участник приглашение, приняли приглашение или отклонил его.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-143">If not, the **MeetingResponse** message only indicates whether the attendee has accepted, tentatively accepted, or declined the meeting.</span></span> 
    
2. <span data-ttu-id="2d8bb-144">Получение существующего элемента календаря организатора для собрания с помощью идентификатора EWS, возвращенного в элементе **ассоЦиатедкалендаритемид** .</span><span class="sxs-lookup"><span data-stu-id="2d8bb-144">Get the organizer's existing calendar item for the meeting by using the EWS identifier returned in the **AssociatedCalendarItemId** element.</span></span> 
    
3. <span data-ttu-id="2d8bb-145">Сравните начальное и конечное время с предложенным новым временем собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-145">Compare the original start and end time with the proposed new meeting time.</span></span> <span data-ttu-id="2d8bb-146">Если предложенное новое время собрания приемлемо для организатора, перейдите к шагу 4.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-146">If the proposed new meeting time is acceptable to the organizer, go to step 4.</span></span> <span data-ttu-id="2d8bb-147">В противном случае Организатор собрания может игнорировать предложенное время собрания или отправить ему сообщение электронной почты участнику, который предложил новое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-147">Otherwise, the meeting organizer can either ignore the proposed meeting time, or send an email response to the attendee that proposed the new meeting time.</span></span>
    
4. <span data-ttu-id="2d8bb-148">Необязательно Выполните вызов операции [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS, чтобы узнать, будет ли предложенное время работать для всех участников, включая почтовые ящики помещений и ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-148">(Optional) Perform a [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS operation call to find out whether the proposed time will work for all attendees, including room and resource mailboxes.</span></span> <span data-ttu-id="2d8bb-149">Для этого можно также использовать метод управляемого API [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-149">(You can also use the [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS Managed API method to do this.)</span></span> 
    
5. <span data-ttu-id="2d8bb-150">После этого организатор может обновить собрание с новым предполагаемым временем собрания и отправить обновления всем участникам с помощью операции [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (или метода [встречи. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) Managed API EWS).</span><span class="sxs-lookup"><span data-stu-id="2d8bb-150">The organizer can then update their meeting with the new proposed meeting times and send the updates to all attendees by using the [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS operation (or the [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) EWS Managed API method).</span></span> 
    
<span data-ttu-id="2d8bb-151">На следующем рисунке показан процесс, выполняемый между организатором собрания, участником и сервером Exchange, который обработал вызовы EWS.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-151">The following figure shows the process that occurs between the meeting organizer, the attendee, and the Exchange server that handled the EWS calls.</span></span>
  
<span data-ttu-id="2d8bb-152">**Рис. 1. Процесс, с помощью которого вы предлагаете новое время проведения собрания**</span><span class="sxs-lookup"><span data-stu-id="2d8bb-152">**Figure 1. Process for proposing a new meeting time**</span></span>

![На рисунке показан рабочий процесс между организатором, Exchange и участником, когда предлагается новое время собрания. если организатор разрешил предложения новых собраний, участник может предложить новое время собрания с помощью объекта ответа.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a><span data-ttu-id="2d8bb-155">Различия версий</span><span class="sxs-lookup"><span data-stu-id="2d8bb-155">Version differences</span></span>
<span data-ttu-id="2d8bb-156"><a name="bk_Behavior"> </a></span><span class="sxs-lookup"><span data-stu-id="2d8bb-156"><a name="bk_Behavior"> </a></span></span>

<span data-ttu-id="2d8bb-157">Функция "предложить новое время" была введена в версии сборки Exchange 15.00.0800.007.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-157">The propose new time feature was introduced in Exchange build version 15.00.0800.007.</span></span> <span data-ttu-id="2d8bb-158">В более ранних версиях Exchange пользователям приложения EWS необходимо отправить отдельное сообщение электронной почты организатору собрания, чтобы запросить другое время собрания.</span><span class="sxs-lookup"><span data-stu-id="2d8bb-158">In earlier versions of Exchange, EWS application users have to send a separate email to the meeting organizer to request a different meeting time.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2d8bb-159">См. также</span><span class="sxs-lookup"><span data-stu-id="2d8bb-159">See also</span></span>


- [<span data-ttu-id="2d8bb-160">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8bb-160">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="2d8bb-161">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="2d8bb-161">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="2d8bb-162">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8bb-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="2d8bb-163">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8bb-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="2d8bb-164">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d8bb-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

