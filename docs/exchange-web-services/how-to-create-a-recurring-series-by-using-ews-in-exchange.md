---
title: Создание серии повторяющихся данных с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 88ed6e87-25f7-4a54-83fa-d757a0ff2528
description: Узнайте, как создавать повторяющиеся собрания с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: db25fd4c97755248ebbbc7637a71749f485f8fa8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760990"
---
# <a name="create-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="8a3db-103">Создание серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3db-103">Create a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="8a3db-104">Узнайте, как создавать повторяющиеся собрания с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a3db-104">Learn how to create recurring meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8a3db-105">Создание повторяющейся встречи или собрания не так сильно отличается от создания [встречи или собрания с одним экземпляром](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="8a3db-105">Creating a recurring appointment or meeting isn't all that much different than creating [a single instance appointment or meeting](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span> <span data-ttu-id="8a3db-106">Необходимо только назначить значения нескольким дополнительным свойствам, связанным с повторением.</span><span class="sxs-lookup"><span data-stu-id="8a3db-106">You just need to assign values to a few additional recurrence-related properties.</span></span> <span data-ttu-id="8a3db-107">Они задаются для объекта [повторения](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) объекта [ExchangeService. Встреча](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) (при использовании управляемого API EWS) или дочернего элемента [повторения](http://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) элемента [календаритем](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) (если вы используете EWS).</span><span class="sxs-lookup"><span data-stu-id="8a3db-107">These are set on an [ExchangeService.Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object's [Recurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) object (if you're using the EWS Managed API), or the [Recurrence](http://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) child element of a [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element (if you're using EWS).</span></span> <span data-ttu-id="8a3db-108">Если вы создаете повторяющееся собрание, а не на одном экземпляре, следует учитывать, что создаваемый элемент календаря является шаблоном повторения для ряда.</span><span class="sxs-lookup"><span data-stu-id="8a3db-108">One thing to consider when you create a recurring, rather than a single-instance meeting, is that the calendar item you create is the recurring master for a series.</span></span> <span data-ttu-id="8a3db-109">Ряд свойств устанавливается только в повторяющейся основной реплике; Эти свойства помогут найти, изменить или удалить отдельные экземпляры в ряду.</span><span class="sxs-lookup"><span data-stu-id="8a3db-109">A number of properties are set only on a recurring master; these properties can help you find, modify, or delete individual instances in a series.</span></span> <span data-ttu-id="8a3db-110">По этой причине при создании серии повторяющихся данных может быть полезно отслеживать идентификатор повторяющегося образца...</span><span class="sxs-lookup"><span data-stu-id="8a3db-110">For this reason, it might be useful to keep track of the ID of the recurring master when you create a recurring series.</span></span> 
  
<span data-ttu-id="8a3db-111">**Таблица 1. Свойства, заданные для повторяющихся элементов главного календаря**</span><span class="sxs-lookup"><span data-stu-id="8a3db-111">**Table 1. Properties set on recurring master calendar items**</span></span>

