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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458224"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="88621-103">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="88621-103">GetUserAvailability operation</span></span>

<span data-ttu-id="88621-104">Поиск сведений о **GetUserAvailabilityной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="88621-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="88621-105">Операция **GetUserAvailability** предоставляет подробные сведения о доступности набора пользователей, помещений и ресурсов в течение заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="88621-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="88621-106">Использование операции GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="88621-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="88621-107">Операция **GetUserAvailability** предоставляет сведения о доступности текущих пользователей на указанном уровне детализации.</span><span class="sxs-lookup"><span data-stu-id="88621-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="88621-108">Клиентские приложения, такие как Outlook, Outlook Web Access, Outlook Mobile Access и другие, используют адреса SMTP для идентификации запрашиваемых сведений о пользователях.</span><span class="sxs-lookup"><span data-stu-id="88621-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="88621-109">Служба доступности расширяет списки рассылки для получения сведений о доступности для каждого участника списка, если количество почтовых ящиков в списке рассылки меньше 100, что является максимальным количеством идентификаторов, которые может запросить операция **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="88621-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="88621-110">Сведения о доступности участников списка рассылки объединяются в один статус занятости для всего списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="88621-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="88621-111">В запросах клиентского приложения указывается период времени, в течение которого запрос доступности.</span><span class="sxs-lookup"><span data-stu-id="88621-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="88621-112">По умолчанию для запрашиваемых сведений используется период времени 42 дней.</span><span class="sxs-lookup"><span data-stu-id="88621-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="88621-113">Если календарь пользователя содержит встречи или собрания, которые находятся в определенном периоде времени и не выходят за него, возвращается встреча.</span><span class="sxs-lookup"><span data-stu-id="88621-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="88621-114">Возвращаемые время встреч и собраний находятся в том же часовом поясе, что и клиентское приложение, запрашивающее собрание.</span><span class="sxs-lookup"><span data-stu-id="88621-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="88621-115">Служба доступности обрабатывает запрос для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="88621-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="88621-116">Служба развертывает все повторяющиеся встречи и возвращает максимальное количество сведений о календаре, которое у запрашивающего клиента имеет разрешение на получение.</span><span class="sxs-lookup"><span data-stu-id="88621-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="88621-117">Если целевой почтовый ящик недоступен или не может быть найден, создается исключение **маилреЦипиентнотфаундексцептион** .</span><span class="sxs-lookup"><span data-stu-id="88621-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="88621-118">Клиент получает сообщение об ошибке, в котором говорится, что получатель не найден в службе каталогов Active Directory или в доменных службах Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="88621-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="88621-119">Заголовки SOAP операции GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="88621-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="88621-120">Операция **GetUserAvailability** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="88621-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="88621-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="88621-121">**Header**</span></span>|<span data-ttu-id="88621-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88621-122">**Element**</span></span>|<span data-ttu-id="88621-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88621-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="88621-124">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="88621-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="88621-125">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="88621-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="88621-126">Определяет пользователя, который олицетворяет клиент.</span><span class="sxs-lookup"><span data-stu-id="88621-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="88621-127">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="88621-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="88621-128">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="88621-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="88621-129">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="88621-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="88621-130">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="88621-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="88621-131">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="88621-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="88621-132">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="88621-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="88621-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="88621-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="88621-134">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="88621-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="88621-135">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="88621-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="88621-136">**тимезонеконтекст**</span><span class="sxs-lookup"><span data-stu-id="88621-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="88621-137">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="88621-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="88621-138">Указывает заголовок SOAP, определяющий часовой пояс, который будет использоваться для всех ответов сервера.</span><span class="sxs-lookup"><span data-stu-id="88621-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="88621-139">Все значения времени, возвращаемые с сервера, будут преобразованы в указанный часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="88621-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="88621-140">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="88621-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="88621-141">Пример запроса GetUserAvailability: получение сведений о доступности</span><span class="sxs-lookup"><span data-stu-id="88621-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="88621-142">В приведенном ниже примере запроса операции **GetUserAvailability** показано, как получить подробные сведения о доступности для двух пользователей в часовом поясе по тихоокеанскому времени.</span><span class="sxs-lookup"><span data-stu-id="88621-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
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

