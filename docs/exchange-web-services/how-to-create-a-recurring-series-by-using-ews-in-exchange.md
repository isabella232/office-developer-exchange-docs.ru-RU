---
title: Создание серии повторяющихся данных с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 88ed6e87-25f7-4a54-83fa-d757a0ff2528
description: Узнайте, как создавать повторяющиеся собрания с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 1d04bd48c56a1a0e94eb1368166f776b3dfeb23a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456873"
---
# <a name="create-a-recurring-series-by-using-ews-in-exchange"></a>Создание серии повторяющихся данных с помощью EWS в Exchange

Узнайте, как создавать повторяющиеся собрания с помощью управляемого API EWS или EWS в Exchange.
  
Создание повторяющейся встречи или собрания не так сильно отличается от создания [встречи или собрания с одним экземпляром](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md). Необходимо только назначить значения нескольким дополнительным свойствам, связанным с повторением. Они задаются для объекта [повторения](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) объекта [ExchangeService. Встреча](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) (при использовании управляемого API EWS) или дочернего элемента [повторения](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) элемента [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) (если вы используете EWS). Если вы создаете повторяющееся собрание, а не на одном экземпляре, следует учитывать, что создаваемый элемент календаря является шаблоном повторения для ряда. Ряд свойств устанавливается только в повторяющейся основной реплике; Эти свойства помогут найти, изменить или удалить отдельные экземпляры в ряду. По этой причине при создании серии повторяющихся данных может быть полезно отслеживать идентификатор повторяющегося образца... 
  
**Таблица 1. Свойства, заданные для повторяющихся элементов главного календаря**

