---
title: Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Узнайте, как удалять встречи в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761018"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="f573e-103">Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="f573e-104">Узнайте, как удалять встречи в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f573e-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="f573e-105">Вы можете использовать управляемый API EWS или EWS для удаления ряда встреч или собраний или только одного экземпляра в ряду.</span><span class="sxs-lookup"><span data-stu-id="f573e-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="f573e-106">Процесс, используемый для удаления всего ряда, практически такой же, как и процесс, используемый для удаления только одного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="f573e-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="f573e-107">Вы используете те же методы управляемого API EWS и операции EWS, которые используются для [удаления встречи или собрания с одним экземпляром](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f573e-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="f573e-108">Разница заключается в ИДЕНТИФИКАТОРе элемента, включенном в метод или операцию.</span><span class="sxs-lookup"><span data-stu-id="f573e-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="f573e-109">Начнем с того, как оба сценария одинаковы.</span><span class="sxs-lookup"><span data-stu-id="f573e-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="f573e-110">Чтобы удалить повторяющиеся ряды или один экземпляр из серии повторяющихся данных, необходимо найти вхождение или ряд, которые нужно удалить, а затем вызвать соответствующий метод или операцию, чтобы удалить его.</span><span class="sxs-lookup"><span data-stu-id="f573e-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="f573e-111">Несмотря на то, что вы можете просто удалить любой тип встречи, мы рекомендуем хранить всех участников или организатора, а также отклонять собрания, которые пользователь организует и отклоняет собрания.</span><span class="sxs-lookup"><span data-stu-id="f573e-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="f573e-112">Так как же сценарии различаются?</span><span class="sxs-lookup"><span data-stu-id="f573e-112">So how are the scenarios different?</span></span> <span data-ttu-id="f573e-113">Это все о объекте [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , используемом для вызова метода (для управляемого API EWS), или идентификатора элемента, включенного в запрос операции (для EWS).</span><span class="sxs-lookup"><span data-stu-id="f573e-113">It's all about the [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="f573e-114">Чтобы удалить весь ряд, необходим объект **встречи** или идентификатор элемента для повторяющегося образца.</span><span class="sxs-lookup"><span data-stu-id="f573e-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="f573e-115">Чтобы удалить один экземпляр, вам потребуется объект **встречи** или идентификатор элемента для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="f573e-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="f573e-116">Удаление повторяющейся встречи с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="f573e-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="f573e-117">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="f573e-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="f573e-118">Параметр _рекуррингитем_ — это объект **встречи** либо для повторения, либо для одного экземпляра.</span><span class="sxs-lookup"><span data-stu-id="f573e-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="f573e-119">Параметр _делетинтиресериес_ указывает, следует ли удалить весь ряд, частью которого является _рекуррингитем_ .</span><span class="sxs-lookup"><span data-stu-id="f573e-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
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

<span data-ttu-id="f573e-120">Чтобы использовать этот пример, необходимо выполнить присоединение [к экземпляру или повторяющейся основной реплике](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)и передать полученный объект **встречи** методу.</span><span class="sxs-lookup"><span data-stu-id="f573e-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="f573e-121">Имейте в виду, что при доступе к встречам с помощью класса [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) полученные элементы будут иметь один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="f573e-121">Keep in mind that if you access appointments by using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="f573e-122">И наоборот, если вы используете класс [итемвиев](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , полученные элементы будут все повторяющимся образцами.</span><span class="sxs-lookup"><span data-stu-id="f573e-122">Conversely, if you use the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="f573e-123">Удаление повторяющейся встречи с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="f573e-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="f573e-124">Удаление повторяющейся серии с помощью EWS аналогично [удалению собрания с одним экземпляром](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f573e-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="f573e-125">На самом деле запросы SOAP имеют одинаковый формат.</span><span class="sxs-lookup"><span data-stu-id="f573e-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="f573e-126">Опять же, ключ — это идентификатор элемента, используемый в запросе.</span><span class="sxs-lookup"><span data-stu-id="f573e-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="f573e-127">Если идентификатор элемента соответствует шаблону повторения, весь ряд будет удален.</span><span class="sxs-lookup"><span data-stu-id="f573e-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="f573e-128">Если идентификатор элемента соответствует одному экземпляру, то удаляется только это событие.</span><span class="sxs-lookup"><span data-stu-id="f573e-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f573e-129">В приведенных ниже примерах кода атрибуты **ItemId**, **чанжекэй**и **рекуррингмастерид** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f573e-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="f573e-130">В этом примере используется [Операция CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) с элементом [канцелкалендаритем](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) для отмены собрания, для которого пользователь является организатором.</span><span class="sxs-lookup"><span data-stu-id="f573e-130">This example uses the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="f573e-131">Значение элемента [референцеитемид](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) указывает элемент для отмены, который может быть идентификатором повторяющегося образца или одним экземпляром.</span><span class="sxs-lookup"><span data-stu-id="f573e-131">The value of the [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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

<span data-ttu-id="f573e-132">В этом примере используется **Операция CreateItem** с элементом [деклинеитем](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) , чтобы отклонить собрание, для которого пользователь не является организатором.</span><span class="sxs-lookup"><span data-stu-id="f573e-132">This example uses the **CreateItem operation** with a [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="f573e-133">Как и в предыдущем примере, значение элемента **референцеитемид** указывает, что элемент следует отклонить, и может быть идентификатором повторяющейся основной или единичной копии.</span><span class="sxs-lookup"><span data-stu-id="f573e-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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

<span data-ttu-id="f573e-134">В этом примере используется [Операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) для удаления одного экземпляра встречи без участников.</span><span class="sxs-lookup"><span data-stu-id="f573e-134">This example uses the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="f573e-135">Удаляемое событие задается элементом [оккурренцеитемид](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , созданным на основе идентификатора элемента повторяющейся основной реплики и индекса экземпляра.</span><span class="sxs-lookup"><span data-stu-id="f573e-135">The occurrence to delete is specified by the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
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

<span data-ttu-id="f573e-136">Обратите внимание, что вы можете получить тот же результат, заменив элемент **оккурренцеитемид** на элемент [ITEMID](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) , содержащий идентификатор элемента, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="f573e-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="f573e-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f573e-137">See also</span></span>


- [<span data-ttu-id="f573e-138">Шаблоны повторения и EWS</span><span class="sxs-lookup"><span data-stu-id="f573e-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="f573e-139">Доступ к повторяющимся сериям с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f573e-140">Создание серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f573e-141">Обновление серии повторяющихся данных с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="f573e-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="f573e-142">Обновление серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f573e-143">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f573e-144">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f573e-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="f573e-145">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f573e-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

