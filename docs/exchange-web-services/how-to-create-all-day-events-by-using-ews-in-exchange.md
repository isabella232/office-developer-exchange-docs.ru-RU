---
title: Создание событий на целый день с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Сведения о создании событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 0547fdf0ca92ba0648caeb5de6940d90d2a8ff46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760989"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="bc02d-103">Создание событий на целый день с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc02d-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="bc02d-104">Сведения о создании событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc02d-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="bc02d-105">События предусмотрена возможность представления, которое происходит для целый день или несколько дней — например, в выходные дни и даже дней отпуска.</span><span class="sxs-lookup"><span data-stu-id="bc02d-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="bc02d-106">Создание событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange — это просто.</span><span class="sxs-lookup"><span data-stu-id="bc02d-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="bc02d-107">Это так же, как [Создание встреч](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), но с небольшие изменения.</span><span class="sxs-lookup"><span data-stu-id="bc02d-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="bc02d-108">Установка времени начала и завершения</span><span class="sxs-lookup"><span data-stu-id="bc02d-108">Setting start and end times</span></span>

<span data-ttu-id="bc02d-109">По определению, запустите событий на целый день в полночь на определенный день и конечных 24 часа (или несколько 24 часов) более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="bc02d-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="bc02d-110">Тем не менее, управляемый API EWS и веб-служб Exchange позволяют указать время, отличный от полуночи при создании события на целый день.</span><span class="sxs-lookup"><span data-stu-id="bc02d-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="bc02d-111">Это может привести к непредвиденным поведение, если вы не знать о том, как это время получения преобразовываться на сервере.</span><span class="sxs-lookup"><span data-stu-id="bc02d-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="bc02d-112">При получении запроса Чтобы создать новое событие на целый день с начала не полночь (в [часовой пояс запроса или встреча](time-zones-and-ews-in-exchange.md)) и/или время окончания, то время, получение настроено в полночь в соответствующие часовой пояс определяется следующими правилами:</span><span class="sxs-lookup"><span data-stu-id="bc02d-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="bc02d-113">Время начала полночь не настроены на полночь до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="bc02d-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="bc02d-114">Например 1:00 PM на 6 июня получает настроенные до 12:00 на 6 июня.</span><span class="sxs-lookup"><span data-stu-id="bc02d-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="bc02d-115">Время окончания полночь не настроены на полночь после указанного времени.</span><span class="sxs-lookup"><span data-stu-id="bc02d-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="bc02d-116">Например 1:00 PM на 6 июня получает настроенные до 12:00 на 7 июня.</span><span class="sxs-lookup"><span data-stu-id="bc02d-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="bc02d-117">Поэтому всегда включая время начала и окончания, укажите, но может затребовать дополнительное время на события, создаваемого пользователя 's календаря из-за shift до полуночи.</span><span class="sxs-lookup"><span data-stu-id="bc02d-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="bc02d-118">Так как сервер будет настроить время начала и окончания полночь, рекомендуется указать времени начала и окончания в полночь, чтобы избежать непреднамеренного изменения значения времени.</span><span class="sxs-lookup"><span data-stu-id="bc02d-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="bc02d-119">Также важно учесть часовые пояса при создании событий на целый день.</span><span class="sxs-lookup"><span data-stu-id="bc02d-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="bc02d-120">Так как Exchange server обеспечивает полночь начала и окончания времени в часовом поясе запроса или встречи, просмотр, целый день в клиент, настроенный для различных часового пояса может привести к непредсказуемым последствиям.</span><span class="sxs-lookup"><span data-stu-id="bc02d-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="bc02d-121">В зависимости от клиента она может оказаться событием на целый день с помощью дополнительных дней, которые не будут включать или она может не отображаться в событием на целый день полностью.</span><span class="sxs-lookup"><span data-stu-id="bc02d-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="bc02d-122">Таким образом мы рекомендуем использовать предпочтительный часовой пояс пользователя по возможности при создании событий на целый день.</span><span class="sxs-lookup"><span data-stu-id="bc02d-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="bc02d-123">Создание событием на целый день с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="bc02d-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="bc02d-124">Следующем примере показано, как использовать управляемый API веб-служб Exchange для создания событием на целый день, начиная с даты, указанного с помощью параметра _startDate_ и выполняемых числа дней, указанных в параметре _numDays_ .</span><span class="sxs-lookup"><span data-stu-id="bc02d-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="bc02d-125">Обратите внимание, что в часовом поясе, указанном свойством [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) будет создано встречи.</span><span class="sxs-lookup"><span data-stu-id="bc02d-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="bc02d-126">В этом примере предполагается, что объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , переданной в параметре _службы_ была ли инициализирована на допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bc02d-126">This example assumes that the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="bc02d-127">Создание событием на целый день с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="bc02d-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="bc02d-128">В следующем примере показано запрос веб-служб Exchange [операции CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания событием на целый день.</span><span class="sxs-lookup"><span data-stu-id="bc02d-128">The following example shows an EWS [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="bc02d-129">Встречи создается по восточному поясному времени, как указано в элементе [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bc02d-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="bc02d-130">Обратите внимание, что время часть значения элементов [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) обоих 04:00Z, который преобразует в полночь в по восточному поясному времени во время перехода на летнее время.</span><span class="sxs-lookup"><span data-stu-id="bc02d-130">Notice that the time portion of the values of the [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="see-also"></a><span data-ttu-id="bc02d-131">См. также</span><span class="sxs-lookup"><span data-stu-id="bc02d-131">See also</span></span>


- [<span data-ttu-id="bc02d-132">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="bc02d-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="bc02d-133">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bc02d-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="bc02d-134">Часовые пояса и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc02d-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
