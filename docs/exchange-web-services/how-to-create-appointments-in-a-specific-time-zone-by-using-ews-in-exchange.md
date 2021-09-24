---
title: Создание встречи в определенном часовом поясе с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Узнайте, как создавать встречи в определенных часовых поясах с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: 589c72982fdda568170468c376b8a6d9f598aa36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521146"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Создание встречи в определенном часовом поясе с помощью EWS в Exchange

Узнайте, как создавать встречи в определенных часовых поясах с помощью управляемого API или EWS EWS в Exchange.
  
При создании встречи или собрания для календаря Exchange часовой пояс, используемый для указания времени начала и окончания, сохраняется как часовой пояс создания встречи. Этот часовой пояс [](time-zones-and-ews-in-exchange.md)также используется для интерпретации значений даты и времени, не заданных явного часового пояса, поэтому важно понимать параметры для указания часового пояса.
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>Создание встреч в разных часовых поясах с помощью управляемого API EWS

При создании встреч или собраний с помощью управляемого API EWS у вас есть три варианта указания часовой пояс:
  
- Чтобы использовать часовой пояс компьютера, на котором выполняется управляемый API EWS, не укажите часовой пояс при создании объекта [ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) 
    
- Чтобы использовать определенный часовой пояс для всех свойств даты и времени, включая свойства при создании новой встречи или собрания, укажите часовой пояс в конструкторе объекта **ExchangeService.** 
    
- Чтобы использовать другой часовой пояс, чем указанный в свойстве [ExchangeService.TimeZone,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) используйте свойства [Appointment.StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) и [Appointment.EndTimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) 
    
    > [!NOTE]
    > Свойство **EndTimeZone** доступно только в том случае, если свойство [ExchangeService.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) настроено на **Exchange2010** или более поздней версии. Если она недоступна, настройка **StartTimeZone** применяется как к началу, так и к конечному времени встречи. 
  
В следующем примере управляемый API EWS используется для создания трех встреч. Каждая встреча начнется в 13:00 через два дня в неустановленном часовом поясе и завершится через час. Первая встреча создается в часовом поясе клиентского компьютера с помощью поведения управляемого API EWS по умолчанию. Второй создается в центральном часовом поясе с помощью свойств **Appointment.StartTimeZone** и **Appointment.EndTimeZone.** Третий создается в часовом поясе Горы с помощью свойства **ExchangeService.TimeZone.** 
  
```cs
using Microsoft.Exchange.WebServices.Data;
using System.Security;
static void CreateAppointments(string userEmail, SecureString userPass)
{
    // *****************************************************
    // Create an appointment using the client computer's time zone.
    // *****************************************************
    // Do not specify a time zone when creating the ExchangeService.
    ExchangeService clientTZService = new ExchangeService(ExchangeVersion.Exchange2010);
    clientTZService.Credentials = new NetworkCredential(userEmail, userPass);
    clientTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment clientTZAppt = new Appointment(clientTZService);
    clientTZAppt.Subject = "Appointment created using client time zone";
    clientTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", clientTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    DateTime startTime = new DateTime(DateTime.Now.Year, DateTime.Now.Month, DateTime.Now.Day + 2);
    startTime = startTime.AddHours(13);
    clientTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    DateTime endTime = startTime.AddHours(1);
    clientTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        clientTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Central time zone by
    // using the StartTimeZone property.
    // *****************************************************
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Create the appointment.
    Appointment centralTZAppt = new Appointment(clientTZService);
    centralTZAppt.Subject = "Appointment created using Central time zone";
    centralTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", centralTZ.DisplayName));
    // Set the time zone on the appointment.
    centralTZAppt.StartTimeZone = centralTZ;
    centralTZAppt.EndTimeZone = centralTZ;
    // Set the start time to 1:00 PM two days from today.
    centralTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    centralTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        centralTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Mountain time zone by
    // using the ExchangeService.TimeZone property.
    // *****************************************************
    // Specify the Mountain time zone when creating the ExchangeService.
    TimeZoneInfo mountainTZ = TimeZoneInfo.FindSystemTimeZoneById("Mountain Standard Time");
    ExchangeService mountainTZService = new ExchangeService(ExchangeVersion.Exchange2010, mountainTZ);
    mountainTZService.Credentials = new NetworkCredential(userEmail, userPass);
    mountainTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment mountainTZAppt = new Appointment(mountainTZService);
    mountainTZAppt.Subject = "Appointment created using Mountain time zone";
    mountainTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", mountainTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    mountainTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    mountainTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        mountainTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
}
```

Когда этот пример выполняется на клиентской компьютере, настроенной в восточном часовом поясе, и три встречи, которые он создает, просматриваются из клиента, настроенного в восточном часовом поясе, они отображаются в 13:00, 14:00 и 15:00 соответственно.
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>Создание встреч в разных часовых поясах с помощью EWS

При создании встреч или собраний с помощью EWS у вас есть три варианта указания часовой пояс:
  
- Чтобы использовать скоординированное универсальное время (UTC), не включайте элемент [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) элемент [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (только Exchange 2007 г.) или элементы [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) и [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 г. и более поздний период) в запрос операции [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Чтобы использовать определенный часовой пояс для всех свойств даты и времени, включая свойства при создании новой встречи или собрания, укажите часовой пояс в [элементе TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) в запросе операции [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Чтобы использовать другой часовой пояс, чем указанный в элементе [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) включите элемент [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) элемент [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (только Exchange 2007 г.) или элементы [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) и [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 г. и более поздний период) в запросе на операцию [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
В следующем примере запрос на операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) создает встречу с помощью UTC. Обратите внимание, что элемент **TimeZoneContext,** элемент **StartTimeZone** и **элемент EndTimeZone** отсутствуют. Значения **элементов** Start и **End** выражаются в UTC. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using UTC</t:Subject>
          <t:Body BodyType="HTML">Time zone: UTC</t:Body>
          <t:Start>2014-06-07T17:00:00.000Z</t:Start>
          <t:End>2014-06-07T18:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере запрос на операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) использует элементы **StartTimeZone** и **EndTimeZone** для указания центрального часовой пояс для встречи. Обратите внимание, **что элемент TimeZoneContext** отсутствует. Однако, если он присутствует, значения элементов **StartTimeZone** и **EndTimeZone** переопределяли бы его значение. Опять же, **значения элементов Начните** и **End** выражены в UTC. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Central time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-06:00) Central Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T18:00:00.000Z</t:Start>
          <t:End>2014-06-07T19:00:00.000Z</t:End>
          <t:StartTimeZone Id="Central Standard Time" />
          <t:EndTimeZone Id="Central Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере [запрос операции CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) задает элемент **TimeZoneContext** в часовой пояс Mountain. Обратите внимание, что **элементы StartTimeZone** и **EndTimeZone** отсутствуют. Опять же, **значения элементов Начните** и **End** выражены в UTC. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Mountain Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Mountain time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-07:00) Mountain Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T19:00:00.000Z</t:Start>
          <t:End>2014-06-07T20:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Когда три встречи, созданные предыдущими запросами на примере EWS, рассматриваются клиентом, настроенным в восточном часовом поясе, они отображаются в 13:00, 14:00 и 15:00 соответственно.
  
## 

Теперь, когда вы знаете, как создавать встречи в [](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) определенных часовых поясах, может потребоваться обновить часовые пояса на существующих встречах до другого. 
  
## <a name="see-also"></a>См. также


- [Часовые пояса и EWS в Exchange](time-zones-and-ews-in-exchange.md)
    
- [Обновление часового пояса встречи с помощью EWS в Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013 г.](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

