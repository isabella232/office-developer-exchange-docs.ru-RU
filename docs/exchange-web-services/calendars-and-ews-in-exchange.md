---
title: Календари и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Сведения о календарях, папках календарей и элементах, встречах и собраниях в Exchange.
localization_priority: Priority
ms.openlocfilehash: 3312ebb4deeb6645ccd7048564d61c3db5ea4b94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456201"
---
# <a name="calendars-and-ews-in-exchange"></a><span data-ttu-id="b8c1e-103">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-103">Calendars and EWS in Exchange</span></span>

<span data-ttu-id="b8c1e-104">Сведения о календарях, папках календарей и элементах, встречах и собраниях в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-104">Learn about calendars, calendar folders and items, appointments, and meetings in Exchange.</span></span>
  
<span data-ttu-id="b8c1e-105">Вы, вероятно, знакомы с многими возможностями календаря в почтовых клиентах, таких как Outlook, которые позволяют отслеживать встречи, планировать собрания, проверять доступность людей, приглашать участников, а также изменять или отменять собрания.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-105">You're probably familiar with many of the calendar features in email clients like Outlook, which enable you to track appointments, schedule meetings, check people's availability, invite attendees, and change or cancel meetings.</span></span>
  
<span data-ttu-id="b8c1e-106">Функции, связанные с календарем, в Exchange немного отличаются от того, что вы видите в клиенте, например Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-106">Calendar-related features in Exchange are a little different than what you see in a client like Outlook.</span></span> <span data-ttu-id="b8c1e-107">Вместо того чтобы отображать информацию, EWS в Exchange позволяет выполнять такие задачи, как создание, хранение, отправка и изменение сведений.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-107">Instead of displaying information, EWS in Exchange enables you to do things like create, store, send, or change information.</span></span> <span data-ttu-id="b8c1e-108">Чтобы использовать EWS для работы с календарями, вам необходимо ознакомиться с такими понятиями, как хранение информации, время, повторение и обмен сообщениями.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-108">To use EWS to work with calendars, you'll need to be familiar with concepts such as information storage, time, recurrence, and message flow.</span></span> <span data-ttu-id="b8c1e-109">Точнее, вам потребуется ознакомиться со следующими сведениями:</span><span class="sxs-lookup"><span data-stu-id="b8c1e-109">More specifically, you'll need to be familiar with the following:</span></span>
  
- <span data-ttu-id="b8c1e-110">Папки календаря, элементы календаря и представления календаря</span><span class="sxs-lookup"><span data-stu-id="b8c1e-110">Calendar folders, calendar items, and calendar views</span></span>
    
- <span data-ttu-id="b8c1e-111">Приглашения на собрания, ответы, планирование, участники, ресурсы, комнаты и доступность</span><span class="sxs-lookup"><span data-stu-id="b8c1e-111">Meeting requests, responses, scheduling, attendees, resources, rooms, and availability</span></span>
    
- <span data-ttu-id="b8c1e-112">Длительность времени, часовые пояса и время начала и окончания собраний и встреч</span><span class="sxs-lookup"><span data-stu-id="b8c1e-112">Time durations, time zones, and start and end times of meetings and appointments</span></span>
    
- <span data-ttu-id="b8c1e-113">Повторяющиеся ряды, шаблоны повторения, исключения и отдельные экземпляры встречи и собрания</span><span class="sxs-lookup"><span data-stu-id="b8c1e-113">Recurring series, recurrence patterns, exceptions, and single instance appointments and meetings</span></span>
    
<span data-ttu-id="b8c1e-114">К счастью, EWS и управляемый API EWS предоставляют богатый набор операций и методов, позволяющих выполнять широкий спектр задач, связанных с календарем.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-114">Fortunately, EWS and the EWS Managed API provide a rich set of operations and methods that enable you to perform a wide range of calendar-related tasks.</span></span> <span data-ttu-id="b8c1e-115">Например, с помощью управляемого API EWS вы можете создать собрание и отправить приглашения участникам с помощью всего нескольких строк кода, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-115">For example, using the EWS Managed API, you can create a meeting and send invitations to attendees with just a few lines of code, as shown in the following example.</span></span>
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a><span data-ttu-id="b8c1e-116">Папки календаря и элементы календаря</span><span class="sxs-lookup"><span data-stu-id="b8c1e-116">Calendar folders and calendar items</span></span>
<span data-ttu-id="b8c1e-117"><a name="bk_CalendarFolder"> </a></span><span class="sxs-lookup"><span data-stu-id="b8c1e-117"><a name="bk_CalendarFolder"> </a></span></span>

