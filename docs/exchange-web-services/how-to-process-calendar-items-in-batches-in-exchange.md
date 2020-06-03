---
title: Обработка элементов календаря в пакетах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fb2952e2-cbfe-43ac-b746-f071faa7665c
description: Узнайте, как создавать, получать, обновлять и удалять пакеты элементов календаря в едином вызове с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 10c5c28e4dda27c9ac9770088db122f0a8e8c101
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527903"
---
# <a name="process-calendar-items-in-batches-in-exchange"></a><span data-ttu-id="2cbb9-103">Обработка элементов календаря в пакетах Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-103">Process calendar items in batches in Exchange</span></span>

<span data-ttu-id="2cbb9-104">Узнайте, как создавать, получать, обновлять и удалять пакеты элементов календаря в едином вызове с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-104">Learn how to create, get, update, or delete batches of calendar items in a single call by using the EWS Managed API or EWS in Exchange.</span></span>

<span data-ttu-id="2cbb9-105">Вы можете использовать управляемый API EWS или EWS для работы с пакетами встреч и собраний, чтобы уменьшить количество звонков клиента на сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-105">You can use the EWS Managed API or EWS to work with batches of appointments and meetings to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="2cbb9-106">При использовании управляемого API EWS для создания, получения, обновления и удаления пакета элементов календаря используются методы объекта [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а при работе с одними элементами календаря используются методы объекта [встреча](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2cbb9-106">When you use the EWS Managed API to create, get, update, and delete a batch of calendar items, you use [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single calendar items, you use [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="2cbb9-107">Если вы используете EWS, вы используете одну и ту же операцию для пакетных вызовов, которые используются для отдельных вызовов.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-107">If you are using EWS, you use the same operation for batch calls that you use for single calls.</span></span>

<span data-ttu-id="2cbb9-108">**Таблица 1. Методы управляемого API EWS и операции EWS для работы с пакетами элементов календаря**</span><span class="sxs-lookup"><span data-stu-id="2cbb9-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of calendar items**</span></span>

|<span data-ttu-id="2cbb9-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="2cbb9-109">**In order to…**</span></span>|<span data-ttu-id="2cbb9-110">**Используйте этот метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="2cbb9-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="2cbb9-111">**Используйте эту операцию EWS**</span><span class="sxs-lookup"><span data-stu-id="2cbb9-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2cbb9-112">Создание элементов календаря в пакетах</span><span class="sxs-lookup"><span data-stu-id="2cbb9-112">Create calendar items in batches</span></span>  <br/> |[<span data-ttu-id="2cbb9-113">CreateItems</span><span class="sxs-lookup"><span data-stu-id="2cbb9-113">CreateItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2cbb9-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="2cbb9-114">CreateItem</span></span>](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2cbb9-115">Получение элементов календаря в пакетном режиме</span><span class="sxs-lookup"><span data-stu-id="2cbb9-115">Get calendar items in batches</span></span>  <br/> |[<span data-ttu-id="2cbb9-116">биндтоитемс</span><span class="sxs-lookup"><span data-stu-id="2cbb9-116">BindToItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2cbb9-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="2cbb9-117">GetItem</span></span>](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2cbb9-118">Обновление элементов календаря в пакетах</span><span class="sxs-lookup"><span data-stu-id="2cbb9-118">Update calendar items in batches</span></span>  <br/> |[<span data-ttu-id="2cbb9-119">упдатеитемс</span><span class="sxs-lookup"><span data-stu-id="2cbb9-119">UpdateItems</span></span>](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2cbb9-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2cbb9-120">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2cbb9-121">Удаление элементов календаря в пакетах</span><span class="sxs-lookup"><span data-stu-id="2cbb9-121">Delete calendar items in batches</span></span>  <br/> |[<span data-ttu-id="2cbb9-122">делетеитемс</span><span class="sxs-lookup"><span data-stu-id="2cbb9-122">DeleteItems</span></span>](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2cbb9-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="2cbb9-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |

<span data-ttu-id="2cbb9-124">В этой статье вы узнаете, как выполнить основные задачи для пакетов элементов календаря с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-124">In this article, you'll learn how to complete basic tasks for batches of calendar items by using the EWS Managed API or EWS.</span></span>

<span data-ttu-id="2cbb9-125">Обратите внимание, что в примерах управляемого API EWS, приведенных в этой статье, если методы вызываются последовательно, можно создать, получить, обновить и удалить пакет элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-125">Note that in the EWS Managed API examples in this article, if the methods are called sequentially, you can create, get, update, and then delete a batch of calendar items.</span></span>

```cs
Collection<ItemId> itemIds = BatchCreateCalendarItems(service);
Collection<Appointment> myAppointments = BatchGetCalendarItems(service, itemIds);
itemIds = BatchUpdateCalendarItems(service, myAppointments);
BatchDeleteCalendarItemsTwice(service, itemIds);

```

## <a name="create-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2cbb9-126">Создание элементов календаря в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-126">Create calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2cbb9-127"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-127"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="2cbb9-128">Вы можете создавать элементы календаря в пакетах, используя метод управляемого API [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-128">You can create calendar items in batches by using the [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="2cbb9-129">В этом примере создаются три объекта [встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) : встреча с одним экземпляром, повторяющаяся встреча и собрание, а затем они добавляются в коллекцию.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-129">This example creates three [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) objects — a single-instance appointment, a recurring appointment, and a meeting — and then adds them to a collection.</span></span>

<span data-ttu-id="2cbb9-130">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-130">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span>

```cs
public static Collection<ItemId> BatchCreateCalendarItems(ExchangeService service)
{
    // These are unsaved local instances of an Appointment object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Appointment appt1 = new Appointment(service);
    Appointment recurrAppt2 = new Appointment(service);
    Appointment meeting3 = new Appointment(service);
    // Set the properties for a single instance appointment.
    appt1.Subject = "Review current quarterly deliverables";
    appt1.Body = "Wrap up all outstanding deliverables for this quarter and prepare for Q2.";
    appt1.Start = DateTime.Now.AddDays(2);
    appt1.End = appt1.Start.AddHours(3);
    appt1.Location = "My office";
    appt1.ReminderMinutesBeforeStart = 30;
    // Set the properties for a recurring appointment.
    recurrAppt2.Subject = "Food bank delivery";
    recurrAppt2.Body = "Deliver the team's weekly food drive collection to the food bank.";
    recurrAppt2.Start = DateTime.Now.AddDays(1);
    recurrAppt2.End = recurrAppt2.Start.AddHours(1);
    recurrAppt2.Location = "Local food bank";
    arecurrAppt2.ReminderMinutesBeforeStart = 30;
    DayOfTheWeek[] dow = new DayOfTheWeek[] {(DayOfTheWeek)recurrAppt2.Start.DayOfWeek};
    recurrAppt2.Recurrence = new Recurrence.WeeklyPattern(recurrAppt2.Start.Date, 1, dow);
    recurrAppt2.Recurrence.StartDate = recurrAppt2.Start.Date;
    recurrAppt2.Recurrence.NumberOfOccurrences = 10;
    // Set the properties for a single instance meeting.
    meeting3.Subject = "Code Blast";
    meeting3.Body = "Let's get together to finish all the methods and unit tests for the ContosoLive project.";
    meeting3.Start = DateTime.Now.AddDays(3);
    meeting3.End = meeting3.Start.AddHours(6);
    meeting3.Location = "The lounge";
    meeting3.RequiredAttendees.Add("Mack@contoso.com");
    meeting3.RequiredAttendees.Add("Sadie@contoso.com");
    meeting3.RequiredAttendees.Add("Magdalena@contoso.com");
    meeting3.ReminderMinutesBeforeStart = 30;
    // Add the appointment objects to a collection.
    Collection<Appointment> calendarItems = new Collection<Appointment>() { appt1, recurrAppt2, meeting3 };
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();

    // Send the batch of Appointment objects.
    // Note that multiple calls to the Exchange server might be made when Appointment objects have attachments.
    // Note also that the the ID of the item collection passed as the first parameter to CreateItems is set on return.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(calendarItems,
                                                                              WellKnownFolderName.Calendar,
                                                                              MessageDisposition.SendAndSaveCopy,
                                                                              SendInvitationsMode.SendToAllAndSaveCopy);
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All appointments and meetings sucessfully created.");
    }
    // Collect the item IDs from the created calendar items.
    foreach (Appointment appt in calendarItems)
    {
        itemIds.Add(appt.Id);
    }
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
// Return the collection of item IDs.
return itemIds;
}

```

<span data-ttu-id="2cbb9-131">Объекты [встреч](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) в коллекции могут представлять собой встречи или собрания, а также отдельные экземпляры или повторяющиеся последовательности.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-131">The [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) objects in the collection can be appointments or meetings, and either single instances or a recurring series of either.</span></span>

## <a name="create-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="2cbb9-132">Создание элементов календаря в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-132">Create calendar items in batches by using EWS</span></span>
<span data-ttu-id="2cbb9-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-133"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="2cbb9-134">Вы можете создавать элементы календаря в пакетах с помощью операции [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-134">You can create calendar items in batches by using the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="2cbb9-135">Это также запрос XML, который отправляет управляемый API EWS при использовании управляемого API EWS для [создания элементов календаря в пакетах](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="2cbb9-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create calendar items in batches](#bk_createewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy" SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Review current quarterly deliverables</t:Subject>
          <t:Body BodyType="HTML">Wrap up all outstanding deliverables for this quarter and prepare for Q2.</t:Body>
          <t:ReminderDueBy>2014-01-07T12:13:40.333-08:00</t:ReminderDueBy>
          <t:Start>2014-01-08T13:13:37.717-08:00</t:Start>
          <t:End>2014-01-08T16:13:37.717-08:00</t:End>
          <t:Location>Local food bank</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Food bank delivery</t:Subject>
          <t:Body BodyType="HTML">Deliver the team's weekly food drive collection to the food bank.</t:Body>
          <t:Start>2014-01-07T13:13:40.333-08:00</t:Start>
          <t:End>2014-01-07T14:13:40.333-08:00</t:End>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Tuesday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-01-07-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Let's get together to finish all the methods and unit tests for the ContosoLive project.</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-01-09T13:13:44.998-08:00</t:Start>
          <t:End>2014-01-09T19:13:44.998-08:00</t:End>
          <t:Location>The lounge</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2cbb9-136">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для каждого** из новых элементов календаря, что означает, что каждый элемент календаря был создан успешно.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-136">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new calendar items, which indicates that each calendar item was created successfully.</span></span>

<span data-ttu-id="2cbb9-137">Обратите внимание, что элементы календаря представляют собой собрания или встречи, а также отдельные экземпляры или повторяющиеся ряды в соответствии со значениями элементов каждого элемента календаря, переданного на сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-137">Note that the calendar items are either meetings or appointments, or single instances or a recurring series, according to the element values of each calendar item passed to the Exchange server.</span></span>

<span data-ttu-id="2cbb9-138">Ниже приведен ответ от сервера.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-138">The following is the response from the server.</span></span> <span data-ttu-id="2cbb9-139">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-139">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="12" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2cbb9-140">Получение элементов календаря в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-140">Get calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2cbb9-141"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-141"><a name="bk_getewsma"> </a></span></span>

<span data-ttu-id="2cbb9-142">Вы можете получать элементы календаря в пакетах, используя метод управляемого API [биндтоитемс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-142">You can get calendar items in batches by using the [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span>

<span data-ttu-id="2cbb9-143">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-143">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span>

```cs
public static Collection<Appointment> BatchGetCalendarItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet appointmentProps = new PropertySet(BasePropertySet.IdOnly,
                                                   AppointmentSchema.Subject,
                                                   AppointmentSchema.Body,
                                                   AppointmentSchema.ReminderMinutesBeforeStart,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.AppointmentType,
                                                   AppointmentSchema.Location,
                                                   AppointmentSchema.RequiredAttendees);

    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, appointmentProps);
    Collection<Appointment> calendarItems = new Collection<Appointment>();
    foreach (GetItemResponse items in response)
    {
        Item item = items.Item;
        Appointment appointmentItem = (Appointment)item;
        calendarItems.Add(appointmentItem);
        Console.WriteLine("Found item {0}.", appointmentItem.Id.ToString().Substring(144));
    }
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All calendar items retrieved successfully.");
        Console.WriteLine("\r\n");
    }
    else
    {
        int counter = 1;
        // List the status of each message.
        foreach (ServiceResponse resp in response)
        {
            // Because item IDs are long, show only last 8 characters.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return calendarItems;
}

```

## <a name="get-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="2cbb9-144">Получение элементов календаря в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-144">Get calendar items in batches by using EWS</span></span>
<span data-ttu-id="2cbb9-145"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-145"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="2cbb9-146">Вы можете получать элементы календаря в пакетах с помощью операции [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-146">You can get calendar items in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="2cbb9-147">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [получения элементов календаря в пакетах](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="2cbb9-147">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get calendar items in batches](#bk_getewsma).</span></span>

<span data-ttu-id="2cbb9-148">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-148">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:Body" />
          <t:FieldURI FieldURI="item:ReminderMinutesBeforeStart" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:RequiredAttendees" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2cbb9-149">Сервер отвечает на запрос **GetItem** с сообщением [жетитемреспонсе](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) с запрошенными свойствами для каждого элемента, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-149">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message with the requested properties for each item, as shown in the following example.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="16" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Review current quarterly deliverables</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Wrap up all outstanding deliverables for this quarter and prepare for Q2.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-19T18:59:07Z</t:Start>
              <t:End>2014-01-19T21:59:07Z</t:End>
              <t:Location>Local food bank</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Food bank delivery</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Deliver the team's weekly food drive collection to the food bank.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-18T18:59:07Z</t:Start>
              <t:End>2014-01-18T19:59:07Z</t:End>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Code Blast</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Let's get together to finish all the methods and unit tests for the ContosoLive project.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-20T18:59:08Z</t:Start>
              <t:End>2014-01-21T00:59:08Z</t:End>
              <t:Location>The lounge</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:RequiredAttendees>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Mack@contoso.com</t:Name>
                    <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Sadie@contoso.com</t:Name>
                    <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Magdalena@contoso.com</t:Name>
                    <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
              </t:RequiredAttendees>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2cbb9-150">Обновление элементов календаря в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-150">Update calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2cbb9-151"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-151"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="2cbb9-152">Вы можете обновлять свойства элементов календаря в пакетах, используя метод управляемого API [упдатеитемс](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-152">You can update calendar item properties in batches by using the [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span>

<span data-ttu-id="2cbb9-153">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-153">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span>

```cs
public static Collection<ItemId> BatchUpdateCalendarItems(ExchangeService service, Collection<Appointment> calendarItems)
{
    int i = 1;
    // Appointment item IDs to return.
    Collection<ItemId> itemIds = new Collection<ItemId>();

    // Update the subject of each calendar item locally.
    foreach (Appointment appointment in calendarItems)
    {
        // Update the subject of each calendar item in the collection
        appointment.Subject = "Company headquarters are moving down the street to 1234 Contoso Drive!: " + appointment.Subject.ToString();
        Console.WriteLine("Updated the subject property for calendar item {0} of {1}, item id {2}.", i, calendarItems.Count, appointment.Id.ToString().Substring(0, 5));
        i++;
        // Collect item IDs to return instead of appointment objects.
        itemIds.Add(appointment.Id);
    }
    // Send the updated items to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(calendarItems,
                                                                                 WellKnownFolderName.Calendar,
                                                                                 ConflictResolutionMode.AutoResolve,
                                                                                 MessageDisposition.SendAndSaveCopy,
                                                                                    SendInvitationsOrCancellationsMode.SendToChangedAndSaveCopy);
    // Display the result of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Calendar items successfully updated.\r\n");
    }
    else
    {
        Console.WriteLine("Not all items were successfully updated on the server.\r\n");
        i = 1;
        foreach (ServiceResponse srvResponse in response)
        {
            Console.WriteLine("Result for message {0}: {1}", i, srvResponse.Result);
            Console.WriteLine("Error code: {0}", srvResponse.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", srvResponse.ErrorMessage);
            i++;
        }
    }
    return itemIds;
}

```

## <a name="update-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="2cbb9-154">Обновление элементов календаря в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-154">Update calendar items in batches by using EWS</span></span>
<span data-ttu-id="2cbb9-155"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-155"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="2cbb9-156">Вы можете обновить несколько элементов календаря с помощью операции [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-156">You can update multiple calendar items by using the [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="2cbb9-157">Это также запрос XML, который отправляет управляемый API EWS при использовании управляемого API EWS для [обновления элементов календаря в пакетах](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="2cbb9-157">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update calendar items in batches](#bk_updateewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SendAndSaveCopy" ConflictResolution="AutoResolve"
                  SendMeetingInvitationsOrCancellations="SendToChangedAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Review current quarterly deliverables
                </t:Subject>
                </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Food bank delivery</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Code Blast</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2cbb9-158">Сервер отвечает на запрос **UpdateItem** с сообщением [упдатеитемреспонсе](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , указывающее на то **, что**все обновления успешно сохранены на сервере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-158">The server responds to the **UpdateItem** request with an [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="2cbb9-159">Все конфликты включаются в элемент [конфликтресулт](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2cbb9-159">Any conflicts are reported in the [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13"
                         Version="V2_8" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="delete-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2cbb9-160">Удаление элементов календаря в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-160">Delete calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2cbb9-161"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-161"><a name="bk_deleteewsma"> </a></span></span>

<span data-ttu-id="2cbb9-162">Вы можете удалять элементы календаря в пакетах, используя метод управляемого API [делетеитемс](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-162">You can delete calendar items in batches by using the [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="2cbb9-163">В этом примере отменяется запрос на удаление во второй раз, чтобы показать, что исключения не возникают, но сервер возвращает ошибку **ерроритемнотфаунд** , указывающую на то, что элементы для удаления не были внесены в хранилище при вызове.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-163">This example makes the deletion request a second time to show that no exceptions are thrown but that the server will return an **ErrorItemNotFound** error to indicate that the items to delete weren't in the store when the call was made.</span></span> <span data-ttu-id="2cbb9-164">Эта ошибка возвращается, если элемент уже удален или на сервер передается идентификатор ошибочного элемента.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-164">This error is returned if the item has already been deleted, or if a bad item ID is passed to the server.</span></span>

<span data-ttu-id="2cbb9-165">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-165">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span>

```cs
public static void BatchDeleteCalendarItemsTwice(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of appointment objects
    // This method call results in a DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds,
                                                                                DeleteMode.MoveToDeletedItems,
                                                                                SendCancellationsMode.SendToAllAndSaveCopy,
                                                                                AffectedTaskOccurrence.AllOccurrences);
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }

    // Now attempt to delete the same items again.
    response = service.DeleteItems(itemIds,
                                    DeleteMode.MoveToDeletedItems,
                                    SendCancellationsMode.SendToAllAndSaveCopy,
                                    AffectedTaskOccurrence.AllOccurrences);
    counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
}

```

<span data-ttu-id="2cbb9-166">Если метод **делетеитемс** вызывается во второй раз, исключение не создается, но сервер возвращает ошибку **ерроритемнотфаунд** в результате.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-166">When the **DeleteItems** method is called the second time, no exception is thrown, but the server returns an **ErrorItemNotFound** error in the result.</span></span>

## <a name="delete-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="2cbb9-167">Удаление элементов календаря в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-167">Delete calendar items in batches by using EWS</span></span>
<span data-ttu-id="2cbb9-168"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-168"><a name="bk_deleteews"> </a></span></span>

<span data-ttu-id="2cbb9-169">Вы можете удалять элементы календаря в пакетах с помощью операции [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-169">You can delete calendar items in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="2cbb9-170">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [удаления элементов календаря в пакетах](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="2cbb9-170">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete calendar items in batches](#bk_deleteewsma).</span></span>

<span data-ttu-id="2cbb9-171">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-171">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems"
                  AffectedTaskOccurrences="AllOccurrences"
                  SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2cbb9-172">Сервер отвечает на запрос **DeleteItem** с сообщением [делетеитемреспонсе](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для удаления для каждого** удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-172">The server responds to the **DeleteItem** request with a [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="2cbb9-173">Обратите внимание, что при выполнении запроса **DeleteItem** , когда связанные элементы уже были удалены, исключение не создается, но сервер возвратит ошибку **ерроритемнотфаунд** в результат.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-173">Note that if the **DeleteItem** request is made when the associated items have already been deleted, no exception will be thrown, but the server will return an **ErrorItemNotFound** error in the result.</span></span> <span data-ttu-id="2cbb9-174">В следующем примере показан ответ сервера на запрос **DeleteItem** , когда связанные элементы уже были удалены.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-174">The following example shows the server response to a **DeleteItem** request when the associated items have already been deleted.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="2cbb9-175">Проверка успешного завершения пакетной обработки</span><span class="sxs-lookup"><span data-stu-id="2cbb9-175">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="2cbb9-176"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="2cbb9-176"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="2cbb9-177">Если один или несколько элементов календаря в пакетном запросе не могут быть обработаны как запрошенные, возвращается ошибка для каждого элемента календаря с ошибкой, а остальные элементы календаря в пакете обрабатываются должным образом.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-177">When one or more calendar items in a batched request can't be processed as requested, an error is returned for each calendar item that failed, and the rest of the calendar items in the batch are processed as expected.</span></span> <span data-ttu-id="2cbb9-178">Ошибки в пакетной обработке могут возникать, если элемент был удален, поэтому не может быть отправлен, извлечен или обновлен, или если элемент перемещен в другую папку, и поэтому не может быть изменен с помощью идентификатора элемента.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-178">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="2cbb9-179">Сведения в этом разделе показывают, как получить сведения об ошибках при пакетной обработке элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-179">The information in this section shows how to get error details about failures in batch processing of calendar items.</span></span>

<span data-ttu-id="2cbb9-180">Чтобы проверить успешность пакетной обработки с помощью управляемого API EWS, можно проверить, что свойство [овераллресулт](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) объекта [сервицереспонсеколлектион](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) равно [сервицересулт. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2cbb9-180">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="2cbb9-181">В таком случае все элементы календаря обрабатывались успешно.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-181">If so, all the calendar items were processed successfully.</span></span> <span data-ttu-id="2cbb9-182">Если **овераллресулт** не равно **сервицересулт. Success**, один или несколько элементов календаря не были обработаны успешно.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-182">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the calendar items were not processed successfully.</span></span> <span data-ttu-id="2cbb9-183">Каждый из объектов, возвращенных в **сервицереспонсеколлектион** , содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="2cbb9-183">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span>

- [<span data-ttu-id="2cbb9-184">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="2cbb9-184">ErrorCode</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [<span data-ttu-id="2cbb9-185">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="2cbb9-185">ErrorDetails</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [<span data-ttu-id="2cbb9-186">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="2cbb9-186">ErrorMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [<span data-ttu-id="2cbb9-187">еррорпропертиес</span><span class="sxs-lookup"><span data-stu-id="2cbb9-187">ErrorProperties</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [<span data-ttu-id="2cbb9-188">Результат</span><span class="sxs-lookup"><span data-stu-id="2cbb9-188">Result</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

<span data-ttu-id="2cbb9-189">Эти свойства содержат сведения о том, почему не удалось обработать элементы календаря по запросу.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-189">These properties contain information about why the calendar items could not be processed as requested.</span></span> <span data-ttu-id="2cbb9-190">В примерах, приведенных в этой статье, распечатываться **результат**, **ErrorCode**и **ErrorMessage** для каждого ошибочного элемента.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-190">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed item.</span></span> <span data-ttu-id="2cbb9-191">Вы можете использовать эти результаты для изучения проблемы.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-191">You can use these results to investigate the issue.</span></span>

<span data-ttu-id="2cbb9-192">Для проверки успешности пакетного процесса в EWS проверьте атрибут [респонсекласс](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) для каждого обрабатываемого элемента.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-192">For EWS, to verify the success of a batched process, check the [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="2cbb9-193">Ниже приведена базовая структура **респонсемессажетипе**, базовый тип которого является производным от всех ответных сообщений.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-193">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span>

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="2cbb9-194">Атрибут **респонсекласс** имеет значение **Success** , если элемент календаря был обработан успешно, или **Ошибка** , если она не была успешно обработана.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-194">The **ResponseClass** attribute is set to **Success** if the calendar item was processed successfully, or **Error** if it was not processed successfully.</span></span> <span data-ttu-id="2cbb9-195">Для элементов календаря не будет появляться **предупреждение** во время пакетной обработки.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-195">For calendar items, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="2cbb9-196">Если **Респонсекласс** **успешно**, элемент [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , который следует за ним, также всегда имеет значение " **Ошибка**".</span><span class="sxs-lookup"><span data-stu-id="2cbb9-196">If the **ResponseClass** is **Success**, the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="2cbb9-197">Если **респонсекласс** является **ошибкой**, необходимо проверить значения элементов [мессажетекст](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **респонсекоде**и [мессажексмл](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) , чтобы определить, что привело к проблеме.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-197">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="2cbb9-198">[Дескриптивелинккэй](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) в настоящее время не используется.</span><span class="sxs-lookup"><span data-stu-id="2cbb9-198">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span>

## <a name="see-also"></a><span data-ttu-id="2cbb9-199">См. также</span><span class="sxs-lookup"><span data-stu-id="2cbb9-199">See also</span></span>


- [<span data-ttu-id="2cbb9-200">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-200">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)

- [<span data-ttu-id="2cbb9-201">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-201">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)

- [<span data-ttu-id="2cbb9-202">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-202">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)

- [<span data-ttu-id="2cbb9-203">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-203">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)

- [<span data-ttu-id="2cbb9-204">Обработка элементов календаря в пакетах Exchange</span><span class="sxs-lookup"><span data-stu-id="2cbb9-204">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)

- [<span data-ttu-id="2cbb9-205">Влияние регулирования на пакетные запросы EWS</span><span class="sxs-lookup"><span data-stu-id="2cbb9-205">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)
