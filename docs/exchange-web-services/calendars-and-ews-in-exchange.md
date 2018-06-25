---
title: Календари и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Узнайте о календарей, папкам календаря и элементов, встречи и собрания в Exchange.
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760934"
---
# <a name="calendars-and-ews-in-exchange"></a><span data-ttu-id="dae53-103">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-103">Calendars and EWS in Exchange</span></span>

<span data-ttu-id="dae53-104">Узнайте о календарей, папкам календаря и элементов, встречи и собрания в Exchange.</span><span class="sxs-lookup"><span data-stu-id="dae53-104">Learn about calendars, calendar folders and items, appointments, and meetings in Exchange.</span></span>
  
<span data-ttu-id="dae53-105">Возможно, вы знакомы с многие функции календаря в клиентов электронной почты, как Outlook, которые позволяют отслеживать встречи, планировать собрания, проверьте доступность людей, пригласить участников и изменение или Отмена собрания.</span><span class="sxs-lookup"><span data-stu-id="dae53-105">You're probably familiar with many of the calendar features in email clients like Outlook, which enable you to track appointments, schedule meetings, check people's availability, invite attendees, and change or cancel meetings.</span></span>
  
<span data-ttu-id="dae53-106">Возможности, связанные с календарем в Exchange, немного отличаются от в клиентом, например Outlook.</span><span class="sxs-lookup"><span data-stu-id="dae53-106">Calendar-related features in Exchange are a little different than what you see in a client like Outlook.</span></span> <span data-ttu-id="dae53-107">Вместо отображения данных, веб-служб Exchange в Exchange позволяет выполнять такие действия, как создание, хранить, отправлять или изменить сведения.</span><span class="sxs-lookup"><span data-stu-id="dae53-107">Instead of displaying information, EWS in Exchange enables you to do things like create, store, send, or change information.</span></span> <span data-ttu-id="dae53-108">Чтобы использовать веб-служб Exchange для работы с календарями, необходимо ознакомиться с понятиями, таких как сведения о хранилище, время, повторения и поток сообщений.</span><span class="sxs-lookup"><span data-stu-id="dae53-108">To use EWS to work with calendars, you'll need to be familiar with concepts such as information storage, time, recurrence, and message flow.</span></span> <span data-ttu-id="dae53-109">В частности необходимо ознакомиться со следующими:</span><span class="sxs-lookup"><span data-stu-id="dae53-109">More specifically, you'll need to be familiar with the following:</span></span>
  
- <span data-ttu-id="dae53-110">Папки календаря, элементы календаря и представления календаря</span><span class="sxs-lookup"><span data-stu-id="dae53-110">Calendar folders, calendar items, and calendar views</span></span>
    
- <span data-ttu-id="dae53-111">Приглашения на собрания, ответы, планирования, участников, ресурсы, комнат и доступности</span><span class="sxs-lookup"><span data-stu-id="dae53-111">Meeting requests, responses, scheduling, attendees, resources, rooms, and availability</span></span>
    
- <span data-ttu-id="dae53-112">Продолжительность времени, часовые пояса и времени начала и окончания собрания и встречи</span><span class="sxs-lookup"><span data-stu-id="dae53-112">Time durations, time zones, and start and end times of meetings and appointments</span></span>
    
- <span data-ttu-id="dae53-113">Ряд повторяющейся, шаблоны повторения, исключения и одиночных встреч и собраний</span><span class="sxs-lookup"><span data-stu-id="dae53-113">Recurring series, recurrence patterns, exceptions, and single instance appointments and meetings</span></span>
    
<span data-ttu-id="dae53-114">К счастью веб-служб Exchange и управляемый API EWS обеспечивают широкий набор операций и методы, которые позволяют выполнять множество задач, связанных с календаря.</span><span class="sxs-lookup"><span data-stu-id="dae53-114">Fortunately, EWS and the EWS Managed API provide a rich set of operations and methods that enable you to perform a wide range of calendar-related tasks.</span></span> <span data-ttu-id="dae53-115">Например с помощью управляемого интерфейса API веб-служб Exchange, можно организовать собрание и отправлять приглашения на собрания с помощью нескольких строк кода, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="dae53-115">For example, using the EWS Managed API, you can create a meeting and send invitations to attendees with just a few lines of code, as shown in the following example.</span></span>
  
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

## <a name="calendar-folders-and-calendar-items"></a><span data-ttu-id="dae53-116">Папки календаря и элементы календаря</span><span class="sxs-lookup"><span data-stu-id="dae53-116">Calendar folders and calendar items</span></span>
<span data-ttu-id="dae53-117"><a name="bk_CalendarFolder"> </a></span><span class="sxs-lookup"><span data-stu-id="dae53-117"></span></span>

