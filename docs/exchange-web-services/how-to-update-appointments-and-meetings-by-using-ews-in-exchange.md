---
title: Обновление встречи и собрания с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 12/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 13256625-083e-4a17-8fd1-2bed1f7cc14e
description: Узнайте, как обновить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: a4265a14a46c146c584a3daa61cef5486958e14e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761119"
---
# <a name="update-appointments-and-meetings-by-using-ews-in-exchange"></a>Обновление встречи и собрания с помощью веб-служб Exchange в Exchange

Узнайте, как обновить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Важные различия между собраний и встреч —, что у участников собрания, а не встреч. Встречи и собрания могут быть отдельные экземпляры или частью серии повторяющихся, но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение. Для внутреннего использования Exchange использует тот же объект для собраний и встреч. Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для работы с собраний и встреч. 
  
**В таблице 1. Управляемый API EWS метод и операции EWS для обновления встречи и собрания**

|**Метод управляемого API EWS**|**Соответствующие операции веб-служб Exchange**|
|:-----|:-----|
|[Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)<br/><br/>          [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) <br/> |
   
## <a name="update-an-appointment-by-using-the-ews-managed-api"></a>Обновление встречи с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_UpdateApptEWSMA"> </a>

В следующем примере кода показано, как использовать [объект встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) для обновления свойств, связанных с встречи и метод [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) , чтобы сохранить встречу в папке календаря. 
  
В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. Локальной переменной `appointmentId` — это идентификатор, связанный с существующей встречи. 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End));
string oldSubject = appointment.Subject;
// Update properties on the appointment with a new subject, start time, and end time.
appointment.Subject = appointment.Subject + " moved one hour later and to the day after " + appointment.Start.DayOfWeek + "!";
appointment.Start.AddHours(25);
appointment.End.AddHours(25);
// Unless explicitly specified, the default is to use SendToAllAndSaveCopy.
// This can convert an appointment into a meeting. To avoid this,
// explicitly set SendToNone on non-meetings.
SendInvitationsOrCancellationsMode mode = appointment.IsMeeting ? 
    SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy : SendInvitationsOrCancellationsMode.SendToNone;
// Send the update request to the Exchange server.
appointment.Update(ConflictResolutionMode.AlwaysOverwrite, mode);
// Verify the update.
Console.WriteLine("Subject for the appointment was \"" + oldSubject + "\". The new subject is \"" + appointment.Subject + "\"");

```

## <a name="update-an-appointment-by-using-ews"></a>Обновление встречи с помощью веб-служб Exchange
<a name="bk_UpdateApptEWS"> </a>

Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [обновление встречи с помощью управляемого интерфейса API веб-служб Exchange](#bk_UpdateApptEWSMA).
  
В следующем примере показано запроса XML при использовании операции [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) обновить встречи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Tennis Lesson moved one hour later and to the day after Wednesday!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML-код, который возвращается в ответ на запрос [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) . Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exc
hange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-a-meeting-by-using-the-ews-managed-api"></a>Обновление собрания с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_UpdateMtgEWSMA"> </a>

При обновлении собрания, в дополнение к Сохранение измененного встречи в папке календаря обычно также требуется отправить обновленные приглашения участникам. В следующем примере кода показано, как обновить собрания и отправка приглашений на собрания.
  
В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. Локальной переменной `meetingId` — это идентификатор, который связан с существующую встречу. 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet(AppointmentSchema.Subject, 
                                                                           AppointmentSchema.Location, 
                                                                           AppointmentSchema.RequiredAttendees, 
                                                                           AppointmentSchema.Resources));
string oldSubject = meeting.Subject;
// Update properties on the appointment with a new subject, location, an additional required attendee, and a resource.
meeting.Subject = "Team building exercise has moved!";
meeting.Location = "4567 Contoso Way, Redmond, OH 33333, USA";
meeting.RequiredAttendees.Add("alisa@contoso.com");
meeting.Resources.Add("dlpprojector@contoso.com");
// Send the update request to the Exchange server.
meeting.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
// Verify the update.
Console.WriteLine("Subject for the meeting was \"" + oldSubject + "\". The new subject is \"" + meeting.Subject + "\"");

```

После установки свойства объекта [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , сохранить собрание в папке календаря и отправлять обновленные приглашения на собрания с помощью метода [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) . 
  
Вы можете передать в одном из двух значений перечисления как параметры при вызове метода [обновления](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) : 
  
- [Перечисление ConflictResolutionMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) — определяет конфликтов обработки состояния между клиентом и сервером. 
    
- [Перечисление SendInvitationsOrCancellationsMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode%28v=exchg.80%29.aspx) — влияет на отправку и сохранения обновления приглашений на собрания. 
    
При установке значения перечисления [ConflictResolutionMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) для **AlwaysOverwrite**вашей версии собрания всегда будут сохраняться в папке календаря.
  
## <a name="update-a-meeting-by-using-ews"></a>Обновление собрания с помощью веб-служб Exchange
<a name="bk_UpdateMtgEWS"> </a>

Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [обновление собрания с помощью управляемого интерфейса API веб-служб Exchange](#bk_UpdateMtgEWSMA). 
  
В следующем примере показано запроса XML при использовании операции [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) обновление собрания. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Team building exercise has moved!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>4567 Contoso Way, Redmond, OH 33333, USA</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack.Chaves@contoso.com</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie.Daniels@contoso.com</t:Name>
                      <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>alisa@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Resources" />
              <t:CalendarItem>
                <t:Resources>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>dlpprojector@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:Resources>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

 В следующем примере показано XML-код, который возвращается в ответ на запрос [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) . Атрибуты **ChangeKey** и **ItemId** URL-были сокращены для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)   
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)   
- [Получение встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)  
- [Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

