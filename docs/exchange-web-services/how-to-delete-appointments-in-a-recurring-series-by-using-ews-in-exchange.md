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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761018"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange

Узнайте, как удаление встреч в серии повторяющихся с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Чтобы удалить ряд встречи или собрания или только один экземпляр из серии можно использовать управляемый API EWS или веб-служб Exchange. Процесс, который используется для удаления всего ряда практически не то же, что процесс, который используется для удаления только одно вхождение. Используйте одинаковые методы управляемый API EWS или операции EWS, используемые для [удаления одного экземпляра встречи или собрания](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md). Отличие заключается в идентификатор, который включен в метод или операции. Давайте начнем, посмотрев как оба сценария, совпадают. 
  
Чтобы удалить серии повторяющихся или одно вхождение в ряду, необходимо найти копию, или серии, которую требуется удалить, а затем вызвать соответствующий метод или операцию, чтобы удалить его. В то время как можно просто удалить любой тип встречи, рекомендуется хранить участников собрания или организатора и отмены собраний, организованных пользователем и отклонение собрания, которые не были организации пользователя.
  
Так как отличаются сценарии? Он все о [встрече](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) объект, используемый для вызова метода (для управляемого API EWS) или идентификатор элемента включен в операции запроса (EWS). Для удаления всей серии, требуется идентификатор объекта или элемента **встречи** образца повторения. Для удаления одного экземпляра, требуется идентификатор объекта или элемента **встречи** этот экземпляр. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Удаление повторяющейся встречи с помощью управляемого интерфейса API веб-служб Exchange

В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. Параметр _recurringItem_ является объектом **встречи** для повторяющихся основной или одно вхождение. Параметр _deleteEntireSeries_ указывает, следует ли удалить всю последовательность, которая является частью процессов _recurringItem_ . 
  
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

Для использования в этом примере, чтобы [присоединить вхождения или повторяющихся главных](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)и передачи результирующего объекта **встречи** в метод. Имейте в виду, что при доступе к встречи с помощью класса [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , полученные их все вхождения одной. И наоборот Если вы используете класс [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , результирующий элементы, всех повторяющихся образцов. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Удаление повторяющейся встречи с помощью веб-служб Exchange

Удаление повторяющихся серии с помощью веб-служб Exchange — это то же самое, что [Удаление экземпляра собрания](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md). На самом деле запросов SOAP имеет тот же формат. Опять же ключ — это идентификатор элемента, используемой в запросе. Если идентификатор соответствует образца повторения, весь ряд будет удалено. Если идентификатор соответствует одно вхождение, только это вхождение будет удалено.
  
> [!NOTE]
> В примерах кода атрибуты **ItemId**, **ChangeKey**и **RecurringMasterId** сокращаются для удобства чтения. 
  
В этом примере с помощью [операции CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) с элементом [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) для отмены собрания, для которой пользователь является организатором. Значение элемента [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) указывает элемент, чтобы отменить, и может быть идентификатор элемента повторяющихся основной или одно вхождение. 
  
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

В этом примере использует **операции CreateItem** с элементом [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) отклонение для которого пользователь не является организатором собрания. Как и в предыдущем примере значение элемента **ReferenceItemId** указывает элемент, чтобы отклонить приглашение, и может быть идентификатор элемента повторяющихся основной или одно вхождение. 
  
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

В этом примере используется [операция DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) для удаления одного экземпляра встречи, ни один из участников. Этот экземпляр для удаления задается элемент [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , который создан на основе идентификатора элемента повторяющихся хозяина и индекс экземпляра. 
  
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

Обратите внимание на то, что можно получить тем же путем замены элемент **OccurrenceItemId** с элементом [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) , содержащее идентификатор экземпляра, как показано. 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>См. также


- [Шаблоны повторения и веб-служб Exchange](recurrence-patterns-and-ews.md)
    
- [Доступ к ряду с помощью веб-служб Exchange в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание встречи с помощью веб-служб Exchange в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся с помощью веб-служб Exchange](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление серии повторяющихся с помощью веб-служб Exchange в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

