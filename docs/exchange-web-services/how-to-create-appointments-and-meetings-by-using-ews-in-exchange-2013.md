---
title: Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fdea70a4-9267-4e5d-9152-b749e2acc3b0
description: Сведения о создании встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 1c840fac2ecca9fb51a28044dfac6299cb4fc038
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760998"
---
# <a name="create-appointments-and-meetings-by-using-ews-in-exchange-2013"></a><span data-ttu-id="458f6-103">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="458f6-103">Create appointments and meetings by using EWS in Exchange 2013</span></span>

<span data-ttu-id="458f6-104">Сведения о создании встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="458f6-104">Learn how to create appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="458f6-105">Важные различия между собраний и встреч —, что у участников собрания, а не встреч.</span><span class="sxs-lookup"><span data-stu-id="458f6-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="458f6-106">Встречи и собрания могут быть отдельные экземпляры или частью серии повторяющихся, но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="458f6-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="458f6-107">Для внутреннего использования Exchange использует тот же объект для собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="458f6-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="458f6-108">Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) для работы с собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="458f6-108">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="458f6-109">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для работы с встречи и собрания**</span><span class="sxs-lookup"><span data-stu-id="458f6-109">**Table 1. EWS Managed API methods and EWS operations for working with appointments and meetings**</span></span>

|<span data-ttu-id="458f6-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="458f6-110">**EWS Managed API method**</span></span>|<span data-ttu-id="458f6-111">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="458f6-111">**EWS operation**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="458f6-112">Appointment.Save</span><span class="sxs-lookup"><span data-stu-id="458f6-112">Appointment.Save</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="458f6-113">Операции CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="458f6-113">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="458f6-114">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="458f6-114">Item.Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/dd634410%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="458f6-115">Операции GetItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="458f6-115">GetItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
   
## <a name="create-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="458f6-116">Создание встречи с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-116">Create an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="458f6-117"><a name="bk_CreateApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="458f6-117"></span></span>

