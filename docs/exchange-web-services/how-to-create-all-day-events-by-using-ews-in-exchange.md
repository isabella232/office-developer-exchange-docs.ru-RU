---
title: Создание событий на целый день с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Узнайте, как создавать события на целый день с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 6be638c17cc0e0c86fa6b4217169aa7259dfd4aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456866"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Создание событий на целый день с помощью EWS в Exchange

Узнайте, как создавать события на целый день с помощью управляемого API EWS или EWS в Exchange.
  
События на целый день представляют собой способ представления какого-либо действия за целый день или несколько дней (например, праздничный день или дни отпуска). Создание событий на целый день с помощью управляемого API EWS или EWS является привязкой. Это так же, как [Создание встреч](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), но с несколькими небольшими изменениями.
  
## <a name="setting-start-and-end-times"></a>Установка времени начала и окончания

По определению, события на целый день начинаются с полуночи в определенный день и заканчиваются 24 часа (или несколько минут в 24 часа). Тем не менее, управляемый API EWS и EWS позволяют указать время, отличное от полуночи, при создании событий на целый день. Это может привести к нежелательному поведению, если вы не помните о том, как эти времена будут переведены на сервер.
  
При получении запроса на создание нового события на целый день без полуночи (в часовом [поясе запроса или встречи](time-zones-and-ews-in-exchange.md)) эти времена корректируются до полуночи в соответствующем часовом поясе в соответствии со следующими правилами:
  
- Время начала не в полночь регулируется до полуночи до указанного времени. Например, 1:00 PM на 6 июня будет изменено на 12:00 AM 6 июня.
    
- Время окончания не в полночь регулируется до полуночи по истечении указанного времени. Например, 1:00 PM на 6 июня будет скорректировано до версии 12:00 AM 7 июня.
    
Поэтому создаваемое событие на целый день всегда является инклюзивным с указанным временем начала и окончания, но может потребовать дополнительного времени в календаре пользователя из-за смены в полночь. Так как на сервере будет задано время начала и окончания, рекомендуется указать время начала и окончания на полночь, чтобы избежать нежелательных изменений.
  
Кроме того, важно учитывать часовые пояса при создании событий на целый день. Так как сервер Exchange применяет время начала и окончания полуночи в часовом поясе запроса или встречи, просмотр этого события на весь день в клиенте, настроенном для другого часового пояса, может привести к непредвиденным результатам. В зависимости от клиента он может отображаться как событие на целый день с дополнительными днями, которые не планировалось включать, или вообще не отображаться как событие на целый день. В связи с этим мы рекомендуем использовать предпочтительный часовой пояс пользователя, когда это возможно, при создании событий на целый день.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Создание события на целый день с помощью управляемого API EWS

В приведенном ниже примере показано, как использовать управляемый API EWS для создания события на целый день, начиная с даты, указанной параметром _StartDate_ , и зафиксированной в течение числа дней, заданного параметром _нумдайс_ . Обратите внимание, что встреча будет создана в часовом поясе, указанном в свойстве [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . В этом примере предполагается, что объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , переданный в параметре _Service_ , инициализирован с допустимыми значениями для свойств [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a>Создание события на целый день с помощью EWS

В следующем примере показан запрос [операции CREATEITEM](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для создания события на целый день. Встреча создается в Восточном часовом поясе, как указано в элементе [тимезонеконтекст](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) . Обратите внимание, что в качестве части значений [начального](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [конечного](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) элементов указаны оба значения 04:00Z, которые преобразуются в полночь в Восточном часовом поясе во время летнего времени. 
  
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
    