<span data-ttu-id="88621-143">Дополнительные сведения о получении предложенных собраний с помощью элемента [сугжестионсвиевоптионс](suggestionsviewoptions.md) можно найти в схеме в виртуальном каталоге EWS.</span><span class="sxs-lookup"><span data-stu-id="88621-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="88621-144">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="88621-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="88621-145">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="88621-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="88621-146">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="88621-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="88621-147">Сдвиг (UTC)</span><span class="sxs-lookup"><span data-stu-id="88621-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="88621-148">StandardTime</span><span class="sxs-lookup"><span data-stu-id="88621-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="88621-149">Bias</span><span class="sxs-lookup"><span data-stu-id="88621-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="88621-150">Time</span><span class="sxs-lookup"><span data-stu-id="88621-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="88621-151">дайордер</span><span class="sxs-lookup"><span data-stu-id="88621-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="88621-152">Month</span><span class="sxs-lookup"><span data-stu-id="88621-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="88621-153">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="88621-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="88621-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="88621-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="88621-155">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="88621-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="88621-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="88621-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="88621-157">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="88621-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="88621-158">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="88621-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="88621-159">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="88621-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="88621-160">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="88621-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="88621-161">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="88621-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="88621-162">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="88621-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="88621-163">StartTime</span><span class="sxs-lookup"><span data-stu-id="88621-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="88621-164">EndTime</span><span class="sxs-lookup"><span data-stu-id="88621-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="88621-165">Успешный отклик операции GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="88621-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="88621-166">В следующем примере показан успешный ответ на запрос операции **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="88621-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="88621-167">Идентификаторы событий календаря были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88621-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="88621-168">Сведения о доступности для каждого пользователя отображаются в уникальном элементе [фрибусиреспонсе](freebusyresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="88621-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="88621-169">Порядок пользователей в запросе операции **GetUserAvailability** определяет порядок данных о доступности для каждого пользователя в отклике.</span><span class="sxs-lookup"><span data-stu-id="88621-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="88621-170">В клиенте возвращается сообщение об ошибке, если количество встреч в периоде времени, определенном в запросе, превышает максимальное число, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="88621-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="88621-171">По умолчанию максимальное число встреч составляет 10 000 одиночных экземпляров и расширенных элементов повторения.</span><span class="sxs-lookup"><span data-stu-id="88621-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="88621-172">Это свойство можно настроить только администратором.</span><span class="sxs-lookup"><span data-stu-id="88621-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="88621-173">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="88621-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="88621-174">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="88621-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="88621-175">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="88621-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="88621-176">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="88621-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="88621-177">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="88621-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="88621-178">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="88621-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="88621-179">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="88621-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="88621-180">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="88621-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="88621-181">фрибусивиевтипе</span><span class="sxs-lookup"><span data-stu-id="88621-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="88621-182">мержедфрибуси</span><span class="sxs-lookup"><span data-stu-id="88621-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="88621-183">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="88621-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="88621-184">календаревент</span><span class="sxs-lookup"><span data-stu-id="88621-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="88621-185">StartTime</span><span class="sxs-lookup"><span data-stu-id="88621-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="88621-186">EndTime</span><span class="sxs-lookup"><span data-stu-id="88621-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="88621-187">буситипе</span><span class="sxs-lookup"><span data-stu-id="88621-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="88621-188">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="88621-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="88621-189">ИД</span><span class="sxs-lookup"><span data-stu-id="88621-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="88621-190">Subject (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="88621-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="88621-191">Местоположение (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="88621-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="88621-192">Проведенное собрание (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="88621-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="88621-193">IsRecurring (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="88621-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="88621-194">Исключение</span><span class="sxs-lookup"><span data-stu-id="88621-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="88621-195">Попамятка</span><span class="sxs-lookup"><span data-stu-id="88621-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="88621-196">Частный</span><span class="sxs-lookup"><span data-stu-id="88621-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="88621-197">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="88621-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="88621-198">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="88621-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="88621-199">Сдвиг (UTC)</span><span class="sxs-lookup"><span data-stu-id="88621-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="88621-200">StandardTime</span><span class="sxs-lookup"><span data-stu-id="88621-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="88621-201">Bias</span><span class="sxs-lookup"><span data-stu-id="88621-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="88621-202">Time</span><span class="sxs-lookup"><span data-stu-id="88621-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="88621-203">дайордер</span><span class="sxs-lookup"><span data-stu-id="88621-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="88621-204">Month</span><span class="sxs-lookup"><span data-stu-id="88621-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="88621-205">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="88621-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="88621-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="88621-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="88621-207">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="88621-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="88621-208">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="88621-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="88621-209">DayOfWeek (Воркингпериод)</span><span class="sxs-lookup"><span data-stu-id="88621-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="88621-210">старттимеинминутес</span><span class="sxs-lookup"><span data-stu-id="88621-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="88621-211">ендтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="88621-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="88621-212">См. также</span><span class="sxs-lookup"><span data-stu-id="88621-212">See also</span></span>

- [<span data-ttu-id="88621-213">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="88621-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="88621-214">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="88621-214">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

