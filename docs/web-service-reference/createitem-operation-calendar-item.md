---
title: Операции CreateItem (элемента календаря)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: aa4a7c94-f668-4bd2-8079-c855f6ab17e1
description: Операции CreateItem создает элементы календаря в хранилище Exchange.
ms.openlocfilehash: c2174dd806b922e640ef7afcab32b98c67c65b41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761891"
---
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="d9cde-103">Операции CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="d9cde-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="d9cde-104">Операции CreateItem создает элементы календаря в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9cde-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9cde-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="d9cde-105">Remarks</span></span>

<span data-ttu-id="d9cde-106">Операции CreateItem создает встреч, собраний и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="d9cde-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="d9cde-107">Если элемент календаря создается без участников, он считается встречи.</span><span class="sxs-lookup"><span data-stu-id="d9cde-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="d9cde-108">Если участники заданы, элемента календаря — это собрание.</span><span class="sxs-lookup"><span data-stu-id="d9cde-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="d9cde-109">При создании собрания с помощью операции CreateItem, приглашений на собрания автоматически отправляются определенного участников Если атрибут SendMeetingInvitations имеет значение для отправки приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="d9cde-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="d9cde-110">Пример запроса CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="d9cde-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="d9cde-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9cde-111">Description</span></span>

<span data-ttu-id="d9cde-112">Запрос CreateItem в следующем примере показано, как создать собрание две обязательных участников.</span><span class="sxs-lookup"><span data-stu-id="d9cde-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="d9cde-113">Этот запрос будет отправлять запросы собрания двух участников.</span><span class="sxs-lookup"><span data-stu-id="d9cde-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="d9cde-114">Программа</span><span class="sxs-lookup"><span data-stu-id="d9cde-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Planning Meeting</Subject>
          <Body BodyType="Text">Plan the agenda for next week's meeting.</Body>
          <ReminderIsSet>true</ReminderIsSet>
          <ReminderMinutesBeforeStart>60</ReminderMinutesBeforeStart>
          <Start>2006-11-02T14:00:00</Start>
          <End>2006-11-02T15:00:00</End>
          <IsAllDayEvent>false</IsAllDayEvent>
          <LegacyFreeBusyStatus>Busy</LegacyFreeBusyStatus>
          <Location>Conference Room 721</Location>
          <RequiredAttendees>
            <Attendee>
              <Mailbox>
                <EmailAddress>User1@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
            <Attendee>
              <Mailbox>
                <EmailAddress>User2@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
          </RequiredAttendees>
        </t:CalendarItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d9cde-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="d9cde-115">Comments</span></span>

<span data-ttu-id="d9cde-116">Пример того, как ответ на приглашения на собрание приведены в разделе [операции CreateItem (запрос на собрание)](createitem-operation-meeting-request.md) .</span><span class="sxs-lookup"><span data-stu-id="d9cde-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="d9cde-117">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="d9cde-117">Request elements</span></span>

<span data-ttu-id="d9cde-118">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d9cde-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d9cde-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="d9cde-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="d9cde-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="d9cde-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="d9cde-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d9cde-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="d9cde-122">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="d9cde-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="d9cde-123">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="d9cde-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="d9cde-124">Subject</span><span class="sxs-lookup"><span data-stu-id="d9cde-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="d9cde-125">Body</span><span class="sxs-lookup"><span data-stu-id="d9cde-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="d9cde-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="d9cde-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="d9cde-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="d9cde-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="d9cde-128">Start</span><span class="sxs-lookup"><span data-stu-id="d9cde-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="d9cde-129">End</span><span class="sxs-lookup"><span data-stu-id="d9cde-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d9cde-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="d9cde-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="d9cde-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d9cde-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="d9cde-132">Location</span><span class="sxs-lookup"><span data-stu-id="d9cde-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="d9cde-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="d9cde-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="d9cde-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="d9cde-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="d9cde-135">Mailbox</span><span class="sxs-lookup"><span data-stu-id="d9cde-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="d9cde-136">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d9cde-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="d9cde-137">Ответ успешные CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="d9cde-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="d9cde-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d9cde-138">Description</span></span>

<span data-ttu-id="d9cde-139">В следующем примере показано успешного ответа на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="d9cde-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d9cde-140">Программа</span><span class="sxs-lookup"><span data-stu-id="d9cde-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAAlAFV" ChangeKey="DwAAABYA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d9cde-141">Комментарии</span><span class="sxs-lookup"><span data-stu-id="d9cde-141">Comments</span></span>

<span data-ttu-id="d9cde-142">Атрибуты **Id** и **ChangeKey** [ItemId](itemid.md) элемента URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="d9cde-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="d9cde-143">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="d9cde-143">Successful response elements</span></span>

<span data-ttu-id="d9cde-144">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d9cde-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d9cde-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d9cde-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d9cde-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="d9cde-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="d9cde-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d9cde-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d9cde-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d9cde-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="d9cde-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d9cde-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d9cde-150">Элементы</span><span class="sxs-lookup"><span data-stu-id="d9cde-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="d9cde-151">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="d9cde-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="d9cde-152">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="d9cde-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="d9cde-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d9cde-153">See also</span></span>



[<span data-ttu-id="d9cde-154">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d9cde-154">CreateItem operation</span></span>](createitem-operation.md)

