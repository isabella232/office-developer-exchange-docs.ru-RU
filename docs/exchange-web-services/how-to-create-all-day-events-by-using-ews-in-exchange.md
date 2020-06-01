---
title: Создание событий на целый день с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Узнайте, как создавать события на целый день с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 6be638c17cc0e0c86fa6b4217169aa7259dfd4aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456866"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="542e4-103">Создание событий на целый день с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="542e4-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="542e4-104">Узнайте, как создавать события на целый день с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="542e4-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="542e4-105">События на целый день представляют собой способ представления какого-либо действия за целый день или несколько дней (например, праздничный день или дни отпуска).</span><span class="sxs-lookup"><span data-stu-id="542e4-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="542e4-106">Создание событий на целый день с помощью управляемого API EWS или EWS является привязкой.</span><span class="sxs-lookup"><span data-stu-id="542e4-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="542e4-107">Это так же, как [Создание встреч](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), но с несколькими небольшими изменениями.</span><span class="sxs-lookup"><span data-stu-id="542e4-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="542e4-108">Установка времени начала и окончания</span><span class="sxs-lookup"><span data-stu-id="542e4-108">Setting start and end times</span></span>

<span data-ttu-id="542e4-109">По определению, события на целый день начинаются с полуночи в определенный день и заканчиваются 24 часа (или несколько минут в 24 часа).</span><span class="sxs-lookup"><span data-stu-id="542e4-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="542e4-110">Тем не менее, управляемый API EWS и EWS позволяют указать время, отличное от полуночи, при создании событий на целый день.</span><span class="sxs-lookup"><span data-stu-id="542e4-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="542e4-111">Это может привести к нежелательному поведению, если вы не помните о том, как эти времена будут переведены на сервер.</span><span class="sxs-lookup"><span data-stu-id="542e4-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="542e4-112">При получении запроса на создание нового события на целый день без полуночи (в часовом [поясе запроса или встречи](time-zones-and-ews-in-exchange.md)) эти времена корректируются до полуночи в соответствующем часовом поясе в соответствии со следующими правилами:</span><span class="sxs-lookup"><span data-stu-id="542e4-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="542e4-113">Время начала не в полночь регулируется до полуночи до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="542e4-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="542e4-114">Например, 1:00 PM на 6 июня будет изменено на 12:00 AM 6 июня.</span><span class="sxs-lookup"><span data-stu-id="542e4-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="542e4-115">Время окончания не в полночь регулируется до полуночи по истечении указанного времени.</span><span class="sxs-lookup"><span data-stu-id="542e4-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="542e4-116">Например, 1:00 PM на 6 июня будет скорректировано до версии 12:00 AM 7 июня.</span><span class="sxs-lookup"><span data-stu-id="542e4-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="542e4-117">Поэтому создаваемое событие на целый день всегда является инклюзивным с указанным временем начала и окончания, но может потребовать дополнительного времени в календаре пользователя из-за смены в полночь.</span><span class="sxs-lookup"><span data-stu-id="542e4-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="542e4-118">Так как на сервере будет задано время начала и окончания, рекомендуется указать время начала и окончания на полночь, чтобы избежать нежелательных изменений.</span><span class="sxs-lookup"><span data-stu-id="542e4-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="542e4-119">Кроме того, важно учитывать часовые пояса при создании событий на целый день.</span><span class="sxs-lookup"><span data-stu-id="542e4-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="542e4-120">Так как сервер Exchange применяет время начала и окончания полуночи в часовом поясе запроса или встречи, просмотр этого события на весь день в клиенте, настроенном для другого часового пояса, может привести к непредвиденным результатам.</span><span class="sxs-lookup"><span data-stu-id="542e4-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="542e4-121">В зависимости от клиента он может отображаться как событие на целый день с дополнительными днями, которые не планировалось включать, или вообще не отображаться как событие на целый день.</span><span class="sxs-lookup"><span data-stu-id="542e4-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="542e4-122">В связи с этим мы рекомендуем использовать предпочтительный часовой пояс пользователя, когда это возможно, при создании событий на целый день.</span><span class="sxs-lookup"><span data-stu-id="542e4-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="542e4-123">Создание события на целый день с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="542e4-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="542e4-124">В приведенном ниже примере показано, как использовать управляемый API EWS для создания события на целый день, начиная с даты, указанной параметром _StartDate_ , и зафиксированной в течение числа дней, заданного параметром _нумдайс_ .</span><span class="sxs-lookup"><span data-stu-id="542e4-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="542e4-125">Обратите внимание, что встреча будет создана в часовом поясе, указанном в свойстве [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="542e4-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="542e4-126">В этом примере предполагается, что объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , переданный в параметре _Service_ , инициализирован с допустимыми значениями для свойств [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="542e4-126">This example assumes that the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void CreateAllDayAppointment(ExchangeService service, DateTime startDate, int numDays)
{
    // Best practice is to set the start date to midnight
    // on the first day of the all-day event.
    DateTime startDateMidnight = startDate.Date;
    // The end date should be midnight on the first day
    // after the event.
    DateTime endDateMidnight = startDateMidnight.AddDays(numDays);
    Appointment allDayEvent = new Appointment(service);
    // Set IsAllDayEvent to true.
    allDayEvent.IsAllDayEvent = true;
    // Set other properties.
    allDayEvent.Subject = "Vacation";
    allDayEvent.LegacyFreeBusyStatus = LegacyFreeBusyStatus.OOF;
    allDayEvent.Start = startDateMidnight;
    allDayEvent.End = endDateMidnight;
    // Save the appointment.
    try
    {
        allDayEvent.Save(WellKnownFolderName.Calendar, SendInvitationsMode.SendToNone);
        Console.WriteLine("All day event created.");
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving all day event: {0}", ex.Message);
    }
}
```

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="542e4-127">Создание события на целый день с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="542e4-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="542e4-128">В следующем примере показан запрос [операции CREATEITEM](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для создания события на целый день.</span><span class="sxs-lookup"><span data-stu-id="542e4-128">The following example shows an EWS [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="542e4-129">Встреча создается в Восточном часовом поясе, как указано в элементе [тимезонеконтекст](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="542e4-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="542e4-130">Обратите внимание, что в качестве части значений [начального](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [конечного](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) элементов указаны оба значения 04:00Z, которые преобразуются в полночь в Восточном часовом поясе во время летнего времени.</span><span class="sxs-lookup"><span data-stu-id="542e4-130">Notice that the time portion of the values of the [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Vacation</t:Subject>
          <t:Start>2014-06-09T04:00:00.000Z</t:Start>
          <t:End>2014-06-10T04:00:00.000Z</t:End>
          <t:IsAllDayEvent>true</t:IsAllDayEvent>
          <t:LegacyFreeBusyStatus>OOF</t:LegacyFreeBusyStatus>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="542e4-131">См. также</span><span class="sxs-lookup"><span data-stu-id="542e4-131">See also</span></span>


- [<span data-ttu-id="542e4-132">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="542e4-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="542e4-133">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="542e4-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="542e4-134">Часовые пояса и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="542e4-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    