|<span data-ttu-id="8a3db-112">**Класс или свойство управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="8a3db-112">**EWS Managed API class or property**</span></span>|<span data-ttu-id="8a3db-113">**Элемент XML EWS**</span><span class="sxs-lookup"><span data-stu-id="8a3db-113">**EWS XML element**</span></span>|<span data-ttu-id="8a3db-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a3db-114">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="8a3db-115">Класс повторения</span><span class="sxs-lookup"><span data-stu-id="8a3db-115">Recurrence class</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) <br/> <span data-ttu-id="8a3db-116">Класс **повторения** — это базовый класс производного класса шаблона: [интервалпаттерн](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx), [релативэйеарлипаттерн](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx)или [еарлипаттерн](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8a3db-116">The **Recurrence** class is the base class for a derived pattern class, either [IntervalPattern](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx), [RelativeYearlyPattern](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx), or [YearlyPattern](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).</span></span>  <br/> |[<span data-ttu-id="8a3db-117">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8a3db-117">Recurrence (RecurrenceType)</span></span>](http://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a3db-118">Содержит сведения, связанные с повторением, включая расписание повторения (ежедневно, еженедельно, ежемесячно и т. д.), дату начала и окончания, число повторений и т. д.</span><span class="sxs-lookup"><span data-stu-id="8a3db-118">Contains recurrence-related information, including the recurrence pattern (daily, weekly, monthly, and so on), start and end date, number of occurrences, and so on.</span></span>  <br/> |
|[<span data-ttu-id="8a3db-119">Свойство Фирстоккурренце</span><span class="sxs-lookup"><span data-stu-id="8a3db-119">FirstOccurrence property</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a3db-120">фирстоккурренце</span><span class="sxs-lookup"><span data-stu-id="8a3db-120">FirstOccurrence</span></span>](http://msdn.microsoft.com/library/d6748860-ce0d-4d2e-b7e4-9ed834f1e45a%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a3db-121">Содержит начальное и конечное время и идентификатор элемента для первого собрания в ряду.</span><span class="sxs-lookup"><span data-stu-id="8a3db-121">Contains the start and end times and the item ID for the first meeting in a series.</span></span>  <br/> |
|[<span data-ttu-id="8a3db-122">Свойство Ластоккурренце</span><span class="sxs-lookup"><span data-stu-id="8a3db-122">LastOccurrence property</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a3db-123">ластоккурренце</span><span class="sxs-lookup"><span data-stu-id="8a3db-123">LastOccurrence</span></span>](http://msdn.microsoft.com/library/c9ef0fcb-4265-4e60-9986-fff0f211d00b%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a3db-124">Содержит начальное и конечное время, а также идентификатор элемента для последнего собрания в ряду.</span><span class="sxs-lookup"><span data-stu-id="8a3db-124">Contains the start and end times and the item ID for the last meeting in a series.</span></span>  <br/> |
|[<span data-ttu-id="8a3db-125">Свойство Модифиедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="8a3db-125">ModifiedOccurrences property</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a3db-126">модифиедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="8a3db-126">ModifiedOccurrences</span></span>](http://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a3db-127">Содержит набор всех собраний в серии, которые были изменены из исходного шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="8a3db-127">Contains the set of all meetings in the series that have been modified from the original recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8a3db-128">Свойство Делетедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="8a3db-128">DeletedOccurrences property</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a3db-129">делетедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="8a3db-129">DeletedOccurrences</span></span>](http://msdn.microsoft.com/library/736fb305-9528-4be8-ad37-65d7556edbf2%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a3db-130">Содержит набор всех собраний в серии, которые были удалены из исходного шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="8a3db-130">Contains the set of all meetings in the series that have been deleted from the original recurrence pattern.</span></span>  <br/> |
   
<span data-ttu-id="8a3db-131">Так как собрания по сути являются встречами, включающими участников, в примерах кода в этой статье показано, как создать повторяющиеся собрания.</span><span class="sxs-lookup"><span data-stu-id="8a3db-131">Because meetings are essentially appointments that include attendees, the code examples in this article show how to create recurring meetings.</span></span> <span data-ttu-id="8a3db-132">Если вы хотите создать повторяющуюся встречу, вы можете изменить примеры, удалив код, связанный с участниками.</span><span class="sxs-lookup"><span data-stu-id="8a3db-132">If you want to create a recurring appointment, you can modify the examples by removing code related to attendees.</span></span>
  
## <a name="create-a-recurring-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="8a3db-133">Создание повторяющегося собрания с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="8a3db-133">Create a recurring meeting by using the EWS Managed API</span></span>
<span data-ttu-id="8a3db-134"><a name="bk_CreateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8a3db-134"><a name="bk_CreateMtgEWSMA"> </a></span></span>

<span data-ttu-id="8a3db-135">В приведенном ниже примере кода показано, как создать повторяющееся собрание.</span><span class="sxs-lookup"><span data-stu-id="8a3db-135">The following code example shows how to create a recurring meeting.</span></span> <span data-ttu-id="8a3db-136">Сначала назначьте значения свойствам [объекта встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , используемого для создания собрания, а затем с помощью метода [сохранения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) сохраните серию в папке "Календарь" и отправьте приглашения на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="8a3db-136">First, assign values to the properties of an [Appointment object](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) used to create a meeting, then use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to save the recurring series to your calendar folder, and send meeting requests to your attendees.</span></span> <span data-ttu-id="8a3db-137">Наконец, используйте метод [встреча. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) для просмотра значений, заданных для шаблона повторения, который вы только что создали.</span><span class="sxs-lookup"><span data-stu-id="8a3db-137">Finally, use the [Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) method to look at the values set on the recurring master for the recurring series you just created.</span></span> 
  
<span data-ttu-id="8a3db-138">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="8a3db-138">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="8a3db-139">Метод, приведенный в этом примере, возвращает [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) повторяющегося образца повторяющейся серии.</span><span class="sxs-lookup"><span data-stu-id="8a3db-139">The method in this example returns the [item ID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the recurring series' recurring master.</span></span> 
  
```cs
public static ItemId CreateARecurringMeeting(ExchangeService service)
{        Appointment recurrMeeting = new Appointment(service);
        // Set the properties you need to create a meeting.
        recurrMeeting.Subject = "Weekly Update Meeting";
        recurrMeeting.Body = "Come hear about how the project is coming along!";
        recurrMeeting.Start = DateTime.Now.AddDays(1);
        recurrMeeting.End = recurrMeeting.Start.AddHours(1);
        recurrMeeting.Location = "Contoso Main Gallery";
        recurrMeeting.RequiredAttendees.Add("Mack@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Sadie@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Magdalena@contoso.com"); recurrMeeting.ReminderMinutesBeforeStart = 30;
             
        DayOfTheWeek[] dow = new DayOfTheWeek[] { (DayOfTheWeek)recurrMeeting.Start.DayOfWeek };
        // The following are the recurrence-specific properties for the meeting.
        recurrMeeting.Recurrence = new Recurrence.WeeklyPattern(recurrMeeting.Start.Date, 1, dow);
        recurrMeeting.Recurrence.StartDate = recurrMeeting.Start.Date;
        recurrMeeting.Recurrence.NumberOfOccurrences = 10;
        // This method results in in a CreateItem call to EWS.
        recurrMeeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
        // Retrieve the meeting subject and the properties that are set on a recurring master when a recurring series is created.
        recurrMeeting = Appointment.Bind(service, recurrMeeting.Id, new PropertySet(AppointmentSchema.Subject,
                                                                                    AppointmentSchema.AppointmentType, 
                                                                                    AppointmentSchema.Recurrence, 
                                                                                    AppointmentSchema.FirstOccurrence,
                                                                                    AppointmentSchema.LastOccurrence,
                                                                                    AppointmentSchema.ModifiedOccurrences,
                                                                                    AppointmentSchema.DeletedOccurrences));
        // Print out the recurring master properties.
        Console.WriteLine("\nAppointment created: " + recurrMeeting.Subject);
        Console.WriteLine("Appointment Type: {0}\n", recurrMeeting.AppointmentType);
        Console.WriteLine("These property values are always null unless the item is a recurring master:\n");
        Console.WriteLine("\tRecurrence pattern: {0}", recurrMeeting.Recurrence.ToString());
        Console.WriteLine("\tRecurring series start Date: {0}", recurrMeeting.Recurrence.StartDate.ToString());
        Console.WriteLine("\tRecurring series end Date: {0}", 
                        recurrMeeting.Recurrence.EndDate == null ? "Null" : recurrMeeting.Recurrence.EndDate.ToString());
        Console.WriteLine("\tHas end: {0}", recurrMeeting.Recurrence.HasEnd.ToString());
        Console.WriteLine("\tNumber of occurrances: {0}", recurrMeeting.Recurrence.NumberOfOccurrences);
        Console.WriteLine("\tLast 24 characters of the first occurrence's item ID:\t {0}", 
                        recurrMeeting.FirstOccurrence.ItemId.ToString().Substring(144));
        Console.WriteLine("\tLast 24 characters of the last occurrence's item ID:\t {0}", 
                        recurrMeeting.LastOccurrence.ItemId.ToString().Substring(144)); 
        Console.WriteLine("\tModified Occurrences: {0}", 
                        (recurrMeeting.ModifiedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString()));
        Console.WriteLine("\tDeleted Occurrences: {0}", 
                        recurrMeeting.DeletedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString());
        // Return the ID of the recurring master.
        return recurrMeeting.Id;
}

```

## <a name="create-a-recurring-meeting-by-using-ews"></a><span data-ttu-id="8a3db-140">Создание повторяющегося собрания с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="8a3db-140">Create a recurring meeting by using EWS</span></span>
<span data-ttu-id="8a3db-141"><a name="bk_CreateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="8a3db-141"><a name="bk_CreateMtgEWS"> </a></span></span>

<span data-ttu-id="8a3db-142">XML-код запроса и ответа в приведенных ниже примерах соответствует вызовам, выполняемым для [создания повторяющегося собрания с помощью управляемого API EWS](#bk_CreateMtgEWSMA).</span><span class="sxs-lookup"><span data-stu-id="8a3db-142">The request and response XML in the following examples correspond to calls made to [create a recurring meeting by using the EWS Managed API](#bk_CreateMtgEWSMA).</span></span> <span data-ttu-id="8a3db-143">Обратите внимание, что кроме установки значений, относящихся [к](http://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) повторению, запрос в основном такой же, как и для создания встречи с одним экземпляром.</span><span class="sxs-lookup"><span data-stu-id="8a3db-143">Note that other than setting recurrence-specific values on the [Recurrence](http://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) element, the request is essentially the same as one you would use to create a single-instance appointment.</span></span> <span data-ttu-id="8a3db-144">В следующем примере показан XML-код запроса при использовании операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания.</span><span class="sxs-lookup"><span data-stu-id="8a3db-144">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Weekly Update Meeting</t:Subject>
          <t:Body BodyType="HTML">Come hear about how the Organized Observational Paradigm SkyNet project is coming along!</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-08T13:21:32.868-08:00</t:Start>
          <t:End>2014-03-08T14:21:32.868-08:00</t:End>
          <t:Location>Contoso Main Gallery</t:Location>
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
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Saturday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-03-08-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="8a3db-145">В следующем примере показан XML-код отклика, возвращаемый операцией **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="8a3db-145">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
<span data-ttu-id="8a3db-146">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a3db-146">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="8a3db-147">В следующем примере показан XML-код запроса, который создается при использовании операции [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) и элемента **ItemId** для созданного ряда, а свойства запроса задаются только для повторяющегося образца, чтобы убедиться в том, что идентификатор **ItemId** , возвращенный сервером при создании повторяющихся рядов, предназначен для повторяющегося образца.</span><span class="sxs-lookup"><span data-stu-id="8a3db-147">The following example shows the request XML that is generated when you use the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation and the **ItemId** for the series you created, and request properties only set on a recurring master to confirm that the **ItemId** returned by the server when creating a recurring series is for a recurring master.</span></span> 
  
<span data-ttu-id="8a3db-148">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a3db-148">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Recurrence" />
          <t:FieldURI FieldURI="calendar:FirstOccurrence" />
          <t:FieldURI FieldURI="calendar:LastOccurrence" />
          <t:FieldURI FieldURI="calendar:ModifiedOccurrences" />
          <t:FieldURI FieldURI="calendar:DeletedOccurrences" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="8a3db-149">В следующем примере показан XML-код отклика, возвращенный операцией **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="8a3db-149">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
<span data-ttu-id="8a3db-150">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a3db-150">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
              <t:Subject>Weekly Update Meeting</t:Subject>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              <t:Recurrence>
                <t:WeeklyRecurrence>
                  <t:Interval>1</t:Interval>
                  <t:DaysOfWeek>Saturday</t:DaysOfWeek>
                </t:WeeklyRecurrence>
                <t:NumberedRecurrence>
                  <t:StartDate>2014-03-08-08:00</t:StartDate>
                  <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
                </t:NumberedRecurrence>
              </t:Recurrence>
              <t:FirstOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-03-08T21:21:00Z</t:Start>
                <t:End>2014-03-08T22:21:00Z</t:End>
                <t:OriginalStart>2014-03-08T21:21:00Z</t:OriginalStart>
              </t:FirstOccurrence>
              <t:LastOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-05-10T20:21:00Z</t:Start>
                <t:End>2014-05-10T21:21:00Z</t:End>
                <t:OriginalStart>2014-05-10T20:21:00Z</t:OriginalStart>
              </t:LastOccurrence>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="8a3db-151">См. также</span><span class="sxs-lookup"><span data-stu-id="8a3db-151">See also</span></span>


- [<span data-ttu-id="8a3db-152">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3db-152">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="8a3db-153">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8a3db-153">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="8a3db-154">Шаблоны повторения и EWS</span><span class="sxs-lookup"><span data-stu-id="8a3db-154">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="8a3db-155">Доступ к повторяющимся сериям с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3db-155">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8a3db-156">Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3db-156">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8a3db-157">Обновление серии повторяющихся данных с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="8a3db-157">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="8a3db-158">Обновление серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3db-158">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

