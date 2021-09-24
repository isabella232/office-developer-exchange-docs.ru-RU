---
title: Создание событий в течение дня с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Узнайте, как создавать события в течение дня с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 8769999907df46f519355a36fdf409f9ad347330
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521223"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Создание событий в течение дня с помощью EWS в Exchange

Узнайте, как создавать события в течение дня с помощью управляемого API EWS или EWS в Exchange.
  
События, которые проводятся в течение всего дня или нескольких дней, — например, праздник или дни отпуска. Создание событий в течение дня с управляемым API EWS или EWS — это простое решение. Это так же, как [создание встреч,](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)но с несколькими небольшими изменениями.
  
## <a name="setting-start-and-end-times"></a>Настройка времени начала и окончания

По определению события в течение всего дня начинаются в полночь в определенный день и заканчиваются через 24 часа (или несколько часов). Однако управляемый API и EWS EWS позволяют указать время, помимо полуночи, при создании событий в течение всего дня. Это может привести к непреднамеренному поведению, если вы не знаете, как эти времена переводятся на сервере.
  
При получении запроса на создание нового события в течение всего дня с не-полуночью (в часовом поясе запроса или [встречи)](time-zones-and-ews-in-exchange.md)время начала и/или окончания, эти времена корректируются до полуночи в соответствующем часовом поясе в соответствии со следующими правилами:
  
- Время начала до полуночи корректируется до полуночи до указанного времени. Например, с 13:00 6 июня корректируется до 12:00 6 июня.
    
- Время окончания полуночи корректируется до полуночи после указанного времени. Например, с 13:00 6 июня корректируется до 12:00 7 июня.
    
Поэтому событие, которое вы создаете в течение всего дня, всегда включено в время начала и окончания, которое вы указываете, но может требовать дополнительного времени в календаре пользователя из-за перехода на полночь. Поскольку сервер будет настраивать время начала и окончания до полуночи, рекомендуется указать время начала и окончания в полночь, чтобы избежать непредвиденных изменений времени.
  
Также важно учитывать часовые пояса при создании событий в течение дня. Поскольку сервер Exchange обеспечивает время начала и окончания полуночи в часовом поясе запроса или встречи, просмотр события в клиенте, настроенном для другого часового пояса, может привести к неожиданным результатам. В зависимости от клиента оно может отображаться как событие на весь день с дополнительными днями, которые вы не собирались включать, или оно может вообще не отображаться как событие на весь день. В связи с этим рекомендуется использовать предпочитаемый часовой пояс пользователя при создании событий в течение всего дня.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Создание события в течение дня с помощью управляемого API EWS

В следующем примере показано, как использовать управляемый API EWS для создания события в течение всего дня, начиная с даты, указанной параметром _startDate,_ и продолжительной в течение количества дней, заданных параметром _numDays._ Обратите внимание, что встреча будет создана в часовом поясе, указанном [свойством ExchangeService.TimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) В этом примере предполагается, что  объект [ExchangeService,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) переданный в параметре службы, инициализирован с допустимым значением для свойств [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) 
  
```cs
static void CreateAllDayAppointment(ExchangeService service, DateTime startDate, int numDays)
{
    // Best practice is to set the start date to midnight
    // on the first day of the all-day event.
    DateTime startDateMidnight = startDate.Date;
    // The end date should be midnight on the first day
    // after the event.
    DateTime endDateMidnight = startDateMidnight.AddDays(numDays);
    Appointment allDayEvent = new Appointment(service);
    // Set IsAllDayEvent to true.
    allDayEvent.IsAllDayEvent = true;
    // Set other properties.
    allDayEvent.Subject = "Vacation";
    allDayEvent.LegacyFreeBusyStatus = LegacyFreeBusyStatus.OOF;
    allDayEvent.Start = startDateMidnight;
    allDayEvent.End = endDateMidnight;
    // Save the appointment.
    try
    {
        allDayEvent.Save(WellKnownFolderName.Calendar, SendInvitationsMode.SendToNone);
        Console.WriteLine("All day event created.");
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving all day event: {0}", ex.Message);
    }
}
```

## <a name="create-an-all-day-event-by-using-ews"></a>Создание события в течение дня с помощью EWS

В следующем примере показан запрос на операцию EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания события на весь день. Назначение создается в восточном часовом поясе, как указывает элемент [TimeZoneContext.](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) Обратите внимание, что временная часть значений элементов Start [и](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) — это 04:00Z, который преобразуется в полночь в восточном часовом поясе во время летнего времени. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Vacation</t:Subject>
          <t:Start>2014-06-09T04:00:00.000Z</t:Start>
          <t:End>2014-06-10T04:00:00.000Z</t:End>
          <t:IsAllDayEvent>true</t:IsAllDayEvent>
          <t:LegacyFreeBusyStatus>OOF</t:LegacyFreeBusyStatus>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Часовые пояса и EWS в Exchange](time-zones-and-ews-in-exchange.md)
    

