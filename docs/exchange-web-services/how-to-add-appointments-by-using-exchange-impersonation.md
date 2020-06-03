---
title: Добавление встреч с помощью олицетворения Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Узнайте, как использовать олицетворение с помощью управляемого API EWS или EWS в Exchange для добавления встреч в календари пользователей.
localization_priority: Priority
ms.openlocfilehash: b1473d72113f8cc07d05364a4d87fedf23c7351d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455333"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Добавление встреч с помощью олицетворения Exchange

Узнайте, как использовать олицетворение с помощью управляемого API EWS или EWS в Exchange для добавления встреч в календари пользователей.
  
Вы можете создать приложение службы, которое вставляет встречи непосредственно в календарь Exchange, используя учетную запись службы с [включенной ролью](how-to-configure-impersonation.md) **ApplicationImpersonation** . При использовании олицетворения приложение выступает в роли пользователя; Это так, как если бы пользователь добавил встречу в календарь с помощью клиента, например Outlook. 
  
При использовании олицетворения учитывайте следующие моменты.
  
- Объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) должен быть связан с учетной записью службы. Вы можете использовать один и тот же объект **ExchangeService** для олицетворения нескольких учетных записей, изменив свойство [имперсонатедусерид](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для каждой учетной записи, для которой необходимо выполнить олицетворение. 
    
- Любой элемент, сохраненный для олицетворенной учетной записи, можно использовать только один раз. Если вы хотите сохранить одну и ту же встречу в нескольких учетных записях, например, необходимо создать объект [встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) для каждой учетной записи. 
    
## <a name="prerequisites"></a>Необходимые компоненты

Для подключения к серверу Exchange приложение должно использовать учетную запись, прежде чем она сможет использовать олицетворение. Мы рекомендуем использовать учетную запись службы для приложения, которому была предоставлена роль олицетворения приложения для учетных записей, к которым будет осуществляться доступ. Дополнительные сведения см в разделе [Настройка олицетворения](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Добавление встреч с помощью олицетворения с помощью управляемого API EWS

В приведенном ниже примере показано, как добавить встречу или собрание в календарь одной или нескольких учетных записей Exchange. Метод принимает три параметра.
  
-  _Service_ — объект **ExchangeService** , привязанный к учетной записи приложения-службы на сервере Exchange. 
    
-  _EmailAddresses_ — объект [System. List](https://msdn.microsoft.com/library/6sh2ey19.aspx) , содержащий список строк адресов электронной почты SMTP. 
    
-  _фабрика_ — объект, который реализует интерфейс **иаппоинтментфактори** . Этот интерфейс содержит один **метод, метод ExchangeService, который** принимает объект **ExchangeService** в качестве параметра и возвращает объект **встречи** . Интерфейс **иаппоинтментфактори** определяется [интерфейсом иаппоинтментфактори](#bk_IAppointmentFactory).
    
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

При сохранении встречи код проверяет, добавлены ли какие бы то ни было участников в свойство [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) . В противном случае метод [встреча. Save](https://msdn.microsoft.com/library/dd635394.aspx) вызывается со значением перечисления [сендтоалландсавекопи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы участники получали приглашения на собрания; в противном случае метод **встреча. Save** вызывается со значением перечисления [сендтононе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы сохранить встречу в календаре олицетворенного пользователя с помощью свойства [Meeting.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) IsFalse, равное **false**.
  
### <a name="iappointmentfactory-interface"></a>Интерфейс Иаппоинтментфактори
<a name="bk_IAppointmentFactory"> </a>

Так как для сохранения встречи в календаре олицетворенного пользователя необходим новый объект **встречи** , интерфейс **иаппоинтментфактори** абстрагирует объект, используемый для заполнения каждого объекта " **встреча** ". Эта версия представляет собой простой интерфейс, который содержит только один метод, метод- **встречу**, который принимает объект **ExchangeService** в качестве параметра и возвращает новый объект **встречи** , привязанный к этому объекту **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

В приведенном ниже примере класса **аппоинтментфактори** показана реализация интерфейса **иаппоинтментфактори** , который возвращает простую встречу, которая находится в течение трех дней с этого момента. Если вы раскомментируйте `appointment.RequiredAttendees.Add` строку, метод **GetAppointment** "метод" будет возвращать собрание, а адрес электронной почты, указанный в этой строке, будет получать приглашение на собрание с олицетворенным пользователем, указанным в качестве организатора. 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a>Добавление встреч с помощью службы EWS с помощью олицетворения

С помощью служб EWS вы можете использовать олицетворение для добавления элементов в календарь от имени владельца календаря. В этом примере показано, как с помощью операции [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) добавить встречу в календарь олицетворенной учетной записи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Обратите внимание, что кроме добавления элемента **ексчанжеимперсонатион** в заголовке SOAP для указания учетной записи, которую вы олицетворять, это тот же XML-запрос, который используется для создания встречи без использования олицетворения. 
  
В следующем примере показан XML-код отклика, возвращаемый операцией **CreateItem** . 
  
> [!NOTE]
> Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

Опять же, это тот же XML-код, который возвращается при использовании операции **CreateItem** без олицетворения. 
  
## <a name="see-also"></a>См. также


- [Олицетворение и EWS в Exchange](impersonation-and-ews-in-exchange.md)
    
- [Роль ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)
    
- [Настройка олицетворения](how-to-configure-impersonation.md)
    
- [Идентификация учетной записи для олицетворения](how-to-identify-the-account-to-impersonate.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Операция CreateItem (элемент календаря)](../web-service-reference/createitem-operation-calendar-item.md)
    
- [Свойство ExchangeService. Имперсонатедусерид](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    