|**Класс или свойство управляемого API EWS**|**Элемент XML EWS**|**Описание**|
|:-----|:-----|:-----|
|[Класс повторения](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) <br/> Класс **повторения** — это базовый класс производного класса шаблона: [интервалпаттерн](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx), [релативэйеарлипаттерн](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx)или [еарлипаттерн](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).  <br/> |[Повторение (RecurrenceType)](https://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) <br/> |Содержит сведения, связанные с повторением, включая расписание повторения (ежедневно, еженедельно, ежемесячно и т. д.), дату начала и окончания, число повторений и т. д.  <br/> |
|[Свойство Фирстоккурренце](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) <br/> |[фирстоккурренце](https://msdn.microsoft.com/library/d6748860-ce0d-4d2e-b7e4-9ed834f1e45a%28Office.15%29.aspx) <br/> |Содержит начальное и конечное время и идентификатор элемента для первого собрания в ряду.  <br/> |
|[Свойство Ластоккурренце](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) <br/> |[ластоккурренце](https://msdn.microsoft.com/library/c9ef0fcb-4265-4e60-9986-fff0f211d00b%28Office.15%29.aspx) <br/> |Содержит начальное и конечное время, а также идентификатор элемента для последнего собрания в ряду.  <br/> |
|[Свойство Модифиедоккурренцес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) <br/> |[модифиедоккурренцес](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) <br/> |Содержит набор всех собраний в серии, которые были изменены из исходного шаблона повторения.  <br/> |
|[Свойство Делетедоккурренцес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) <br/> |[делетедоккурренцес](https://msdn.microsoft.com/library/736fb305-9528-4be8-ad37-65d7556edbf2%28Office.15%29.aspx) <br/> |Содержит набор всех собраний в серии, которые были удалены из исходного шаблона повторения.  <br/> |
   
Так как собрания по сути являются встречами, включающими участников, в примерах кода в этой статье показано, как создать повторяющиеся собрания. Если вы хотите создать повторяющуюся встречу, вы можете изменить примеры, удалив код, связанный с участниками.
  
## <a name="create-a-recurring-meeting-by-using-the-ews-managed-api"></a>Создание повторяющегося собрания с помощью управляемого API EWS
<a name="bk_CreateMtgEWSMA"> </a>

В приведенном ниже примере кода показано, как создать повторяющееся собрание. Сначала назначьте значения свойствам [объекта встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , используемого для создания собрания, а затем с помощью метода [сохранения](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) сохраните серию в папке "Календарь" и отправьте приглашения на собрание участникам. Наконец, используйте метод [встреча. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) для просмотра значений, заданных для шаблона повторения, который вы только что создали. 
  
В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**. Метод, приведенный в этом примере, возвращает [идентификатор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) повторяющегося образца повторяющейся серии. 
  
```cs
public static ItemId CreateARecurringMeeting(ExchangeService service)
{        Appointment recurrMeeting = new Appointment(service);
        // Set the properties you need to create a meeting.
        recurrMeeting.Subject = "Weekly Update Meeting";
        recurrMeeting.Body = "Come hear about how the project is coming along!";
        recurrMeeting.Start = DateTime.Now.AddDays(1);
        recurrMeeting.End = recurrMeeting.Start.AddHours(1);
        recurrMeeting.Location = "Contoso Main Gallery";
        recurrMeeting.RequiredAttendees.Add("Mack@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Sadie@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Magdalena@contoso.com"); recurrMeeting.ReminderMinutesBeforeStart = 30;
             
        DayOfTheWeek[] dow = new DayOfTheWeek[] { (DayOfTheWeek)recurrMeeting.Start.DayOfWeek };
        // The following are the recurrence-specific properties for the meeting.
        recurrMeeting.Recurrence = new Recurrence.WeeklyPattern(recurrMeeting.Start.Date, 1, dow);
        recurrMeeting.Recurrence.StartDate = recurrMeeting.Start.Date;
        recurrMeeting.Recurrence.NumberOfOccurrences = 10;
        // This method results in in a CreateItem call to EWS.
        recurrMeeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
        // Retrieve the meeting subject and the properties that are set on a recurring master when a recurring series is created.
        recurrMeeting = Appointment.Bind(service, recurrMeeting.Id, new PropertySet(AppointmentSchema.Subject,
                                                                                    AppointmentSchema.AppointmentType, 
                                                                                    AppointmentSchema.Recurrence, 
                                                                                    AppointmentSchema.FirstOccurrence,
                                                                                    AppointmentSchema.LastOccurrence,
                                                                                    AppointmentSchema.ModifiedOccurrences,
                                                                                    AppointmentSchema.DeletedOccurrences));
        // Print out the recurring master properties.
        Console.WriteLine("\nAppointment created: " + recurrMeeting.Subject);
        Console.WriteLine("Appointment Type: {0}\n", recurrMeeting.AppointmentType);
        Console.WriteLine("These property values are always null unless the item is a recurring master:\n");
        Console.WriteLine("\tRecurrence pattern: {0}", recurrMeeting.Recurrence.ToString());
        Console.WriteLine("\tRecurring series start Date: {0}", recurrMeeting.Recurrence.StartDate.ToString());
        Console.WriteLine("\tRecurring series end Date: {0}", 
                        recurrMeeting.Recurrence.EndDate == null ? "Null" : recurrMeeting.Recurrence.EndDate.ToString());
        Console.WriteLine("\tHas end: {0}", recurrMeeting.Recurrence.HasEnd.ToString());
        Console.WriteLine("\tNumber of occurrances: {0}", recurrMeeting.Recurrence.NumberOfOccurrences);
        Console.WriteLine("\tLast 24 characters of the first occurrence's item ID:\t {0}", 
                        recurrMeeting.FirstOccurrence.ItemId.ToString().Substring(144));
        Console.WriteLine("\tLast 24 characters of the last occurrence's item ID:\t {0}", 
                        recurrMeeting.LastOccurrence.ItemId.ToString().Substring(144)); 
        Console.WriteLine("\tModified Occurrences: {0}", 
                        (recurrMeeting.ModifiedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString()));
        Console.WriteLine("\tDeleted Occurrences: {0}", 
                        recurrMeeting.DeletedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString());
        // Return the ID of the recurring master.
        return recurrMeeting.Id;
}

```

## <a name="create-a-recurring-meeting-by-using-ews"></a>Создание повторяющегося собрания с помощью EWS
<a name="bk_CreateMtgEWS"> </a>

XML-код запроса и ответа в приведенных ниже примерах соответствует вызовам, выполняемым для [создания повторяющегося собрания с помощью управляемого API EWS](#bk_CreateMtgEWSMA). Обратите внимание, что кроме установки значений, относящихся [к](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) повторению, запрос в основном такой же, как и для создания встречи с одним экземпляром. В следующем примере показан XML-код запроса при использовании операции [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Weekly Update Meeting</t:Subject>
          <t:Body BodyType="HTML">Come hear about how the Organized Observational Paradigm SkyNet project is coming along!</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-08T13:21:32.868-08:00</t:Start>
          <t:End>2014-03-08T14:21:32.868-08:00</t:End>
          <t:Location>Contoso Main Gallery</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Saturday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-03-08-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

 В следующем примере показан XML-код отклика, возвращаемый операцией **CreateItem** . 
  
Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

В следующем примере показан XML-код запроса, который создается при использовании операции [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) и элемента **ItemId** для созданного ряда, а свойства запроса задаются только для повторяющегося образца, чтобы убедиться в том, что идентификатор **ItemId** , возвращенный сервером при создании повторяющихся рядов, предназначен для повторяющегося образца. 
  
Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Recurrence" />
          <t:FieldURI FieldURI="calendar:FirstOccurrence" />
          <t:FieldURI FieldURI="calendar:LastOccurrence" />
          <t:FieldURI FieldURI="calendar:ModifiedOccurrences" />
          <t:FieldURI FieldURI="calendar:DeletedOccurrences" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 В следующем примере показан XML-код отклика, возвращенный операцией **GetItem** . 
  
Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
              <t:Subject>Weekly Update Meeting</t:Subject>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              <t:Recurrence>
                <t:WeeklyRecurrence>
                  <t:Interval>1</t:Interval>
                  <t:DaysOfWeek>Saturday</t:DaysOfWeek>
                </t:WeeklyRecurrence>
                <t:NumberedRecurrence>
                  <t:StartDate>2014-03-08-08:00</t:StartDate>
                  <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
                </t:NumberedRecurrence>
              </t:Recurrence>
              <t:FirstOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-03-08T21:21:00Z</t:Start>
                <t:End>2014-03-08T22:21:00Z</t:End>
                <t:OriginalStart>2014-03-08T21:21:00Z</t:OriginalStart>
              </t:FirstOccurrence>
              <t:LastOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-05-10T20:21:00Z</t:Start>
                <t:End>2014-05-10T21:21:00Z</t:End>
                <t:OriginalStart>2014-05-10T20:21:00Z</t:OriginalStart>
              </t:LastOccurrence>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Шаблоны повторения и EWS](recurrence-patterns-and-ews.md)
    
- [Доступ к повторяющимся сериям с помощью EWS в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся данных с помощью EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление серии повторяющихся данных с помощью EWS в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

