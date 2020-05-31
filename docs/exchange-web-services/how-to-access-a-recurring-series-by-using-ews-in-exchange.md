---
title: Доступ к повторяющимся сериям с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Узнайте, как получать доступ к элементам календаря в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 9f78ef5b51766a69d23fce3f36c55fbb9422fb16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760958"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="20487-103">Доступ к повторяющимся сериям с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="20487-103">Access a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="20487-104">Узнайте, как получать доступ к элементам календаря в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="20487-104">Learn how to access calendar items in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="20487-105">Повторяющиеся ряды встреч и собраний состоят из повторяющегося образца, числа повторений в серии, которые повторяются в соответствии с шаблоном набора, и (при необходимости) — с измененными и удаленными копиями.</span><span class="sxs-lookup"><span data-stu-id="20487-105">A recurring series of appointments or meetings is made up of a recurring master, a number of occurrences in a series that repeat according to a set pattern, and, optionally, sets of occurrences that were changed and that were deleted.</span></span> <span data-ttu-id="20487-106">Вы можете использовать управляемый API EWS или EWS для доступа к элементам календаря в повторяющихся рядах.</span><span class="sxs-lookup"><span data-stu-id="20487-106">You can use the EWS Managed API or EWS to access calendar items in a recurring series.</span></span> <span data-ttu-id="20487-107">Это позволяет:</span><span class="sxs-lookup"><span data-stu-id="20487-107">This enables you to:</span></span>
  
- <span data-ttu-id="20487-108">Проверьте, является ли элемент календаря, связанный с ИДЕНТИФИКАТОРом элемента, повторяющейся копией, вхождением в цикле или исключением из ряда.</span><span class="sxs-lookup"><span data-stu-id="20487-108">Check to see if a calendar item associated with an item ID is a recurring master, an occurrence in a series, or an exception to a series.</span></span>
    
- <span data-ttu-id="20487-109">Поиск повторяющихся встреч в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="20487-109">Search your calendar folder for recurrence appointments.</span></span>
    
- <span data-ttu-id="20487-110">Получение связанных элементов календаря повторения</span><span class="sxs-lookup"><span data-stu-id="20487-110">Get related recurrence calendar items</span></span>
    
- <span data-ttu-id="20487-111">Итерация по вхождениям в рядах, исключениях вхождений или удалении вхождений.</span><span class="sxs-lookup"><span data-stu-id="20487-111">Iterate through occurrences in a series, occurrence exceptions, or occurrence deletions.</span></span>
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="20487-112">Получение коллекции повторяющихся элементов календаря с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="20487-112">Get a collection of recurring calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="20487-113">Если вы хотите получить коллекцию встреч, можно использовать метод [ExchangeService. FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) для получения всех встреч между заданными начальной и конечной датами, а затем добавить все элементы календаря с типом "встреча **" или "** **исключение** " в коллекцию, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="20487-113">If you want to retrieve a collection of appointments, you can use the [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve all appointments between a given start and end date, and then add all calendar items with an appointment type of **Occurrence** or **Exception** to a collection, as shown in the following example.</span></span> 
  
<span data-ttu-id="20487-114">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="20487-114">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static Collection<Appointment> FindRecurringCalendarItems(ExchangeService service, 
                                                                    DateTime startSearchDate, 
                                                                    DateTime endSearchDate)
{
    // Instantiate a collection to hold occurrences and exception calendar items.
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a calendar view to search the calendar folder and specify the properties to return.
    CalendarView calView = new CalendarView(startSearchDate, endSearchDate);
    calView.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                            AppointmentSchema.Subject, 
                                            AppointmentSchema.Start, 
                                            AppointmentSchema.IsRecurring, 
                                            AppointmentSchema.AppointmentType);
    // Retrieve a collection of calendar items.
    FindItemsResults<Appointment> findResults = service.FindAppointments(WellKnownFolderName.Calendar, calView);
    // Add all calendar items in your view that are occurrences or exceptions to your collection.
    foreach (Appointment appt in findResults.Items)
    {
        if (appt.AppointmentType == AppointmentType.Occurrence || appt.AppointmentType == AppointmentType.Exception)
        {
            foundAppointments.Add(appt);
        }
        else
        {
            Console.WriteLine("Discarding calendar item of type {0}.", appt.AppointmentType);
        }
    }
    return foundAppointments;
}