<span data-ttu-id="458f6-118">В следующем примере кода показано, как использовать [объект Appointment](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) для создания встречи, метод [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для сохранения в папке календаря и метод [Item.Bind](http://msdn.microsoft.com/ru-ru/library/dd634410%28v=exchg.80%29.aspx) , чтобы убедиться, что был создан встречи.</span><span class="sxs-lookup"><span data-stu-id="458f6-118">The following code example shows how to use the [Appointment object](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) to create an appointment, the [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to save it to your calendar folder, and the [Item.Bind](http://msdn.microsoft.com/ru-ru/library/dd634410%28v=exchg.80%29.aspx) method to verify that the appointment was created.</span></span> 
  
<span data-ttu-id="458f6-119">В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="458f6-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment appointment = new Appointment(service);
// Set the properties on the appointment object to create the appointment.
appointment.Subject = "Tennis lesson";
appointment.Body = "Focus on backhand this week.";
appointment.Start = DateTime.Now.AddDays(2);
appointment.End = appointment.Start.AddHours(1);
appointment.Location = "Tennis club";
appointment.ReminderDueBy = DateTime.Now;
// Save the appointment to your calendar.
appointment.Save(SendInvitationsMode.SendToNone);
// Verify that the appointment was created by using the appointment's item ID.
Item item = Item.Bind(service, appointment.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nAppointment created: " + item.Subject + "\n");

```

<span data-ttu-id="458f6-120">После установки свойства объекта встречи, встречи сохраните в папке календаря с помощью метода [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) объекта встречи.</span><span class="sxs-lookup"><span data-stu-id="458f6-120">After setting the properties on the appointment object, you save the appointment to the calendar folder by using the appointment object's [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="458f6-121">Обратите внимание на то, что на этапе проверки, вы элемента [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) , связанный с встречи в убедитесь, что встречи, в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="458f6-121">Note that in the verification step, you use the item [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the appointment to verify that the appointment is in the calendar folder.</span></span> <span data-ttu-id="458f6-122">Рекомендуется, ограничить свойства, возвращенные сервером для только что необходимо — в этом случае Тема встречи.</span><span class="sxs-lookup"><span data-stu-id="458f6-122">As a best practice, limit the properties returned by the server to only what you need — in this case, the appointment's subject.</span></span> 
  
## <a name="create-an-appointment-by-using-ews"></a><span data-ttu-id="458f6-123">Создание встречи с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-123">Create an appointment by using EWS</span></span>
<span data-ttu-id="458f6-124"><a name="bk_CreateApptEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="458f6-124"></span></span>

<span data-ttu-id="458f6-125">Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с кодом управляемый API EWS в разделе [Создание встречи с помощью управляемого интерфейса API веб-служб Exchange](#bk_CreateApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="458f6-125">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Create an appointment by using the EWS Managed API](#bk_CreateApptEWSMA).</span></span> <span data-ttu-id="458f6-126">Также показаны запрос и ответ XML-кода, выполняется проверка наличия элементы встреч в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="458f6-126">The request and response XML that verifies that the appointment items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="458f6-127">В следующем примере показано запроса XML при использовании операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания встречи.</span><span class="sxs-lookup"><span data-stu-id="458f6-127">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an appointment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

 <span data-ttu-id="458f6-128">В следующем примере показано XML, возвращенные операцией **CreateItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="458f6-128">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-129">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-129">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
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

<span data-ttu-id="458f6-130">В следующем примере показано запрос, который был создан XML, которая порождается при использовании операции [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) чтобы убедиться, что встречи.</span><span class="sxs-lookup"><span data-stu-id="458f6-130">The following example shows the request XML that is generated when you use the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation to verify that the appointment was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-131">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-131">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="458f6-132">В следующем примере показано XML, возвращенные операцией **GetItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="458f6-132">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-133">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-133">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Tennis lesson</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="create-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="458f6-134">Создание встречи с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-134">Create a meeting by using the EWS Managed API</span></span>
<span data-ttu-id="458f6-135"><a name="bk_CreateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="458f6-135"></span></span>

<span data-ttu-id="458f6-136">При создании собрания, в дополнение к Сохранение элемента в папке календаря обычно также требуется отправлять приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="458f6-136">When you create a meeting, in addition to saving an item to the calendar folder, you also typically want to send meeting requests to attendees.</span></span> <span data-ttu-id="458f6-137">В следующем примере кода показано, как создать встречу и отправка приглашений на собрания.</span><span class="sxs-lookup"><span data-stu-id="458f6-137">The following code example shows how to create a meeting and send meeting requests.</span></span>
  
<span data-ttu-id="458f6-138">В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="458f6-138">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment meeting = new Appointment(service);
// Set the properties on the meeting object to create the meeting.
meeting.Subject = "Team building exercise";
meeting.Body = "Let's learn to really work as a team and then have lunch!";
meeting.Start = DateTime.Now.AddDays(2);            
meeting.End = meeting.Start.AddHours(4);
meeting.Location = "Conference Room 12";
meeting.RequiredAttendees.Add("Mack@contoso.com");
meeting.RequiredAttendees.Add("Sadie@contoso.com");
meeting.OptionalAttendees.Add("Magdalena@contoso.com");
meeting.ReminderMinutesBeforeStart = 60;
// Save the meeting to the Calendar folder and send the meeting request.
meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
// Verify that the meeting was created.
Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nMeeting created: " + item.Subject + "\n");

```

<span data-ttu-id="458f6-139">После установки свойства объекта [встречи](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , сохраните собрания в папке календаря с помощью метода [Save](http://msdn.microsoft.com/ru-ru/library/dd635394%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="458f6-139">After setting the properties on the [Appointment](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, save the meeting to your calendar folder by using the [Save](http://msdn.microsoft.com/ru-ru/library/dd635394%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="458f6-140">При установке значения перечисления [SendInvitationsMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) **SendOnlyToAll** или **SendToAllAndSaveCopy**отправляются приглашения участников.</span><span class="sxs-lookup"><span data-stu-id="458f6-140">When you set the [SendInvitationsMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) enumeration value to **SendOnlyToAll** or **SendToAllAndSaveCopy**, invitations are sent to attendees.</span></span>
  
<span data-ttu-id="458f6-141">Использование элемента [код](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) , связанный с собрания, чтобы убедиться, что она была сохранена в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="458f6-141">Use the item [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the meeting to verify that it was saved in the calendar folder.</span></span> <span data-ttu-id="458f6-142">Рекомендуется ограничение свойства, возвращенные сервером для только что необходимо — в этом случае тему собрания.</span><span class="sxs-lookup"><span data-stu-id="458f6-142">As a best practice, limit the properties returned by the server to only what you need - in this case, the meeting's subject.</span></span> 
  
## <a name="create-a-meeting-by-using-ews"></a><span data-ttu-id="458f6-143">Создание встречи с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-143">Create a meeting by using EWS</span></span>
<span data-ttu-id="458f6-144"><a name="bk_CreateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="458f6-144"></span></span>

<span data-ttu-id="458f6-145">Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [Создание собрания с помощью управляемого интерфейса API веб-служб Exchange](#bk_CreateMtgEWSMA).</span><span class="sxs-lookup"><span data-stu-id="458f6-145">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Create a meeting by using the EWS Managed API](#bk_CreateMtgEWSMA).</span></span> <span data-ttu-id="458f6-146">Также показаны запрос и ответ XML-кода, выполняется проверка наличия собрания элементов в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="458f6-146">The request and response XML that verifies that the meeting items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="458f6-147">В следующем примере показано запроса XML при использовании операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания.</span><span class="sxs-lookup"><span data-stu-id="458f6-147">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2013-09-21T16:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:OptionalAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena.Kemp@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:OptionalAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="458f6-148">В следующем примере показано XML, возвращенные операцией **CreateItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="458f6-148">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-149">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-149">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
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

<span data-ttu-id="458f6-150">В следующем примере показано запроса XML, который создается операции [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) при убедитесь, что был создан собрания.</span><span class="sxs-lookup"><span data-stu-id="458f6-150">The following example shows the request XML that is generated by the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation when you verify that the meeting was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-151">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-151">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="458f6-152">В следующем примере показано XML, возвращенные операцией **GetItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="458f6-152">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="458f6-153">Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="458f6-153">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Team building exercise</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="458f6-154">См. также</span><span class="sxs-lookup"><span data-stu-id="458f6-154">See also</span></span>

- [<span data-ttu-id="458f6-155">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-155">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)  
- [<span data-ttu-id="458f6-156">Получение встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-156">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="458f6-157">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-157">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="458f6-158">Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-158">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="458f6-159">Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="458f6-159">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

