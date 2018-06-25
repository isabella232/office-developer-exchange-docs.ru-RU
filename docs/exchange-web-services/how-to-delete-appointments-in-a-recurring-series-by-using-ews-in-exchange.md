---
title: Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Узнайте, как удаление встреч в серии повторяющихся с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761018"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="38793-103">Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="38793-104">Узнайте, как удаление встреч в серии повторяющихся с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="38793-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="38793-105">Чтобы удалить ряд встречи или собрания или только один экземпляр из серии можно использовать управляемый API EWS или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="38793-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="38793-106">Процесс, который используется для удаления всего ряда практически не то же, что процесс, который используется для удаления только одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="38793-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="38793-107">Используйте одинаковые методы управляемый API EWS или операции EWS, используемые для [удаления одного экземпляра встречи или собрания](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="38793-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="38793-108">Отличие заключается в идентификатор, который включен в метод или операции.</span><span class="sxs-lookup"><span data-stu-id="38793-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="38793-109">Давайте начнем, посмотрев как оба сценария, совпадают.</span><span class="sxs-lookup"><span data-stu-id="38793-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="38793-110">Чтобы удалить серии повторяющихся или одно вхождение в ряду, необходимо найти копию, или серии, которую требуется удалить, а затем вызвать соответствующий метод или операцию, чтобы удалить его.</span><span class="sxs-lookup"><span data-stu-id="38793-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="38793-111">В то время как можно просто удалить любой тип встречи, рекомендуется хранить участников собрания или организатора и отмены собраний, организованных пользователем и отклонение собрания, которые не были организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="38793-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="38793-112">Так как отличаются сценарии?</span><span class="sxs-lookup"><span data-stu-id="38793-112">So how are the scenarios different?</span></span> <span data-ttu-id="38793-113">Он все о [встрече](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) объект, используемый для вызова метода (для управляемого API EWS) или идентификатор элемента включен в операции запроса (EWS).</span><span class="sxs-lookup"><span data-stu-id="38793-113">It's all about the [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="38793-114">Для удаления всей серии, требуется идентификатор объекта или элемента **встречи** образца повторения.</span><span class="sxs-lookup"><span data-stu-id="38793-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="38793-115">Для удаления одного экземпляра, требуется идентификатор объекта или элемента **встречи** этот экземпляр.</span><span class="sxs-lookup"><span data-stu-id="38793-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="38793-116">Удаление повторяющейся встречи с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="38793-117">В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="38793-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="38793-118">Параметр _recurringItem_ является объектом **встречи** для повторяющихся основной или одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="38793-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="38793-119">Параметр _deleteEntireSeries_ указывает, следует ли удалить всю последовательность, которая является частью процессов _recurringItem_ .</span><span class="sxs-lookup"><span data-stu-id="38793-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

<span data-ttu-id="38793-120">Для использования в этом примере, чтобы [присоединить вхождения или повторяющихся главных](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)и передачи результирующего объекта **встречи** в метод.</span><span class="sxs-lookup"><span data-stu-id="38793-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="38793-121">Имейте в виду, что при доступе к встречи с помощью класса [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , полученные их все вхождения одной.</span><span class="sxs-lookup"><span data-stu-id="38793-121">Keep in mind that if you access appointments by using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="38793-122">И наоборот Если вы используете класс [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , результирующий элементы, всех повторяющихся образцов.</span><span class="sxs-lookup"><span data-stu-id="38793-122">Conversely, if you use the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="38793-123">Удаление повторяющейся встречи с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="38793-124">Удаление повторяющихся серии с помощью веб-служб Exchange — это то же самое, что [Удаление экземпляра собрания](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="38793-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="38793-125">На самом деле запросов SOAP имеет тот же формат.</span><span class="sxs-lookup"><span data-stu-id="38793-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="38793-126">Опять же ключ — это идентификатор элемента, используемой в запросе.</span><span class="sxs-lookup"><span data-stu-id="38793-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="38793-127">Если идентификатор соответствует образца повторения, весь ряд будет удалено.</span><span class="sxs-lookup"><span data-stu-id="38793-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="38793-128">Если идентификатор соответствует одно вхождение, только это вхождение будет удалено.</span><span class="sxs-lookup"><span data-stu-id="38793-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="38793-129">В примерах кода атрибуты **ItemId**, **ChangeKey**и **RecurringMasterId** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="38793-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="38793-130">В этом примере с помощью [операции CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) с элементом [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) для отмены собрания, для которой пользователь является организатором.</span><span class="sxs-lookup"><span data-stu-id="38793-130">This example uses the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="38793-131">Значение элемента [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) указывает элемент, чтобы отменить, и может быть идентификатор элемента повторяющихся основной или одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="38793-131">The value of the [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38793-132">В этом примере использует **операции CreateItem** с элементом [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) отклонение для которого пользователь не является организатором собрания.</span><span class="sxs-lookup"><span data-stu-id="38793-132">This example uses the **CreateItem operation** with a [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="38793-133">Как и в предыдущем примере значение элемента **ReferenceItemId** указывает элемент, чтобы отклонить приглашение, и может быть идентификатор элемента повторяющихся основной или одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="38793-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38793-134">В этом примере используется [операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) для удаления одного экземпляра встречи, ни один из участников.</span><span class="sxs-lookup"><span data-stu-id="38793-134">This example uses the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="38793-135">Этот экземпляр для удаления задается элемент [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , который создан на основе идентификатора элемента повторяющихся хозяина и индекс экземпляра.</span><span class="sxs-lookup"><span data-stu-id="38793-135">The occurrence to delete is specified by the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
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
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38793-136">Обратите внимание на то, что можно получить тем же путем замены элемент **OccurrenceItemId** с элементом [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) , содержащее идентификатор экземпляра, как показано.</span><span class="sxs-lookup"><span data-stu-id="38793-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="38793-137">См. также</span><span class="sxs-lookup"><span data-stu-id="38793-137">See also</span></span>


- [<span data-ttu-id="38793-138">Шаблоны повторения и веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="38793-139">Доступ к ряду с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="38793-140">Создание встречи с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="38793-141">Обновление серии повторяющихся с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="38793-142">Обновление серии повторяющихся с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="38793-143">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="38793-144">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="38793-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="38793-145">Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38793-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

