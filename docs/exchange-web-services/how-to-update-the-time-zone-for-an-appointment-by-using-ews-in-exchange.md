---
title: Обновление часового пояса для встречи с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Узнайте, как обновить часовой пояс для существующих встреч и собраний с помощью управляемого API EWS и EWS в Exchange.
ms.openlocfilehash: 535eb9f546d9a4353408579f3a24750f32237699
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761126"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a>Обновление часового пояса для встречи с помощью веб-служб Exchange в Exchange

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Узнайте, как обновить часовой пояс для существующих встреч и собраний с помощью управляемого API EWS и EWS в Exchange.
  
При создании встречи или собрания для календаря Exchange часовой пояс, используемый для указания времени начала и окончания, сохраняется как часовой пояс создания встречи. Этот часовой пояс можно изменить с помощью EWS или управляемого API EWS. Тем не менее, изменение часового пояса приводит и к другим последствиям для времени начала и окончания встречи.
  
Значения времени хранятся на сервере Exchange Server в формате UTC. Таким образом, если встреча начинается в 13:00 по Восточному времени США (UTC-05:00), это значение сохраняется на сервере как 18:00, при условии что часовой пояс находится в стандартной фазе (зимнее время). При просмотре этой встречи в других часовых поясах соответствующее количество часов добавляется или вычитается из значения времени в формате UTC для определения конкретного времени. Например, если встреча начинается в 13:00 по Восточному времени США (18:00 UTC) и ее просматривает клиент из Тихоокеанского часового пояса (UTC-08:00), временем начала встречи для этого клиента будет 10:00 (18:00-08:00).
  
При изменении часового пояса встречи без обновления времени начала и окончания сервер обновляет значения в формате UTC, хранящиеся на сервере. Рассмотрим встречу, которая начинается в 13:00 по Восточному времени. Время хранится на сервере как 18:00 UTC. Если часовой пояс встречи изменяется на Тихоокеанский, сервер сдвигает время начала на 13:00 по Тихоокеанскому времени (21:00 UTC).
  
Это поведение можно изменить, явно задав время начала и окончания.
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a>Обновление часового пояса существующей встречи с помощью управляемого API EWS

В следующем примере управляемый API EWS используется для обновления часового пояса на существующую встречу в центре часовой пояс, изменив свойства **Appointment.EndTimeZone** и **Appointment.StartTimeZone** . Если параметр _shiftAppointnment_ имеет значение **true**, код не заданы явно времени начала и завершения для встречи. В этом случае сервер будет сместиться времени начала и завершения для сохранения их в одно и то же время относительно часового пояса в новый часовой пояс. Если задано значение **false**, код преобразует времени начала и завершения явным образом, чтобы сохранить встречу в то же время в формате UTC. 

В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
```cs
static void UpdateAppointmentTimeZone(ExchangeService service, ItemId apptId, bool shiftAppointment)
{
    PropertySet includeTimeZones = new PropertySet(AppointmentSchema.Subject,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.ReminderDueBy,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.StartTimeZone,
                                                   AppointmentSchema.EndTimeZone);
    Appointment apptToUpdate;
    // Load the existing appointment.
    // This will result in a call to EWS.
    try
    {
        apptToUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("Before update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptToUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptToUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptToUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptToUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptToUpdate.EndTimeZone.DisplayName);
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Update the time zones on the appointment.
    apptToUpdate.StartTimeZone = centralTZ;
    apptToUpdate.EndTimeZone = centralTZ;
    if (!shiftAppointment)
    {
        // Set the start and end times explicitly so that the appointment
        // will start and end at the same UTC time.
        // Convert the times to then Central time zone. This
        // will keep them at the same time in UTC.
        // For example, 1:00 PM Eastern becomes 12:00 PM Central.
        DateTime newStartTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.Start, centralTZ);
        DateTime newEndTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.End, centralTZ);
        apptToUpdate.Start = newStartTime;
        apptToUpdate.End = newEndTime;
    }
    try
    {
        // Save the changes. This will result in a call to EWS.
        apptToUpdate.Update(ConflictResolutionMode.AlwaysOverwrite, 
            SendInvitationsOrCancellationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating appointment: {0}", ex.Message);
        return;
    }
    // Now rebind to the appointment to get the new values.
    Appointment apptAfterUpdate;
    
    try
    {
        // This will result in a call to EWS.
        apptAfterUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("After update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptAfterUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptAfterUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptAfterUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptAfterUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptAfterUpdate.EndTimeZone.DisplayName);
}
```

Когда пример используется для обновления встречи, которая начинается в 13:00 по Восточному времени и заканчивается в 14:00 по Восточному времени, при этом для параметра  _shiftAppointment_ задано значение true, а свойству [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) присвоен Восточный часовой пояс, результат выглядит следующим образом. 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 2:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 2:00:00 PM
  End: 6/20/2014 3:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

Когда пример используется для обновления той же встречи, при этом для параметра  _shiftAppointment_ установлено значение false, а свойству **TimeZone** также присвоен Восточный часовой пояс, результат немного отличается. 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

Обратите внимание, что время начала и окончания не было изменены. Это происходит потому, что время интерпретируются в Восточном часовом поясе (так как свойству **TimeZone** присвоен Восточный часовой пояс), а значения времени были обновлены, чтобы предотвратить сдвиг встречи. 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a>Обновление часового пояса существующей встречи с помощью EWS

Следующий пример запроса [UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS обновляет часовой пояс встречи. В этом примере обновляются только элементы [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) и [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx), поэтому сервер будет сдвигать время начала и окончания встречи, чтобы сохранить то же относительное время в новом часовом поясе. Значение элемента **ItemId** укорочено для удобства чтения. 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

Следующий пример запроса обновляет часовой пояс встречи, а также время начала и окончания, явно задавая элементы **Start** и **End**. Значение элемента **ItemId** укорочено для удобства чтения. 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-06-20T17:00:00.000Z</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-06-20T18:00:00.000Z</t:End>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также

- [Часовые пояса и EWS в Exchange](time-zones-and-ews-in-exchange.md)   
- [Создание встречи в конкретного часового пояса с помощью веб-служб Exchange в Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

