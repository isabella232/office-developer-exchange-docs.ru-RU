---
title: Удаление встреч в повторяющейся серии с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Узнайте, как удалять встречи в повторяющихся сериях с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: 8a68b6655c98f290d569a14dc0ac518c5d875cbe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513194"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Удаление встреч в повторяющейся серии с помощью EWS в Exchange

Узнайте, как удалять встречи в повторяющихся сериях с помощью управляемого API или EWS EWS в Exchange.
  
Управляемый API или EWS можно использовать для удаления ряда встреч или собраний или одного экземпляра в серии. Процесс удаления целой серии по сути тот же, что и процесс, который используется для удаления одного события. Вы используете те же методы управляемого API EWS или операции EWS, которые используются для удаления одного экземпляра встречи [или собрания.](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) Разница заключается в ID элемента, включенного в метод или операцию. Начнем с того, как оба сценария одинаковы. 
  
Чтобы удалить повторяющиеся серии или единичное возникновение в повторяющейся серии, необходимо найти возникновение или серию, которые необходимо удалить, а затем вызвать соответствующий метод или операцию, чтобы удалить его. Хотя вы можете просто удалить любой тип встречи, мы рекомендуем держать всех участников или организатора в курсе и отменять собрания, которые пользователь организовал, и отказаться от собраний, которые пользователь не организовал.
  
Как же отличаются сценарии? Это объект [Appointment,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) используемый для вызова метода (для управляемого API EWS) или ID элемента, включенного в запрос операции (для EWS). Чтобы удалить целую серию, для повторяющегося мастера необходим объект **"Назначение"** или "ID элемента". Чтобы удалить одно происшествие, вам потребуется объект **Назначения** или ID элемента для возникновения. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Удаление повторяющейся встречи с помощью управляемого API EWS

В этом примере предполагается, что вы сдали Exchange сервер и приобрели службу с именем [объекта ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) Параметр  _recurringItem_ — это объект **Назначения** для повторяющегося мастера или одного события. Параметр _deleteEntireSeries_ указывает, следует ли удалять всю серию, в которую входит повторяющийсяItem.  
  
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

Чтобы использовать этот пример, необходимо [](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)связаться либо с возникновением, либо с повторяющимся мастером, а затем передать в метод объект **"Назначение".** Имейте в виду, что при доступе к встречам с помощью класса [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) все эти элементы являются единиями. И наоборот, если вы используете [класс ItemView,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) все возникающие элементы являются повторяющимися мастерами. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Удаление повторяющейся встречи с помощью EWS

Удаление повторяющейся серии с помощью EWS такое же, как удаление собрания [одного экземпляра.](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md) Фактически запросы SOAP принимают один и тот же формат. Опять же, ключ — это ID элемента, используемый в запросе. Если ID элемента соответствует повторяющимся мастером, вся серия будет удалена. Если ID элемента соответствует одному появлению, будет удален только этот случай.
  
> [!NOTE]
> В последующих примерах кода атрибуты **ItemId,** **ChangeKey** и **RecurringMasterId** сокращаются для читаемости. 
  
В этом примере операция [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) с элементом [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) отменяет собрание, организатором которого является пользователь. Значение элемента [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) указывает на отмену элемента и может быть ИД элемента повторяющегося мастера или одного события. 
  
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

В этом примере операция **CreateItem** с элементом [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) отклонит собрание, для которого пользователь не является организатором. Как и в предыдущем примере, значение элемента **ReferenceItemId** указывает на отклонение элемента и может быть ID элемента повторяющегося мастера или одного возникновения. 
  
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

В этом примере операция [DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) используется для удаления одного события встречи без участников. Возникновение для удаления указывается [элементом OccurrenceItemId,](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) который строится из ID элемента повторяющегося мастера и индекса возникновения. 
  
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
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

Обратите внимание, что такой же результат можно получить, заменив элемент **OccurrenceItemId** [элементом ItemId,](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) который содержит ID элемента возникновения, как показано. 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>См. также


- [Шаблоны повторения и EWS](recurrence-patterns-and-ews.md)
    
- [Доступ к повторяющимся сериям с помощью EWS в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание повторяющейся серии с помощью EWS в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление повторяющихся серий с помощью EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление повторяющейся серии с помощью EWS в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013 г.](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

