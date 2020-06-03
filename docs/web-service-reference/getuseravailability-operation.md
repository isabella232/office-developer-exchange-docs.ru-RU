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
description: Поиск сведений о GetUserAvailabilityной операции EWS.
ms.openlocfilehash: b6d03c7da65e3f30f093b7e41448abcca2330a84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458224"
---
# <a name="getuseravailability-operation"></a>Операция GetUserAvailability

Поиск сведений о **GetUserAvailabilityной** операции EWS. 
  
Операция **GetUserAvailability** предоставляет подробные сведения о доступности набора пользователей, помещений и ресурсов в течение заданного периода времени. 
  
## <a name="using-the-getuseravailability-operation"></a>Использование операции GetUserAvailability

Операция **GetUserAvailability** предоставляет сведения о доступности текущих пользователей на указанном уровне детализации. Клиентские приложения, такие как Outlook, Outlook Web Access, Outlook Mobile Access и другие, используют адреса SMTP для идентификации запрашиваемых сведений о пользователях. 
  
Служба доступности расширяет списки рассылки для получения сведений о доступности для каждого участника списка, если количество почтовых ящиков в списке рассылки меньше 100, что является максимальным количеством идентификаторов, которые может запросить операция **GetUserAvailability** . Сведения о доступности участников списка рассылки объединяются в один статус занятости для всего списка рассылки. 
  
В запросах клиентского приложения указывается период времени, в течение которого запрос доступности. По умолчанию для запрашиваемых сведений используется период времени 42 дней. Если календарь пользователя содержит встречи или собрания, которые находятся в определенном периоде времени и не выходят за него, возвращается встреча. 
  
Возвращаемые время встреч и собраний находятся в том же часовом поясе, что и клиентское приложение, запрашивающее собрание.
  
Служба доступности обрабатывает запрос для каждого клиента. Служба развертывает все повторяющиеся встречи и возвращает максимальное количество сведений о календаре, которое у запрашивающего клиента имеет разрешение на получение.
  
> [!NOTE]
> Если целевой почтовый ящик недоступен или не может быть найден, создается исключение **маилреЦипиентнотфаундексцептион** . Клиент получает сообщение об ошибке, в котором говорится, что получатель не найден в службе каталогов Active Directory или в доменных службах Active Directory (AD DS). 
  
### <a name="getuseravailability-operation-soap-headers"></a>Заголовки SOAP операции GetUserAvailability

Операция **GetUserAvailability** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Определяет пользователя, который олицетворяет клиент. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
|**тимезонеконтекст** <br/> |[тимезонеконтекст](timezonecontext.md) <br/> |Указывает заголовок SOAP, определяющий часовой пояс, который будет использоваться для всех ответов сервера. Все значения времени, возвращаемые с сервера, будут преобразованы в указанный часовой пояс. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>Пример запроса GetUserAvailability: получение сведений о доступности

В приведенном ниже примере запроса операции **GetUserAvailability** показано, как получить подробные сведения о доступности для двух пользователей в часовом поясе по тихоокеанскому времени. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Дополнительные сведения о получении предложенных собраний с помощью элемента [сугжестионсвиевоптионс](suggestionsviewoptions.md) можно найти в схеме в виртуальном каталоге EWS. 
  
Текст SOAP Request содержит следующие элементы:
  
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
    
- [Часовой пояс (доступность)](timezone-availability.md)
    
- [Сдвиг (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [дайордер](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (TimeZone)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [маилбоксдатааррай](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [Электронная почта (EmailAddressType)](email-emailaddresstype.md)
    
- [Address (строка)](address-string.md)
    
- [AttendeeType](attendeetype.md)
    
- [ексклудеконфликтс](excludeconflicts.md)
    
- [фрибусивиевоптионс](freebusyviewoptions.md)
    
- [TimeWindow](timewindow.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>Успешный отклик операции GetUserAvailability

В следующем примере показан успешный ответ на запрос операции **GetUserAvailability** . 
  
> [!NOTE]
> Идентификаторы событий календаря были сокращены для сохранения удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Сведения о доступности для каждого пользователя отображаются в уникальном элементе [фрибусиреспонсе](freebusyresponse.md) . Порядок пользователей в запросе операции **GetUserAvailability** определяет порядок данных о доступности для каждого пользователя в отклике. 
  
В клиенте возвращается сообщение об ошибке, если количество встреч в периоде времени, определенном в запросе, превышает максимальное число, указанное администратором. По умолчанию максимальное число встреч составляет 10 000 одиночных экземпляров и расширенных элементов повторения. Это свойство можно настроить только администратором.
  
В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
    
- [фрибусиреспонсеаррай](freebusyresponsearray.md)
    
- [фрибусиреспонсе](freebusyresponse.md)
    
- [респонсемессаже](responsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [фрибусивиев](freebusyview.md)
    
- [фрибусивиевтипе](freebusyviewtype.md)
    
- [мержедфрибуси](mergedfreebusy.md)
    
- [календаревентаррай](calendareventarray.md)
    
- [календаревент](calendarevent.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [буситипе](busytype.md)
    
- [календаревентдетаилс](calendareventdetails.md)
    
- [ИД](id.md)
    
- [Subject (Календаревентдетаилс)](subject-calendareventdetails.md)
    
- [Местоположение (Календаревентдетаилс)](location-calendareventdetails.md)
    
- [Проведенное собрание (Календаревентдетаилс)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (Календаревентдетаилс)](isrecurring-calendareventdetails.md)
    
- [Исключение](isexception.md)
    
- [Попамятка](isreminderset.md)
    
- [Частный](isprivate.md)
    
- [воркингхаурс](workinghours-ex15websvcsotherref.md)
    
- [Часовой пояс (доступность)](timezone-availability.md)
    
- [Сдвиг (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [дайордер](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (TimeZone)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [воркингпериодаррай](workingperiodarray.md)
    
- [воркингпериод](workingperiod.md)
    
- [DayOfWeek (Воркингпериод)](dayofweek-workingperiod.md)
    
- [старттимеинминутес](starttimeinminutes.md)
    
- [ендтимеинминутес](endtimeinminutes.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