```

<span data-ttu-id="20487-115">Обратите внимание, что повторяющиеся элементы основного календаря не возвращаются при вызове **FindAppointments**.</span><span class="sxs-lookup"><span data-stu-id="20487-115">Note that recurring master calendar items aren't returned in a call to **FindAppointments**.</span></span> <span data-ttu-id="20487-116">Если вы хотите извлечь повторяющиеся шаблоны или хотите использовать более общий подход к извлечению элементов календаря, необходимо использовать [ExchangeService. FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="20487-116">If you want to retrieve recurring masters, or you want a more general approach to retrieving calendar items, you need to use [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="20487-117">Затем можно использовать фильтр поиска, чтобы получить только те элементы, Дата начала которых больше или равна выбранному значению, и представление элемента, чтобы ограничить количество возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="20487-117">You can then use a search filter to retrieve only items with a start date greater than or equal to a date you choose, and an item view to limit the number of items to return.</span></span> <span data-ttu-id="20487-118">Обратите внимание, что повторяющаяся основная реплика с датой начала, предшествующей дате начала поиска, не будет найдена, даже если вхождения встречаются в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="20487-118">Note that a recurring master with a start date earlier than the start date in your search will not be found, even if occurrences occur in this range.</span></span>
  
<span data-ttu-id="20487-119">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="20487-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static Collection<Appointment> FindCalendarItemsByAppointmentType(ExchangeService service, 
                                                                         AppointmentType myAppointmentType, 
                                                                         DateTime startSearchDate)
{
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a search filter based on the start search date.
    SearchFilter.SearchFilterCollection searchFilter = new SearchFilter.SearchFilterCollection();
    searchFilter.Add(new SearchFilter.IsGreaterThanOrEqualTo(AppointmentSchema.Start, startSearchDate));
    // Create an item view to specify which properties to return.
    ItemView view = new ItemView(20);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                       AppointmentSchema.Subject, 
                                       AppointmentSchema.Start, 
                                       AppointmentSchema.AppointmentType,
                                       AppointmentSchema.IsRecurring);
    // Get the appointment items from the server with the properties we specified.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Calendar, searchFilter, view);
    // Add each of the appointments of the type you want to the collection.
    foreach (Item item in findResults.Items)
    {
        Appointment appt = item as Appointment;
        if (appt.AppointmentType == myAppointmentType)
        {
            foundAppointments.Add(appt);
        }
    }
    return foundAppointments;
}

```

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="20487-120">Получение связанных элементов календаря повторения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="20487-120">Get related recurrence calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="20487-121">Иногда у вас есть один элемент головоломки, но чтобы решить эту проблему, необходимо выполнить остальные части.</span><span class="sxs-lookup"><span data-stu-id="20487-121">Sometimes you have one piece of the puzzle, but to solve it you need the rest of the pieces.</span></span> <span data-ttu-id="20487-122">Если у вас есть идентификатор элемента календаря повторения, вы можете получить другие необходимые части, используя один из нескольких свойств или методов управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="20487-122">If you have the item ID for a recurrence calendar item, you can get the other pieces you need by using one of several EWS Managed API properties or methods.</span></span>
  
<span data-ttu-id="20487-123">**Таблица 1. Свойство или метод управляемого API EWS, используемые для получения связанных элементов календаря повторений**</span><span class="sxs-lookup"><span data-stu-id="20487-123">**Table 1. EWS Managed API property or method to use to get related recurrence calendar items**</span></span>

