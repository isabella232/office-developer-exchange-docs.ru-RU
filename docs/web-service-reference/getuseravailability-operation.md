---
title: Операция GetUserAvailability
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailability
api_type:
- schema
ms.assetid: 8da17226-5d3a-4525-9ffa-d83730f47bb1
description: Найдите сведения о веб-служб Exchange GetUserAvailability операции.
ms.openlocfilehash: 41246fe22bfb7444cd4aa7b1d4651d475dd9231c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833686"
---
# <a name="getuseravailability-operation"></a>Операция GetUserAvailability

Найдите сведения о операция **GetUserAvailability** веб-служб Exchange. 
  
Операция **GetUserAvailability** приведены подробные сведения о доступности из набора пользователей, помещений и ресурсов внутри заданного периода времени. 
  
## <a name="using-the-getuseravailability-operation"></a>С помощью операции GetUserAvailability

Операция **GetUserAvailability** предоставляет сведения о доступности текущего пользователя на указанном уровне детализации. Клиентские приложения, такие как Outlook, Outlook Web Access, Outlook Mobile Access и другим пользователям использовать SMTP-адреса для идентификации сведения запрошенного пользователя. 
  
Служба доступности расширяет списки рассылки, чтобы получить состояние сведений о доступности для каждого элемента списка, до тех пор, пока число почтовых ящиков в список рассылки — это меньше, чем 100, максимальное число идентификаторов, **GetUserAvailability **операции можно запросить. Состояния занятости членов списка рассылки будут объединены одного состояния занятости для списка рассылки целиком. 
  
Запросы клиентов приложения укажите период времени доступности запрос. Значение по умолчанию промежуток времени для запрошенные данные — 42 дня. Если календарь пользователя содержит встречи или собрания, которые являются как внутри, так и за пределами за определенный период для запроса, возвращается встречи. 
  
Время встречи и собрания, возвращенных находятся в другом часовом поясе по клиентское приложение, которое запрашивает собрания.
  
Служба доступности обрабатывает запрос для каждого клиента. Служба расширяет повторяющихся встреч и возвращает максимальное количество сведений календаря, для которых есть разрешение на получение запрашивающего клиента.
  
> [!NOTE]
> Если целевой почтовый ящик недоступен или не удается найти, **MailRecipientNotFoundException** исключение. Клиент получает сообщение об ошибке о том, что получатель не найден в службе каталогов Active Directory или доменных служб Active Directory (AD DS). 
  
### <a name="getuseravailability-operation-soap-headers"></a>Заголовки SOAP операция GetUserAvailability

Операция **GetUserAvailability** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения клиента. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Задает заголовок SOAP, который определяет часовой пояс, который будет использоваться для всех ответов с сервера. Все значения времени, возвращаемые с сервера будут преобразованы в указанном часовом поясе. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>Пример запроса GetUserAvailability: получение данных о доступности

В следующем примере запрос операция **GetUserAvailability** показано, как получить сведения о доступности подробные для двух пользователей в часовом поясе по тихоокеанскому времени. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </t:TimeZone>
      <MailboxDataArray>
        <t:MailboxData>
          <t:Email>
            <t:Address>user1@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
        <t:MailboxData>
          <t:Email>
            <t:Address>user2@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
      </MailboxDataArray>
      <t:FreeBusyViewOptions>
        <t:TimeWindow>
          <t:StartTime>2006-10-16T00:00:00</t:StartTime>
          <t:EndTime>2006-10-16T23:59:59</t:EndTime>
        </t:TimeWindow>
        <t:MergedFreeBusyIntervalInMinutes>60</t:MergedFreeBusyIntervalInMinutes>
        <t:RequestedView>DetailedMerged</t:RequestedView>
      </t:FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

Дополнительные сведения о получении предложенного собрания с помощью элемента [SuggestionsViewOptions](suggestionsviewoptions.md) можно схемы в виртуальном каталоге веб-служб Exchange. 
  
Запрос SOAP body содержит следующие элементы:
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
    
- [Часовой пояс (доступность)](timezone-availability.md)
    
- [Смещение (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Уровень защиты](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Месяц](month.md)
    
- [DayOfWeek (часовой пояс)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [MailboxDataArray](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [Электронной почты (EmailAddressType)](email-emailaddresstype.md)
    
- [Адрес (строка)](address-string.md)
    
- [AttendeeType](attendeetype.md)
    
- [ExcludeConflicts](excludeconflicts.md)
    
- [FreeBusyViewOptions](freebusyviewoptions.md)
    
- [Значение TimeWindow](timewindow.md)
    
- [Время начала](starttime.md)
    
- [Время окончания](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>Успешного ответа операция GetUserAvailability

В следующем примере показано успешного ответа на запрос операция **GetUserAvailability** . 
  
> [!NOTE]
> Идентификаторы событий календаря URL-были сокращены, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T06:00:00-07:00</StartTime>
                <EndTime>2006-10-16T06:30:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0</ID>
                  <Subject>Meet with Contoso Account Executives</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T07:00:00-07:00</StartTime>
                <EndTime>2006-10-16T08:00:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>E14B6414B0B</ID>
                  <Subject>Pick up my groceries</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T09:40:00-07:00</StartTime>
                <EndTime>2006-10-16T10:10:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0B1</ID>
                  <Subject>Meet with doctor</Subject>
                  <Location>Kirkland</Location>
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
      </FreeBusyResponseArray>
    </GetUserAvailabilityResponse>
  </soap:Body>
</soap:Envelope>
```

Сведения о доступности для каждого пользователя отображается в элементе уникальный [FreeBusyResponse](freebusyresponse.md) . Порядок пользователей в запросе операция **GetUserAvailability** определяет приоритет данных о доступности для каждого пользователя в ответе. 
  
Ошибка будут возвращены клиенту, если число встреч в период времени, определенного в запросе превышает максимальное время, указанное администратором. По умолчанию максимальное число встреч — 10 000 отдельные экземпляры и расширенное повторяющихся элементов. Это свойство можно настроить только администратором.
  
В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
    
- [FreeBusyResponseArray](freebusyresponsearray.md)
    
- [FreeBusyResponse](freebusyresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [FreeBusyView](freebusyview.md)
    
- [FreeBusyViewType](freebusyviewtype.md)
    
- [MergedFreeBusy](mergedfreebusy.md)
    
- [CalendarEventArray](calendareventarray.md)
    
- [CalendarEvent](calendarevent.md)
    
- [Время начала](starttime.md)
    
- [Время окончания](endtime.md)
    
- [BusyType](busytype.md)
    
- [CalendarEventDetails](calendareventdetails.md)
    
- [ИД](id.md)
    
- [Тема (CalendarEventDetails)](subject-calendareventdetails.md)
    
- [Расположение (CalendarEventDetails)](location-calendareventdetails.md)
    
- [IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)
    
- [IsException](isexception.md)
    
- [IsReminderSet](isreminderset.md)
    
- [IsPrivate](isprivate.md)
    
- [WorkingHours](workinghours-ex15websvcsotherref.md)
    
- [Часовой пояс (доступность)](timezone-availability.md)
    
- [Смещение (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Уровень защиты](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Месяц](month.md)
    
- [DayOfWeek (часовой пояс)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [WorkingPeriodArray](workingperiodarray.md)
    
- [WorkingPeriod](workingperiod.md)
    
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
    
- [StartTimeInMinutes](starttimeinminutes.md)
    
- [EndTimeInMinutes](endtimeinminutes.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

