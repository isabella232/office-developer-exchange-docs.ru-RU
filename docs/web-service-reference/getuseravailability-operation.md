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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833686"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="4615c-103">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4615c-103">GetUserAvailability operation</span></span>

<span data-ttu-id="4615c-104">Найдите сведения о операция **GetUserAvailability** веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4615c-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="4615c-105">Операция **GetUserAvailability** приведены подробные сведения о доступности из набора пользователей, помещений и ресурсов внутри заданного периода времени.</span><span class="sxs-lookup"><span data-stu-id="4615c-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="4615c-106">С помощью операции GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4615c-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="4615c-107">Операция **GetUserAvailability** предоставляет сведения о доступности текущего пользователя на указанном уровне детализации.</span><span class="sxs-lookup"><span data-stu-id="4615c-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="4615c-108">Клиентские приложения, такие как Outlook, Outlook Web Access, Outlook Mobile Access и другим пользователям использовать SMTP-адреса для идентификации сведения запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4615c-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="4615c-109">Служба доступности расширяет списки рассылки, чтобы получить состояние сведений о доступности для каждого элемента списка, до тех пор, пока число почтовых ящиков в список рассылки — это меньше, чем 100, максимальное число идентификаторов, **GetUserAvailability **операции можно запросить.</span><span class="sxs-lookup"><span data-stu-id="4615c-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="4615c-110">Состояния занятости членов списка рассылки будут объединены одного состояния занятости для списка рассылки целиком.</span><span class="sxs-lookup"><span data-stu-id="4615c-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="4615c-111">Запросы клиентов приложения укажите период времени доступности запрос.</span><span class="sxs-lookup"><span data-stu-id="4615c-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="4615c-112">Значение по умолчанию промежуток времени для запрошенные данные — 42 дня.</span><span class="sxs-lookup"><span data-stu-id="4615c-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="4615c-113">Если календарь пользователя содержит встречи или собрания, которые являются как внутри, так и за пределами за определенный период для запроса, возвращается встречи.</span><span class="sxs-lookup"><span data-stu-id="4615c-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="4615c-114">Время встречи и собрания, возвращенных находятся в другом часовом поясе по клиентское приложение, которое запрашивает собрания.</span><span class="sxs-lookup"><span data-stu-id="4615c-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="4615c-115">Служба доступности обрабатывает запрос для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="4615c-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="4615c-116">Служба расширяет повторяющихся встреч и возвращает максимальное количество сведений календаря, для которых есть разрешение на получение запрашивающего клиента.</span><span class="sxs-lookup"><span data-stu-id="4615c-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4615c-117">Если целевой почтовый ящик недоступен или не удается найти, **MailRecipientNotFoundException** исключение.</span><span class="sxs-lookup"><span data-stu-id="4615c-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="4615c-118">Клиент получает сообщение об ошибке о том, что получатель не найден в службе каталогов Active Directory или доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="4615c-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="4615c-119">Заголовки SOAP операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4615c-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="4615c-120">Операция **GetUserAvailability** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4615c-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="4615c-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="4615c-121">**Header**</span></span>|<span data-ttu-id="4615c-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4615c-122">**Element**</span></span>|<span data-ttu-id="4615c-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4615c-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4615c-124">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="4615c-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="4615c-125">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4615c-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4615c-126">Идентифицирует пользователя, которого олицетворения клиента.</span><span class="sxs-lookup"><span data-stu-id="4615c-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="4615c-127">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="4615c-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4615c-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="4615c-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="4615c-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4615c-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4615c-130">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="4615c-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="4615c-131">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="4615c-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4615c-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="4615c-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="4615c-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4615c-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4615c-134">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="4615c-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="4615c-135">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="4615c-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="4615c-136">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="4615c-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="4615c-137">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="4615c-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="4615c-138">Задает заголовок SOAP, который определяет часовой пояс, который будет использоваться для всех ответов с сервера.</span><span class="sxs-lookup"><span data-stu-id="4615c-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="4615c-139">Все значения времени, возвращаемые с сервера будут преобразованы в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="4615c-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="4615c-140">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="4615c-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="4615c-141">Пример запроса GetUserAvailability: получение данных о доступности</span><span class="sxs-lookup"><span data-stu-id="4615c-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="4615c-142">В следующем примере запрос операция **GetUserAvailability** показано, как получить сведения о доступности подробные для двух пользователей в часовом поясе по тихоокеанскому времени.</span><span class="sxs-lookup"><span data-stu-id="4615c-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
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

