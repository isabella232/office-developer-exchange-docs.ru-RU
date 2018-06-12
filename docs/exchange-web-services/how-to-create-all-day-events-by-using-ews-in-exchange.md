---
title: Создание событий на целый день с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Сведения о создании событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 0547fdf0ca92ba0648caeb5de6940d90d2a8ff46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760989"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Создание событий на целый день с помощью веб-служб Exchange в Exchange

Сведения о создании событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
События предусмотрена возможность представления, которое происходит для целый день или несколько дней — например, в выходные дни и даже дней отпуска. Создание событий на целый день с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange — это просто. Это так же, как [Создание встреч](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), но с небольшие изменения.
  
## <a name="setting-start-and-end-times"></a>Установка времени начала и завершения

По определению, запустите событий на целый день в полночь на определенный день и конечных 24 часа (или несколько 24 часов) более поздней версии. Тем не менее, управляемый API EWS и веб-служб Exchange позволяют указать время, отличный от полуночи при создании события на целый день. Это может привести к непредвиденным поведение, если вы не знать о том, как это время получения преобразовываться на сервере.
  
При получении запроса Чтобы создать новое событие на целый день с начала не полночь (в [часовой пояс запроса или встреча](time-zones-and-ews-in-exchange.md)) и/или время окончания, то время, получение настроено в полночь в соответствующие часовой пояс определяется следующими правилами:
  
- Время начала полночь не настроены на полночь до указанного времени. Например 1:00 PM на 6 июня получает настроенные до 12:00 на 6 июня.
    
- Время окончания полночь не настроены на полночь после указанного времени. Например 1:00 PM на 6 июня получает настроенные до 12:00 на 7 июня.
    
Поэтому всегда включая время начала и окончания, укажите, но может затребовать дополнительное время на события, создаваемого пользователя 's календаря из-за shift до полуночи. Так как сервер будет настроить время начала и окончания полночь, рекомендуется указать времени начала и окончания в полночь, чтобы избежать непреднамеренного изменения значения времени.
  
Также важно учесть часовые пояса при создании событий на целый день. Так как Exchange server обеспечивает полночь начала и окончания времени в часовом поясе запроса или встречи, просмотр, целый день в клиент, настроенный для различных часового пояса может привести к непредсказуемым последствиям. В зависимости от клиента она может оказаться событием на целый день с помощью дополнительных дней, которые не будут включать или она может не отображаться в событием на целый день полностью. Таким образом мы рекомендуем использовать предпочтительный часовой пояс пользователя по возможности при создании событий на целый день.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Создание событием на целый день с помощью управляемого интерфейса API веб-служб Exchange

Следующем примере показано, как использовать управляемый API веб-служб Exchange для создания событием на целый день, начиная с даты, указанного с помощью параметра _startDate_ и выполняемых числа дней, указанных в параметре _numDays_ . Обратите внимание, что в часовом поясе, указанном свойством [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) будет создано встречи. В этом примере предполагается, что объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , переданной в параметре _службы_ была ли инициализирована на допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a>Создание событием на целый день с помощью веб-служб Exchange

В следующем примере показано запрос веб-служб Exchange [операции CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания событием на целый день. Встречи создается по восточному поясному времени, как указано в элементе [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) . Обратите внимание, что время часть значения элементов [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) обоих 04:00Z, который преобразует в полночь в по восточному поясному времени во время перехода на летнее время. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Часовые пояса и EWS в Exchange](time-zones-and-ews-in-exchange.md)
    

