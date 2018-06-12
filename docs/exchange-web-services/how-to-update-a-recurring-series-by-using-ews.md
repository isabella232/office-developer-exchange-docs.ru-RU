---
title: Обновление серии повторяющихся с помощью веб-служб Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e61bee9-4840-4773-a0a7-47b11e1fdf59
description: Узнайте, как изменить встреч в серии повторяющихся с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: ecee78457d2e6f91483cf897cfb4976fbd83400c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761129"
---
# <a name="update-a-recurring-series-by-using-ews"></a>Обновление серии повторяющихся с помощью веб-служб Exchange

Узнайте, как изменить встреч в серии повторяющихся с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Управляемый API EWS или веб-служб Exchange можно использовать для обновления серии повторяющихся, либо [обновление всей серии](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)или обновив одно вхождение. В этой статье мы обсудим, как обновить одно вхождение.
  
Изменение одного встречу в ряде является очень похоже на [Изменение встречи один экземпляр](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md). Используйте одинаковые методы и операции, но использовать идентификатор экземпляра, который нужно изменить.
  
При изменении одно вхождение из серии это вхождение добавляется в массив измененные встречи, связанные с повторяющейся главной серии. Можно использовать свойство управляемый API EWS [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) или элемент [ModifiedOccurrences](http://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) веб-служб Exchange для доступа к все встречи в цикле, которые были изменены. 
  
## <a name="modify-a-single-occurrence-in-a-series-by-using-the-ews-managed-api"></a>Измените одно вхождение в цикле с помощью управляемого интерфейса API веб-служб Exchange

Для изменения один экземпляр списка, который:
  
1. Привязка к этот экземпляр, который необходимо изменить с помощью метода [Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) с значение индекса элемента, либо метод [Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) с идентификатором этот экземпляр. Получить этот код из свойства [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) , соответствующий этот экземпляр объекта [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или из свойство [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) объекта [OccurrenceInfo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) , соответствующий этот экземпляр. 
    
2. Обновляет свойства объекта встречи этот экземпляр.
    
3. Сохраните изменения в этот экземпляр объекта встречи с помощью метода [Appointment.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) . 
    
В следующем примере обновляется встречу в ряде повторяющихся и проверяет, что измененная встречи обновляется в образце повторяющейся. В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. `recurrenceMasterId` Параметр — это идентификатор, связанный с повторяющейся главным источником для появления для изменения. 
  
```cs
public static ItemId ModifyARecurringSeries(ExchangeService service, ItemId recurrenceMasterId)
{
    Appointment calendarItem = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    if (calendarItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        // Get the recurring master from an occurrence in a recurring series with the properties you need.
        recurrMaster = Appointment.Bind(service,
                                        recurrenceMasterId,
                                        new PropertySet(AppointmentSchema.AppointmentType,
                                                        AppointmentSchema.Subject,
                                                        AppointmentSchema.FirstOccurrence,
                                                        AppointmentSchema.LastOccurrence,
                                                        AppointmentSchema.ModifiedOccurrences,
                                                        AppointmentSchema.DeletedOccurrences));
    }
    else
    {
        Console.WriteLine("Item id was not for a recurring master.");
        return recurrenceMasterId;
    }
    // Bind to the second occurrence in the series with the properties to modify.
    Appointment occurrenceToModify = Appointment.BindToOccurrence(service,
                                                                    recurrMaster.Id,
                                                                    2,
                                                                    new PropertySet(AppointmentSchema.Location,
                                                                                    AppointmentSchema.Start,
                                                                                    AppointmentSchema.End,
                                                                                    AppointmentSchema.RequiredAttendees,
                                                                                    AppointmentSchema.Subject));
    // Update the properties you want to change.
    occurrenceToModify.Location = "Helipad of Contoso Bldg 1";
    occurrenceToModify.Start = occurrenceToModify.Start.AddDays(1);
    occurrenceToModify.End = occurrenceToModify.End.AddDays(1);
    occurrenceToModify.RequiredAttendees.Add("Contoso CEO", "sadie@contoso");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Research", "ronnie@contoso.com");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Security", "alfred@contoso.com");
    occurrenceToModify.Subject = occurrenceToModify.Subject.ToString() + ":Mandatory";
    // Update the occurrence in your calendar folder and send meeting update requests to attendees.
    // This method call results in an UpdateItem request to EWS.
    occurrenceToModify.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
    // View updated and deleted occurrences on the recurring master prior to retrieving updated information.
    Console.WriteLine("Modified Occurrences prior to updating recurring master: {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    // Update the recurring master to view the modified and deleted occurrences.
    recurrMaster = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.ModifiedOccurrences,
                                                                        AppointmentSchema.DeletedOccurrences));
    // View updated and deleted occurrences on the recurring master after retrieving updated information.
    Console.WriteLine("Modified Occurrences after updating recurring master:\t {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    return recurrMaster.Id;            
}

```

## <a name="modify-a-single-occurrence-in-a-series-by-using-ews"></a>Измените одно вхождение в цикле с помощью веб-служб Exchange

Изменение один экземпляр из серии практически не то же, что изменение встречи один экземпляр. Можно указать вхождение изменение с помощью [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) или элемент [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) . 
  
В следующем примере показано запроса XML при использовании операции [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) обновить вхождения в серии повторяющихся встреч. **Идентификатор элемента** и **ChangeKey** сокращаются для удобства чтения. 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>Helipad of Contoso Bldg 1</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-03-27T19:33:00.000-07:00</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-03-27T20:33:00.000-07:00</t:End>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack@contoso.com</t:Name>
                      <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie@contoso.com</t:Name>
                      <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Magdalena@contoso.com</t:Name>
                      <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso CEO</t:Name>
                      <t:EmailAddress>sadie@contoso</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Research</t:Name>
                      <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Security</t:Name>
                      <t:EmailAddress>alfred@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Weekly Update Meeting:Mandatory</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **UpdateItem** с [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) сообщения, которое содержит значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что этот экземпляр обновлен успешно и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из обновленные встречи. 
  
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Шаблоны повторения и веб-служб Exchange](recurrence-patterns-and-ews.md)
    
- [Доступ к ряду с помощью веб-служб Exchange в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание встречи с помощью веб-служб Exchange в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся с помощью веб-служб Exchange в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

