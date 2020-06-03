---
title: Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Узнайте, как удалять встречи в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 5646a30d218ed4d795044aefe5efea1399d19a79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528127"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange

Узнайте, как удалять встречи в повторяющихся рядах с помощью управляемого API EWS или EWS в Exchange.
  
Вы можете использовать управляемый API EWS или EWS для удаления ряда встреч или собраний или только одного экземпляра в ряду. Процесс, используемый для удаления всего ряда, практически такой же, как и процесс, используемый для удаления только одного экземпляра. Вы используете те же методы управляемого API EWS и операции EWS, которые используются для [удаления встречи или собрания с одним экземпляром](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md). Разница заключается в ИДЕНТИФИКАТОРе элемента, включенном в метод или операцию. Начнем с того, как оба сценария одинаковы. 
  
Чтобы удалить повторяющиеся ряды или один экземпляр из серии повторяющихся данных, необходимо найти вхождение или ряд, которые нужно удалить, а затем вызвать соответствующий метод или операцию, чтобы удалить его. Несмотря на то, что вы можете просто удалить любой тип встречи, мы рекомендуем хранить всех участников или организатора, а также отклонять собрания, которые пользователь организует и отклоняет собрания.
  
Так как же сценарии различаются? Это все о объекте [встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , используемом для вызова метода (для управляемого API EWS), или идентификатора элемента, включенного в запрос операции (для EWS). Чтобы удалить весь ряд, необходим объект **встречи** или идентификатор элемента для повторяющегося образца. Чтобы удалить один экземпляр, вам потребуется объект **встречи** или идентификатор элемента для этого экземпляра. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Удаление повторяющейся встречи с помощью управляемого API EWS

В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**. Параметр _рекуррингитем_ — это объект **встречи** либо для повторения, либо для одного экземпляра. Параметр _делетинтиресериес_ указывает, следует ли удалить весь ряд, частью которого является _рекуррингитем_ . 
  
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

Чтобы использовать этот пример, необходимо выполнить присоединение [к экземпляру или повторяющейся основной реплике](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)и передать полученный объект **встречи** методу. Имейте в виду, что при доступе к встречам с помощью класса [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) полученные элементы будут иметь один экземпляр. И наоборот, если вы используете класс [итемвиев](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , полученные элементы будут все повторяющимся образцами. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Удаление повторяющейся встречи с помощью EWS

Удаление повторяющейся серии с помощью EWS аналогично [удалению собрания с одним экземпляром](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md). На самом деле запросы SOAP имеют одинаковый формат. Опять же, ключ — это идентификатор элемента, используемый в запросе. Если идентификатор элемента соответствует шаблону повторения, весь ряд будет удален. Если идентификатор элемента соответствует одному экземпляру, то удаляется только это событие.
  
> [!NOTE]
> В приведенных ниже примерах кода атрибуты **ItemId**, **чанжекэй**и **рекуррингмастерид** сокращаются для удобочитаемости. 
  
В этом примере используется [Операция CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) с элементом [канцелкалендаритем](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) для отмены собрания, для которого пользователь является организатором. Значение элемента [референцеитемид](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) указывает элемент для отмены, который может быть идентификатором повторяющегося образца или одним экземпляром. 
  
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

В этом примере используется **Операция CreateItem** с элементом [деклинеитем](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) , чтобы отклонить собрание, для которого пользователь не является организатором. Как и в предыдущем примере, значение элемента **референцеитемид** указывает, что элемент следует отклонить, и может быть идентификатором повторяющейся основной или единичной копии. 
  
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

В этом примере используется [Операция DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) для удаления одного экземпляра встречи без участников. Удаляемое событие задается элементом [оккурренцеитемид](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , созданным на основе идентификатора элемента повторяющейся основной реплики и индекса экземпляра. 
  
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

Обратите внимание, что вы можете получить тот же результат, заменив элемент **оккурренцеитемид** на элемент [ITEMID](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) , содержащий идентификатор элемента, как показано ниже. 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>См. также


- [Шаблоны повторения и EWS](recurrence-patterns-and-ews.md)
    
- [Доступ к повторяющимся сериям с помощью EWS в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание серии повторяющихся данных с помощью EWS в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся данных с помощью EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление серии повторяющихся данных с помощью EWS в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