|<span data-ttu-id="20487-124">**Если у вас есть идентификатор элемента для...**</span><span class="sxs-lookup"><span data-stu-id="20487-124">**If you have the item ID for…**</span></span>|<span data-ttu-id="20487-125">**Вы можете получить...**</span><span class="sxs-lookup"><span data-stu-id="20487-125">**You can get…**</span></span>|<span data-ttu-id="20487-126">**С помощью метода...**</span><span class="sxs-lookup"><span data-stu-id="20487-126">**By using the…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="20487-127">Элемент повторяющегося основного календаря</span><span class="sxs-lookup"><span data-stu-id="20487-127">The recurring master calendar item</span></span>  <br/> | <span data-ttu-id="20487-128">Первое вхождение в серии</span><span class="sxs-lookup"><span data-stu-id="20487-128">The first occurrence in a series</span></span>  <br/>  <span data-ttu-id="20487-129">Последнее вхождение в серии</span><span class="sxs-lookup"><span data-stu-id="20487-129">The last occurrence in a series</span></span>  <br/>  <span data-ttu-id="20487-130">Исключения из серии</span><span class="sxs-lookup"><span data-stu-id="20487-130">The exceptions to a series</span></span>  <br/>  <span data-ttu-id="20487-131">Удаленные встречи в ряду</span><span class="sxs-lookup"><span data-stu-id="20487-131">The deleted appointments in a series</span></span>  <br/>  <span data-ttu-id="20487-132">Все вхождения (при наличии индекса)</span><span class="sxs-lookup"><span data-stu-id="20487-132">Any occurrence (given its index)</span></span>  <br/> |<span data-ttu-id="20487-133">Свойство [встреча. фирстоккурренце](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-133">[Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="20487-134">Свойство [встреча. ластоккурренце](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-134">[Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="20487-135">Свойство [встреча. модифиедоккурренцес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-135">[Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="20487-136">Свойство [встреча. делетедоккурренцес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-136">[Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="20487-137">Метод [встреча. биндтуккурренце](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-137">[Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="20487-138">Один экземпляр в ряду</span><span class="sxs-lookup"><span data-stu-id="20487-138">A single occurrence in a series</span></span>  <br/> |<span data-ttu-id="20487-139">Шаблон повторения</span><span class="sxs-lookup"><span data-stu-id="20487-139">The recurring master</span></span>  <br/> |<span data-ttu-id="20487-140">Метод [встреча. биндторекуррингмастер](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-140">[Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="20487-141">Любой элемент календаря (объект [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) )</span><span class="sxs-lookup"><span data-stu-id="20487-141">Any calendar item (an [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object)</span></span>  <br/> |<span data-ttu-id="20487-142">Значение перечисления [типа встреча](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-142">The [appointment type](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) enumeration value</span></span>  <br/> |<span data-ttu-id="20487-143">Свойство [встреча. аппоинтменттипе](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="20487-143">[Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) property</span></span>  <br/> |
   
<span data-ttu-id="20487-144">В приведенном ниже примере кода показано, как получить повторяющуюся основную страницу, первое или Последнее вхождение в ряду или вхождение, заданное индексом.</span><span class="sxs-lookup"><span data-stu-id="20487-144">The following code example shows how to get a recurring master, the first or last occurrence in a series, or an occurrence given its index.</span></span>
  
<span data-ttu-id="20487-145">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="20487-145">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static void GetRelatedRecurrenceCalendarItems(ExchangeService service, ItemId itemId)
{
    Appointment calendarItem = Appointment.Bind(service, itemId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    PropertySet props = new PropertySet(AppointmentSchema.AppointmentType,
                                        AppointmentSchema.Subject,
                                        AppointmentSchema.FirstOccurrence,
                                        AppointmentSchema.LastOccurrence,
                                        AppointmentSchema.ModifiedOccurrences,
                                        AppointmentSchema.DeletedOccurrences);
    // If the item ID is not for a recurring master, retrieve the recurring master for the series.
    switch (calendarItem.AppointmentType)
    {
        // Calendar item is a recurring master so use Appointment.Bind
        case AppointmentType.RecurringMaster:
            recurrMaster = Appointment.Bind(service, itemId, props);
            break;
        // The calendar item is a single instance meeting, so there are no instances to modify or delete.
        case AppointmentType.Single:
            Console.WriteLine("Item id must reference a calendar item that is part of a recurring series.");
            return;
        // The calendar item is an occurrence in the series, so use BindToRecurringMaster.
        case AppointmentType.Occurrence:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
        // The calendar item is an exception to the series, so use BindToRecurringMaster.                
        case AppointmentType.Exception:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
    }
    // View the first occurrence, last occurrence, and number of modified and deleted occurrences associated with the recurring master.
    Console.WriteLine("Information for the {0} recurring series:", recurrMaster.Subject);
    Console.WriteLine("The start time for the first appointment with id \t{0} was on \t{1}.", 
                        recurrMaster.FirstOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.FirstOccurrence.Start.ToString());
    Console.WriteLine("The start time for the last appointment with id \t{0} will be on \t{1}.", 
                        recurrMaster.LastOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.LastOccurrence.Start.ToString());
    Console.WriteLine("There are {0} modified occurrences and {1} deleted occurrences.", 
                        recurrMaster.ModifiedOccurrences == null ? "no" : recurrMaster.ModifiedOccurrences.Count.ToString(), 
                        recurrMaster.DeletedOccurrences == null ? "no" : recurrMaster.DeletedOccurrences.Count.ToString());
    // Bind to the first occurrence of a series by using its index.
    Appointment firstOccurrence = Appointment.BindToOccurrence(service, 
                                                                recurrMaster.Id, 
                                                                1, // Index of first item is 1, not 0.
                                                                new PropertySet(AppointmentSchema.AppointmentType,
                                                                                AppointmentSchema.Start));
    Console.WriteLine("Compare the start times for a recurring master's first occurrence " + 
                        "and the occurrence found at index 1 using the BindToOccurrence method:");
    Console.WriteLine("The appointment at index 1 has a start time of\t\t\t\t {0}\n" +
                        "Which matches that of the first occurrence on the recurring master: \t {1}",
                        firstOccurrence.Start.ToString(),
                        recurrMaster.FirstOccurrence.Start.ToString());
}

```

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a><span data-ttu-id="20487-146">Доступ к элементам календаря в повторяющихся рядах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="20487-146">Access calendar items in a recurring series by using EWS</span></span>

<span data-ttu-id="20487-147">Доступ к элементам календаря в повторяющихся рядах очень похож на доступ к отдельным экземплярам элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="20487-147">Accessing calendar items in a recurring series is very similar to accessing single instances of calendar items.</span></span> <span data-ttu-id="20487-148">Вы используете запрос операции [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , указав нужные свойства с помощью [оккурренцеитемид](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) экземпляра встречи.</span><span class="sxs-lookup"><span data-stu-id="20487-148">You use a [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request, specifying the properties you want, with the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) of the appointment instance you need.</span></span> <span data-ttu-id="20487-149">[Оккурренцеитемид](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) содержит **идентификатор элемента** повторяющейся основной реплики, а также значение индекса в ряду.</span><span class="sxs-lookup"><span data-stu-id="20487-149">The [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contains the **ItemID** of the occurrence's recurring master, as well as its index value in the series.</span></span> 
  
<span data-ttu-id="20487-150">В следующем XML-коде показан запрос [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , используемый для возврата вхождения в серии, указанной по индексу.</span><span class="sxs-lookup"><span data-stu-id="20487-150">The following XML shows the [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) request used to return an occurrence in a series specified by its index.</span></span> <span data-ttu-id="20487-151">Обратите внимание, что **идентификатор элемента** повторяющейся основной реплики был сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20487-151">Note that the **ItemID** of the recurring master has been shortened for readability.</span></span> 
  
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
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Start" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkA" InstanceIndex="1" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="20487-152">Сервер отвечает на запрос **GetItem** с сообщением [жетитемреспонсе](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **, которое**указывает на то, что сообщение было создано успешно, и идентификатор элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) вновь созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="20487-152">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="20487-153">См. также</span><span class="sxs-lookup"><span data-stu-id="20487-153">See also</span></span>


- [<span data-ttu-id="20487-154">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="20487-154">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
- [<span data-ttu-id="20487-155">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="20487-155">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