<span data-ttu-id="dae53-118">Папки календаря содержат элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="dae53-118">Calendar folders contain calendar items.</span></span> <span data-ttu-id="dae53-119">Папки календаря имеют [папки класс](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) **IPF. Встреча**и может содержать только элементы, определенные в свойстве управляемый API EWS [ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) , связанной с объектом [Класса встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="dae53-119">Calendar folders have a [folder class](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) of **IPF.Appointment**, and can include only the items defined by the [ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API property, which is associated with an [Appointment Class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, or the EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="dae53-120">Элементов в папке календаря являются немного отличаться от элементов в других папках в почтовый ящик, поскольку вхождений в ряду и исключения из серии повторяющихся не фактические элементов в почтовом ящике, но вместо хранятся во внутренней сети, в виде вложений повторяющейся Образец.</span><span class="sxs-lookup"><span data-stu-id="dae53-120">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="dae53-121">Таким образом Чтобы получить все встречи в определенный период, необходимо использовать календарном представлении.</span><span class="sxs-lookup"><span data-stu-id="dae53-121">Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view.</span></span> <span data-ttu-id="dae53-122">Дополнительные сведения о получении встреч и представления календаря видеть [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="dae53-122">To learn more about retrieving appointments and calendar views, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="meetings-and-appointments"></a><span data-ttu-id="dae53-123">Собрания и встречи</span><span class="sxs-lookup"><span data-stu-id="dae53-123">Meetings and appointments</span></span>
<span data-ttu-id="dae53-124"><a name="bk_meetings"> </a></span><span class="sxs-lookup"><span data-stu-id="dae53-124"></span></span>

<span data-ttu-id="dae53-125">Важные различия между собраний и встреч —, что у участников собрания, а не встреч.</span><span class="sxs-lookup"><span data-stu-id="dae53-125">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="dae53-126">Для внутреннего использования Exchange использует тот же объект для собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="dae53-126">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="dae53-127">Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для работы с собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="dae53-127">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="dae53-128">Встречи и собрания могут быть отдельные экземпляры или частью [серии повторяющихся](recurrence-patterns-and-ews.md), но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="dae53-128">Both appointments and meetings can be single instances or part of a [recurring series](recurrence-patterns-and-ews.md), but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span>
  
<span data-ttu-id="dae53-129">Так как собраний отправки и отвечать на запросы и обновления, они включают в себя больше, чем просто доступ к элементов в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="dae53-129">Because meetings include sending and responding to requests and updates, they involve more than just accessing items in a Calendar folder.</span></span> <span data-ttu-id="dae53-130">Они также могут связанного рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="dae53-130">They also have an associated workflow.</span></span> <span data-ttu-id="dae53-131">Необходимо запланировать собрания, если участники доступны и может также включать в себя резервирование конференц-зала или ресурсов, таких как проектор или другого оборудования.</span><span class="sxs-lookup"><span data-stu-id="dae53-131">Meetings must be scheduled when attendees are available, and can also involve reserving a meeting room, or resources such as a projector or other equipment.</span></span>
  
<span data-ttu-id="dae53-132">Рабочий процесс собрания обычно состоит из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="dae53-132">The meeting workflow typically involves the following steps:</span></span>
  
1. <span data-ttu-id="dae53-133">Собрания созданы и заполнены с начала и время окончания, расположение и текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="dae53-133">A meeting is created and populated with information such as start and end time, location, and a message body.</span></span>
    
2. <span data-ttu-id="dae53-134">Создать список потенциальных участников, ресурсы и комнаты.</span><span class="sxs-lookup"><span data-stu-id="dae53-134">A list of prospective attendees, resources, and rooms is created.</span></span>
    
3. <span data-ttu-id="dae53-135">Проверяется состояние доступности участников.</span><span class="sxs-lookup"><span data-stu-id="dae53-135">The availability status of attendees is checked.</span></span> 
    
4. <span data-ttu-id="dae53-136">Приглашения на собрание отправляется участников.</span><span class="sxs-lookup"><span data-stu-id="dae53-136">A meeting request is sent to attendees.</span></span>
    
5. <span data-ttu-id="dae53-137">Участники ответ на собрание с выполняемое посещение или нет.</span><span class="sxs-lookup"><span data-stu-id="dae53-137">Attendees reply to the meeting with their intention to attend or not.</span></span> <span data-ttu-id="dae53-138">Участники могут также предложить новое время собрания.</span><span class="sxs-lookup"><span data-stu-id="dae53-138">Attendees may also propose a new time for the meeting.</span></span>
    
6. <span data-ttu-id="dae53-139">Собрания можно остановить или обновления, который обычно запуск новых сообщений, отправляемых участникам.</span><span class="sxs-lookup"><span data-stu-id="dae53-139">Meetings can be canceled or updated, which typically trigger new messages to be sent to attendees.</span></span>
    
## <a name="calendars-and-time"></a><span data-ttu-id="dae53-140">Календари и времени</span><span class="sxs-lookup"><span data-stu-id="dae53-140">Calendars and time</span></span>
<span data-ttu-id="dae53-141"><a name="bk_Time"> </a></span><span class="sxs-lookup"><span data-stu-id="dae53-141"></span></span>

<span data-ttu-id="dae53-142">Функции, связанные с временем включается ведение календаря.</span><span class="sxs-lookup"><span data-stu-id="dae53-142">Time-related functionality is integral to calendaring.</span></span> <span data-ttu-id="dae53-143">Встречи и собрания иметь начала и окончания, длительности и другие свойства, связанные с времени, например, время создания, отправки и получения сообщения.</span><span class="sxs-lookup"><span data-stu-id="dae53-143">Appointments and meetings have start and end times, durations, and other time-related properties, such as the time at which a message is created, sent, and received.</span></span> <span data-ttu-id="dae53-144">Существующие встречи и собрания могут быть получены из папки календаря на основе времени начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="dae53-144">Existing appointments and meetings can be retrieved from a Calendar folder based on a start and end time.</span></span> <span data-ttu-id="dae53-145">Повторяющееся иметь основные компоненты и заканчивается.</span><span class="sxs-lookup"><span data-stu-id="dae53-145">Recurring series have beginnings and ends.</span></span> <span data-ttu-id="dae53-146">И собраний в пределах указанной часовой пояс, который является очень важно в глобальной экономики.</span><span class="sxs-lookup"><span data-stu-id="dae53-146">And meetings occur within a given time zone, which is increasingly important in a global economy.</span></span>
  
<span data-ttu-id="dae53-147">Время хранятся во внутренней сети на сервере Exchange server в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="dae53-147">Times are stored internally on an Exchange server in Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="dae53-148">Exchange преобразует их в локальный часовой пояс, на основе параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="dae53-148">Exchange converts them to local time zone based on client settings.</span></span> <span data-ttu-id="dae53-149">Свойства [даты и времени](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) распространяются локального часового пояса.</span><span class="sxs-lookup"><span data-stu-id="dae53-149">[DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) properties are scoped to the computer's local time zone.</span></span> 
  
## <a name="recurring-series"></a><span data-ttu-id="dae53-150">Повторяющееся</span><span class="sxs-lookup"><span data-stu-id="dae53-150">Recurring series</span></span>
<span data-ttu-id="dae53-151"><a name="bk_recurrence"> </a></span><span class="sxs-lookup"><span data-stu-id="dae53-151"></span></span>

<span data-ttu-id="dae53-152">Ряд повторяющейся встречи или собрания включает в себя образцом повторения набора элементов вхождение и при необходимости набора элементов исключение.</span><span class="sxs-lookup"><span data-stu-id="dae53-152">A recurring series of appointments or meetings is comprised of a recurring master, a set of occurrence items, and optionally, a set of exception items.</span></span> <span data-ttu-id="dae53-153">Сведения о повторения хранятся на повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="dae53-153">Recurrence information is stored on the recurring master item.</span></span> <span data-ttu-id="dae53-154">Элемент веб-служб Exchange [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) связан с вхождений и исключений из серии, или можно использовать метод веб-служб Exchange [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) управляемого интерфейса API для получения регулярное главной.</span><span class="sxs-lookup"><span data-stu-id="dae53-154">The [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS element is associated with occurrences and exceptions in a series, or you can use the [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API method to get the recurring master.</span></span> <span data-ttu-id="dae53-155">С помощью экземпляра ряда, можно найти все элементы и сведения, связанные с серии.</span><span class="sxs-lookup"><span data-stu-id="dae53-155">Using an instance of a series, you can find all the elements and information associated with the series.</span></span> 
  
<span data-ttu-id="dae53-156">Обратите внимание на то, что повторения свойства существуют во всех элементах календаря, но записываются только на повторяющиеся основные элементы.</span><span class="sxs-lookup"><span data-stu-id="dae53-156">Note that recurrence properties exist on all calendar items, but they are populated only on recurring master items.</span></span> <span data-ttu-id="dae53-157">Помимо индекса все вхождения из серии повторяющихся главных содержит ссылку на измененные и удаленные вхождений и повторов рядов (например, ежедневно, еженедельно, ежемесячно или ежегодно).</span><span class="sxs-lookup"><span data-stu-id="dae53-157">In addition to an index of all occurrences in a series, the recurring master has a reference to modified and deleted occurrences and the recurrence pattern of a series (for example, daily, weekly, monthly, or yearly).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="dae53-158">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="dae53-158">In this section</span></span>
<span data-ttu-id="dae53-159"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="dae53-159"></span></span>

- [<span data-ttu-id="dae53-160">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="dae53-160">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="dae53-161">Создание событий на целый день с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-161">Create all-day events by using EWS in Exchange</span></span>](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-162">Получение встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-163">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-164">Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-165">Получить список помещений с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-165">Get room lists by using EWS in Exchange</span></span>](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-166">Получение сведений о доступности с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-166">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-167">Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-167">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dae53-168">В Exchange обработки элементов календаря в пакетах</span><span class="sxs-lookup"><span data-stu-id="dae53-168">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="dae53-169">Шаблоны повторения и веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-169">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="dae53-170">См. также</span><span class="sxs-lookup"><span data-stu-id="dae53-170">See also</span></span>


- [<span data-ttu-id="dae53-171">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="dae53-172">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-172">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="dae53-173">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="dae53-173">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