<span data-ttu-id="4615c-143">Дополнительные сведения о получении предложенного собрания с помощью элемента [SuggestionsViewOptions](suggestionsviewoptions.md) можно схемы в виртуальном каталоге веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4615c-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="4615c-144">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4615c-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4615c-145">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4615c-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="4615c-146">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="4615c-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="4615c-147">Смещение (UTC)</span><span class="sxs-lookup"><span data-stu-id="4615c-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="4615c-148">StandardTime</span><span class="sxs-lookup"><span data-stu-id="4615c-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="4615c-149">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="4615c-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="4615c-150">Time</span><span class="sxs-lookup"><span data-stu-id="4615c-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="4615c-151">DayOrder</span><span class="sxs-lookup"><span data-stu-id="4615c-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="4615c-152">Месяц</span><span class="sxs-lookup"><span data-stu-id="4615c-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="4615c-153">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="4615c-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="4615c-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="4615c-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="4615c-155">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="4615c-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="4615c-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="4615c-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="4615c-157">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4615c-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="4615c-158">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="4615c-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="4615c-159">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="4615c-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="4615c-160">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="4615c-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="4615c-161">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="4615c-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="4615c-162">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="4615c-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="4615c-163">Время начала</span><span class="sxs-lookup"><span data-stu-id="4615c-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="4615c-164">Время окончания</span><span class="sxs-lookup"><span data-stu-id="4615c-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="4615c-165">Успешного ответа операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4615c-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="4615c-166">В следующем примере показано успешного ответа на запрос операция **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="4615c-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4615c-167">Идентификаторы событий календаря URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="4615c-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="4615c-168">Сведения о доступности для каждого пользователя отображается в элементе уникальный [FreeBusyResponse](freebusyresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="4615c-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="4615c-169">Порядок пользователей в запросе операция **GetUserAvailability** определяет приоритет данных о доступности для каждого пользователя в ответе.</span><span class="sxs-lookup"><span data-stu-id="4615c-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="4615c-170">Ошибка будут возвращены клиенту, если число встреч в период времени, определенного в запросе превышает максимальное время, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="4615c-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="4615c-171">По умолчанию максимальное число встреч — 10 000 отдельные экземпляры и расширенное повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="4615c-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="4615c-172">Это свойство можно настроить только администратором.</span><span class="sxs-lookup"><span data-stu-id="4615c-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="4615c-173">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4615c-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4615c-174">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4615c-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4615c-175">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4615c-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="4615c-176">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="4615c-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="4615c-177">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="4615c-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="4615c-178">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4615c-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="4615c-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4615c-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4615c-180">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="4615c-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="4615c-181">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="4615c-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="4615c-182">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="4615c-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="4615c-183">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="4615c-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="4615c-184">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="4615c-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="4615c-185">Время начала</span><span class="sxs-lookup"><span data-stu-id="4615c-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="4615c-186">Время окончания</span><span class="sxs-lookup"><span data-stu-id="4615c-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="4615c-187">BusyType</span><span class="sxs-lookup"><span data-stu-id="4615c-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="4615c-188">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="4615c-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="4615c-189">ИД</span><span class="sxs-lookup"><span data-stu-id="4615c-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="4615c-190">Тема (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="4615c-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="4615c-191">Расположение (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="4615c-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="4615c-192">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="4615c-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="4615c-193">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="4615c-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="4615c-194">IsException</span><span class="sxs-lookup"><span data-stu-id="4615c-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="4615c-195">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="4615c-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="4615c-196">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="4615c-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="4615c-197">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="4615c-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="4615c-198">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="4615c-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="4615c-199">Смещение (UTC)</span><span class="sxs-lookup"><span data-stu-id="4615c-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="4615c-200">StandardTime</span><span class="sxs-lookup"><span data-stu-id="4615c-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="4615c-201">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="4615c-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="4615c-202">Time</span><span class="sxs-lookup"><span data-stu-id="4615c-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="4615c-203">DayOrder</span><span class="sxs-lookup"><span data-stu-id="4615c-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="4615c-204">Месяц</span><span class="sxs-lookup"><span data-stu-id="4615c-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="4615c-205">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="4615c-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="4615c-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="4615c-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="4615c-207">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="4615c-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="4615c-208">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="4615c-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="4615c-209">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="4615c-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="4615c-210">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="4615c-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="4615c-211">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="4615c-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="4615c-212">См. также</span><span class="sxs-lookup"><span data-stu-id="4615c-212">See also</span></span>

- [<span data-ttu-id="4615c-213">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4615c-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="4615c-214">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="4615c-214">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

