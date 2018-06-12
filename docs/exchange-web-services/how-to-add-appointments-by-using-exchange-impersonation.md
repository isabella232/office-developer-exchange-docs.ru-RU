---
title: Добавление встреч с использованием олицетворения Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Узнайте, как использовать олицетворение управляемый API EWS или веб-служб Exchange в Exchange на добавление встреч календарей пользователей.
ms.openlocfilehash: fe737658b88aca66d8b4c2860245db000888ba17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760997"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Добавление встреч с использованием олицетворения Exchange

Узнайте, как использовать олицетворение управляемый API EWS или веб-служб Exchange в Exchange на добавление встреч календарей пользователей.
  
Можно создать приложения-службы, которая вставляет встреч непосредственно в календаре Exchange с помощью учетной записи службы, имеющей[роли включены](how-to-configure-impersonation.md) **AppplicationImpersonation**. При использовании олицетворения приложения используется в качестве пользователя; Это, как если бы пользователь добавлен встречи календаря с помощью клиента, такие как Outlook. 
  
При использовании олицетворения необходимо учитывать следующее:
  
- Объект [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) должен быть привязан к учетной записи службы. Можно использовать один и тот же объект **ExchangeService** для олицетворения нескольких учетных записей с помощью изменения свойства [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для каждой учетной записи, которую требуется олицетворения. 
    
- Любой элемент, сохранять олицетворенным учетной записи может использоваться только один раз. Если вы хотите сохранить же встречу в нескольких учетных записей, например, необходимо создать [объект для каждой учетной записи](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) . 
    
## <a name="prerequisites"></a>Необходимые компоненты

Приложению учетной записи, используемой для подключения к Exchange server для использования олицетворения. Рекомендуется использовать учетную запись службы для приложения, которому назначена роль олицетворения приложения для учетных записей, которые будут пользоваться. Дополнительные сведения можно [настроить олицетворения](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Добавление встреч с использованием олицетворения с помощью управляемого интерфейса API веб-служб Exchange

В следующем примере добавляется встречи или собрания в календарь одного или нескольких учетных записей Exchange. Метод принимает три параметра.
  
-  _Служба_ — объект **ExchangeService** привязан к учетной записи приложения-службы на сервере Exchange. 
    
-  _emailAddresses_ — [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object, содержащий список строк адресов электронной почты SMTP. 
    
-  _фабрика_ — это объект, реализующий интерфейс **IAppointmentFactory** . Этот интерфейс содержит один метод **GetAppointment** , который принимает объект **ExchangeService** как параметр и возвращает объект **встречи** . Интерфейс **IAppointmentFactory** определен [интерфейс IAppointmentFactory](#bk_IAppointmentFactory).
    
```cs
private static void CreateAppointments(ExchangeService service, List<string> emailAddresses, IAppointmentFactory factory)
{
  // Loop through the list of email addresses to add the appointment.
  foreach (var emailAddress in emailAddresses)
  {
    Console.WriteLine(string.Format("  Placing appointment in calendar for {0}.", emailAddress));
    // Set the email address of the account to get the appointment.
    service.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, emailAddress);
    // Get the appointment to add.
    Appointment appointment = factory.GetAppointment(service);
    // Save the appointment.
    try
    {
      if (appointment.RequiredAttendees.Count > 0)
      {
        // The appointment has attendees so send them the meeting request.
        appointment.Save(SendInvitationsMode.SendToAllAndSaveCopy);
      }
      else
      {
        // The appointment does not have attendees, so just save to calendar.
        appointment.Save(SendInvitationsMode.SendToNone);
      }
    }
    catch (ServiceResponseException ex)
    {
      Console.WriteLine(string.Format("Could not create appointment for {0}", emailAddress));
      Console.WriteLine(ex.Message);
    }
  }
}
```

При сохранении встречи, код проверяется ли свойство [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) были добавлены участников собрания. Если у них есть метод [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) вызывается с значение перечисления [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы участники получают приглашения на собрания; в противном случае метод **Appointment.Save** вызывается с значение перечисления [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы встречи сохраняется в календарь для олицетворения пользователя с помощью свойства [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) значение **false**.
  
### <a name="iappointmentfactory-interface"></a>Интерфейс IAppointmentFactory
<a name="bk_IAppointmentFactory"> </a>

Так как новый объект **встречи** требуется каждый раз, когда вы хотите сохранить встречу в календаре олицетворения пользователя, интерфейс **IAppointmentFactory** выделяет объект, используемый для заполнения каждого объекта **встречи** . Эта версия — это простой интерфейс, который содержит только один метод, **GetAppointment**, который принимает объект **ExchangeService** как параметр и возвращает объект новой **встречи** , привязанные к объекту **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

В следующем примере класс **AppointmentFactory** показано, что реализацию интерфейса **IAppointmentFactory** , которое возвращает простой встречи, которая происходит через три дня. При раскомментировании `appointment.RequiredAttendees.Add` строку, **GetAppointment** метод возвратит собрания и адрес электронной почты, указанных в том, что строка будет получать приглашения на собрание с олицетворенным пользователем, указано, что организатора. 
  
```cs
class AppointmentFactory : IAppointmentFactory
{
  public Appointment GetAppointment(ExchangeService service)
  {
    // First create the appointment to add.
    Appointment appointment = new Appointment(service);
    // Set the properties on the appointment.
    appointment.Subject = "Tennis lesson";
    appointment.Body = "Focus on backhand this week.";
    appointment.Start = DateTime.Now.AddDays(3);
    appointment.End = appointment.Start.AddHours(1);
    appointment.Location = "Tennis club";
    // appointment.RequiredAttendees.Add(new Attendee("sonyaf@contoso1000.onmicrosoft.com"));
    return appointment;
  }
}

```

## <a name="add-appointments-by-using-impersonation-with-ews"></a>Добавление встреч с использованием олицетворения с помощью веб-служб Exchange

Веб-служб Exchange позволяет приложения для использования олицетворения для добавления элементов в календаре от имени владельца календаря. В этом примере показано, как использовать операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для добавления встречи в календаре олицетворенным учетной записи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Обратите внимание на то, что кроме элемента **ExchangeImpersonation** в заголовке SOAP, чтобы указать учетную запись, мы олицетворения это же запрос XML, используемые для создания встречи без использования олицетворения. 
  
В следующем примере показано XML, возвращенные операцией **CreateItem** ответа. 
  
> [!NOTE]
> Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

Опять же это же XML-ФАЙЛ, который возвращается при использовании операции **CreateItem** без использования олицетворения. 
  
## <a name="see-also"></a>См. также


- [Олицетворение и EWS в Exchange](impersonation-and-ews-in-exchange.md)
    
- [Роль ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [Настройка олицетворения](how-to-configure-impersonation.md)
    
- [Идентификация учетной записи для олицетворения](how-to-identify-the-account-to-impersonate.md)
    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Операции CreateItem (элемента календаря)](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [Свойство ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    