<span data-ttu-id="b8c1e-118">Папки календаря содержат элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-118">Calendar folders contain calendar items.</span></span> <span data-ttu-id="b8c1e-119">Папки календаря имеют [класс Folder](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) объекта **IPF. Встреча**и может включать только те элементы, которые определены свойством управляемого API [ItemClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS, связанным с объектом [класса встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , или элементом EWS [календаритемтипе](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b8c1e-119">Calendar folders have a [folder class](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) of **IPF.Appointment**, and can include only the items defined by the [ItemClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API property, which is associated with an [Appointment Class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, or the EWS [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="b8c1e-120">Элементы в папке "Календарь" немного отличаются от элементов в других папках почтового ящика, так как повторения в повторяющихся рядах и исключения в повторяющихся рядах не являются фактическими элементами в почтовом ящике, а хранятся внутренне как вложения в повторяющейся основной реплике.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-120">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="b8c1e-121">Таким образом, чтобы получить все встречи в заданном диапазоне дат, необходимо использовать представление "Календарь".</span><span class="sxs-lookup"><span data-stu-id="b8c1e-121">Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view.</span></span> <span data-ttu-id="b8c1e-122">Чтобы узнать больше об извлечении встреч и представлений календаря, ознакомьтесь со [статьей получение встреч и собраний с помощью EWS в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b8c1e-122">To learn more about retrieving appointments and calendar views, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="meetings-and-appointments"></a><span data-ttu-id="b8c1e-123">Собрания и встречи</span><span class="sxs-lookup"><span data-stu-id="b8c1e-123">Meetings and appointments</span></span>
<span data-ttu-id="b8c1e-124"><a name="bk_meetings"> </a></span><span class="sxs-lookup"><span data-stu-id="b8c1e-124"><a name="bk_meetings"> </a></span></span>

<span data-ttu-id="b8c1e-125">Существенным различием между собраниями и встречами является то, что собрания имеют участников, а встречи — нет.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-125">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="b8c1e-126">На внутреннем сервере Exchange использует один и тот же объект для собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-126">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="b8c1e-127">Для работы с собраниями и встречами используется [класс встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) управляемого API EWS или элемент EWS [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b8c1e-127">You use the EWS Managed API [Appointment class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="b8c1e-128">Встречи и собрания могут быть отдельными экземплярами или частью [повторяющихся рядов](recurrence-patterns-and-ews.md), но так как встречи не включают участников, комнаты или ресурсы, им не требуется отправлять сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-128">Both appointments and meetings can be single instances or part of a [recurring series](recurrence-patterns-and-ews.md), but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span>
  
<span data-ttu-id="b8c1e-129">Так как собрания включают в себя отправку и реагирование на запросы и обновления, они используют не только доступ к элементам в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="b8c1e-129">Because meetings include sending and responding to requests and updates, they involve more than just accessing items in a Calendar folder.</span></span> <span data-ttu-id="b8c1e-130">У них также есть связанный рабочий процесс.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-130">They also have an associated workflow.</span></span> <span data-ttu-id="b8c1e-131">Собрания должны быть запланированы, когда доступны участники, и может также включать резервирование комнаты для собраний или ресурсы, такие как проектор или другое оборудование.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-131">Meetings must be scheduled when attendees are available, and can also involve reserving a meeting room, or resources such as a projector or other equipment.</span></span>
  
<span data-ttu-id="b8c1e-132">Рабочий процесс для собраний обычно состоит из следующих этапов:</span><span class="sxs-lookup"><span data-stu-id="b8c1e-132">The meeting workflow typically involves the following steps:</span></span>
  
1. <span data-ttu-id="b8c1e-133">Собрание создается и заполняется такими сведениями, как время начала и окончания, расположение и текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-133">A meeting is created and populated with information such as start and end time, location, and a message body.</span></span>
    
2. <span data-ttu-id="b8c1e-134">Создается список потенциальных участников, ресурсов и комнат.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-134">A list of prospective attendees, resources, and rooms is created.</span></span>
    
3. <span data-ttu-id="b8c1e-135">Выбрано состояние доступности участников.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-135">The availability status of attendees is checked.</span></span> 
    
4. <span data-ttu-id="b8c1e-136">Приглашение на собрание отправляется участникам.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-136">A meeting request is sent to attendees.</span></span>
    
5. <span data-ttu-id="b8c1e-137">Участники отвечают на собрание с намерением принять участие или нет.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-137">Attendees reply to the meeting with their intention to attend or not.</span></span> <span data-ttu-id="b8c1e-138">Участники могут также предложить новое время собрания.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-138">Attendees may also propose a new time for the meeting.</span></span>
    
6. <span data-ttu-id="b8c1e-139">Собрания могут быть отменены или обновлены, что обычно вызывает отправку новых сообщений участникам.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-139">Meetings can be canceled or updated, which typically trigger new messages to be sent to attendees.</span></span>
    
## <a name="calendars-and-time"></a><span data-ttu-id="b8c1e-140">Календари и время</span><span class="sxs-lookup"><span data-stu-id="b8c1e-140">Calendars and time</span></span>
<span data-ttu-id="b8c1e-141"><a name="bk_Time"> </a></span><span class="sxs-lookup"><span data-stu-id="b8c1e-141"><a name="bk_Time"> </a></span></span>

<span data-ttu-id="b8c1e-142">Функции, связанные со временем, являются неотъемлемой частью календаря.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-142">Time-related functionality is integral to calendaring.</span></span> <span data-ttu-id="b8c1e-143">Встречи и собрания имеют время начала и окончания, продолжительность и другие связанные с временем свойства, такие как время создания, отправки и получения сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-143">Appointments and meetings have start and end times, durations, and other time-related properties, such as the time at which a message is created, sent, and received.</span></span> <span data-ttu-id="b8c1e-144">Существующие встречи и собрания можно получить из папки "Календарь" на основе времени начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-144">Existing appointments and meetings can be retrieved from a Calendar folder based on a start and end time.</span></span> <span data-ttu-id="b8c1e-145">Повторяющиеся ряды начинаются и заканчиваются.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-145">Recurring series have beginnings and ends.</span></span> <span data-ttu-id="b8c1e-146">Собрания выполняются в заданном часовом поясе, что является все более важным в глобальной экономике.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-146">And meetings occur within a given time zone, which is increasingly important in a global economy.</span></span>
  
<span data-ttu-id="b8c1e-147">Значения времени хранятся внутренним образом на сервере Exchange в формате всемирного координированного времени (UTC).</span><span class="sxs-lookup"><span data-stu-id="b8c1e-147">Times are stored internally on an Exchange server in Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="b8c1e-148">Exchange преобразует их в местный часовой пояс на основе параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-148">Exchange converts them to local time zone based on client settings.</span></span> <span data-ttu-id="b8c1e-149">Свойства [DateTime](https://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) ограничены локальным часовым поясом компьютера.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-149">[DateTime](https://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) properties are scoped to the computer's local time zone.</span></span> 
  
## <a name="recurring-series"></a><span data-ttu-id="b8c1e-150">Ряд повторяющихся данных</span><span class="sxs-lookup"><span data-stu-id="b8c1e-150">Recurring series</span></span>
<span data-ttu-id="b8c1e-151"><a name="bk_recurrence"> </a></span><span class="sxs-lookup"><span data-stu-id="b8c1e-151"><a name="bk_recurrence"> </a></span></span>

<span data-ttu-id="b8c1e-152">Повторяющиеся ряды встреч и собраний состоят из повторяющегося образца, набора элементов вхождения и (необязательно) набора элементов исключения.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-152">A recurring series of appointments or meetings is comprised of a recurring master, a set of occurrence items, and optionally, a set of exception items.</span></span> <span data-ttu-id="b8c1e-153">Сведения о повторении хранятся в повторяющемся элементе шаблона.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-153">Recurrence information is stored on the recurring master item.</span></span> <span data-ttu-id="b8c1e-154">Элемент [рекуррингмастеритемид](https://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS связан с вхождениями и исключениями в ряду, или можно использовать метод [встречи. биндторекуррингмастер](https://msdn.microsoft.com/library/dd635978%28v=EXCHG.80%29.aspx) , управляемый API EWS, для получения основной реплики.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-154">The [RecurringMasterItemId](https://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS element is associated with occurrences and exceptions in a series, or you can use the [Appointment.BindToRecurringMaster](https://msdn.microsoft.com/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API method to get the recurring master.</span></span> <span data-ttu-id="b8c1e-155">С помощью экземпляра ряда можно найти все элементы и сведения, связанные с серией.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-155">Using an instance of a series, you can find all the elements and information associated with the series.</span></span> 
  
<span data-ttu-id="b8c1e-156">Обратите внимание, что свойства повторения существуют для всех элементов календаря, но они заполняются только для повторяющихся элементов шаблона.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-156">Note that recurrence properties exist on all calendar items, but they are populated only on recurring master items.</span></span> <span data-ttu-id="b8c1e-157">В дополнение к индексу всех вхождений в ряду, повторяющееся эталонное руководство содержит ссылку на измененные и удаленные экземпляры, а также расписание повторения ряда (например, ежедневно, еженедельно, ежемесячно или ежегодно).</span><span class="sxs-lookup"><span data-stu-id="b8c1e-157">In addition to an index of all occurrences in a series, the recurring master has a reference to modified and deleted occurrences and the recurrence pattern of a series (for example, daily, weekly, monthly, or yearly).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="b8c1e-158">В этой статье</span><span class="sxs-lookup"><span data-stu-id="b8c1e-158">In this section</span></span>
<span data-ttu-id="b8c1e-159"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="b8c1e-159"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="b8c1e-160">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b8c1e-160">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="b8c1e-161">Создание событий на целый день с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-161">Create all-day events by using EWS in Exchange</span></span>](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-162">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-163">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-164">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-165">Получение списков помещений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-165">Get room lists by using EWS in Exchange</span></span>](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-166">Получение сведений о доступности с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-166">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-167">Предложение нового времени проведения собрания с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-167">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-168">Обработка элементов календаря в пакетах Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-168">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-169">Шаблоны повторения и EWS</span><span class="sxs-lookup"><span data-stu-id="b8c1e-169">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="b8c1e-170">См. также</span><span class="sxs-lookup"><span data-stu-id="b8c1e-170">See also</span></span>


- [<span data-ttu-id="b8c1e-171">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="b8c1e-172">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-172">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="b8c1e-173">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-173">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

