---
title: Операция GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Найдите сведения об операции с помощью службы EWS.
ms.openlocfilehash: dcbe20c674d7524a7776d374fa6964899abf472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458308"
---
# <a name="getreminders-operation"></a><span data-ttu-id="b98cf-103">Операция GetReminders</span><span class="sxs-lookup"><span data-stu-id="b98cf-103">GetReminders operation</span></span>

<span data-ttu-id="b98cf-104">Найдите сведения об операции **с помощью** службы EWS.</span><span class="sxs-lookup"><span data-stu-id="b98cf-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="b98cf-105">Операция веб- **служб Exchange (** EWS) получает напоминания для элементов календаря и задач.</span><span class="sxs-lookup"><span data-stu-id="b98cf-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="b98cf-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b98cf-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="b98cf-107">Использование операции "распоминать"</span><span class="sxs-lookup"><span data-stu-id="b98cf-107">Using the GetReminders operation</span></span>

<span data-ttu-id="b98cf-108">Операция **по** распамятке получает напоминания о текущем и будущем календаре и элементах задач в почтовом ящике пользователя в зависимости от значений элементов, переданных в запросе.</span><span class="sxs-lookup"><span data-stu-id="b98cf-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="b98cf-109">Эта операция может получать все текущие и будущие элементы календаря, а также задачи, для которых задано напоминание.</span><span class="sxs-lookup"><span data-stu-id="b98cf-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="b98cf-110">В ответы включаются элементы закрытого календаря.</span><span class="sxs-lookup"><span data-stu-id="b98cf-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="b98cf-111">Задачи без напоминаний не включаются в отклики, а также не используются электронные письма с отметками и напоминаниями.</span><span class="sxs-lookup"><span data-stu-id="b98cf-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="b98cf-112">Чтобы получить все текущие напоминания, рекомендуется установить для параметра [реминдертипе](remindertype.md) значение **ALL** , а для свойства [EndTime](endtime-remindermessagedatatype.md) — текущее время.</span><span class="sxs-lookup"><span data-stu-id="b98cf-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="b98cf-113">Если в запрос включены элементы [бегинтиме](begintime.md) и **EndTime** , ответ включает в себя напоминания для всех элементов календаря и задач, которые происходят между **бегинтиме** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b98cf-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="b98cf-114">В следующей таблице описывается поведение элемента **реминдертипе** при включении элементов **бегинтиме** и **EndTime** .</span><span class="sxs-lookup"><span data-stu-id="b98cf-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="b98cf-115">Значение элемента Реминдертипе \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="b98cf-115">\*\*\*\*ReminderType\*\* element value\*\*</span></span>|<span data-ttu-id="b98cf-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b98cf-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b98cf-117">Все</span><span class="sxs-lookup"><span data-stu-id="b98cf-117">All</span></span>  <br/> |<span data-ttu-id="b98cf-118">Напоминания, происходящие между **бегинтиме** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b98cf-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="b98cf-119">Current</span><span class="sxs-lookup"><span data-stu-id="b98cf-119">Current</span></span>  <br/> |<span data-ttu-id="b98cf-120">Напоминания, возвращенные **всеми**, а также напоминания, предшествующие запрошенному окну времени, если событие продолжает выполняться, а также все встречи, независимо от возраста.</span><span class="sxs-lookup"><span data-stu-id="b98cf-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="b98cf-121">Ранее</span><span class="sxs-lookup"><span data-stu-id="b98cf-121">Old</span></span>  <br/> |<span data-ttu-id="b98cf-122">Напоминания, возвращаемые **всеми**, за вычетом событий, которые еще не выполнены, за вычетом всех встреч.</span><span class="sxs-lookup"><span data-stu-id="b98cf-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="b98cf-123">Для элементов **бегинтиме** и **EndTime** необходимо задать **старое** значение.</span><span class="sxs-lookup"><span data-stu-id="b98cf-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="b98cf-124">Заголовков SOAP операции с раснапоминаниями</span><span class="sxs-lookup"><span data-stu-id="b98cf-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="b98cf-125">В операции " **Пронапомнить** " могут использоваться заголовки SOAP, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b98cf-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b98cf-126">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="b98cf-126">**Header name**</span></span>|<span data-ttu-id="b98cf-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b98cf-127">**Element**</span></span>|<span data-ttu-id="b98cf-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b98cf-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b98cf-129">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="b98cf-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b98cf-130">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="b98cf-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b98cf-131">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="b98cf-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b98cf-132">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b98cf-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b98cf-133">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="b98cf-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b98cf-134">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b98cf-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b98cf-135">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b98cf-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b98cf-136">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b98cf-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b98cf-137">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="b98cf-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b98cf-138">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b98cf-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b98cf-139">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b98cf-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b98cf-140">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b98cf-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b98cf-141">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="b98cf-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b98cf-142">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b98cf-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b98cf-143">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b98cf-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b98cf-144">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="b98cf-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="b98cf-145">Пример запроса операции с раснапоминаниями</span><span class="sxs-lookup"><span data-stu-id="b98cf-145">GetReminders operation request example</span></span>

<span data-ttu-id="b98cf-146">В приведенном ниже примере запроса операции " **Пронапомниться** " показано, как получить первые пять элементов календаря, которые происходят между **бегинтиме** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b98cf-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b98cf-147">В примере сообщения SOAP Request содержатся следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b98cf-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b98cf-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="b98cf-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="b98cf-149">EndTime</span><span class="sxs-lookup"><span data-stu-id="b98cf-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="b98cf-150">реминдертипе</span><span class="sxs-lookup"><span data-stu-id="b98cf-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="b98cf-151">В теле SOAP также могут содержаться следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b98cf-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="b98cf-152">бегинтиме</span><span class="sxs-lookup"><span data-stu-id="b98cf-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="b98cf-153">макситемс</span><span class="sxs-lookup"><span data-stu-id="b98cf-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="b98cf-154">Успешный ответ на операцию</span><span class="sxs-lookup"><span data-stu-id="b98cf-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="b98cf-155">В приведенном ниже примере показан успешный ответ **на запрос по операции GetResponse** .</span><span class="sxs-lookup"><span data-stu-id="b98cf-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="b98cf-156">Ответ содержит напоминание о задаче "собрание группы" и напоминание о задаче "задача по отправке заметок о собраниях".</span><span class="sxs-lookup"><span data-stu-id="b98cf-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b98cf-157">Идентификаторы сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b98cf-157">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b98cf-158">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b98cf-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b98cf-159">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="b98cf-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="b98cf-160">Reminders</span><span class="sxs-lookup"><span data-stu-id="b98cf-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="b98cf-161">Reminder</span><span class="sxs-lookup"><span data-stu-id="b98cf-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="b98cf-162">Тема</span><span class="sxs-lookup"><span data-stu-id="b98cf-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="b98cf-163">Location</span><span class="sxs-lookup"><span data-stu-id="b98cf-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="b98cf-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="b98cf-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="b98cf-165">StartDate</span><span class="sxs-lookup"><span data-stu-id="b98cf-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="b98cf-166">EndDate</span><span class="sxs-lookup"><span data-stu-id="b98cf-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="b98cf-167">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b98cf-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b98cf-168">рекуррингмастеритемид</span><span class="sxs-lookup"><span data-stu-id="b98cf-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="b98cf-169">реминдерграуп</span><span class="sxs-lookup"><span data-stu-id="b98cf-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="b98cf-170">UID</span><span class="sxs-lookup"><span data-stu-id="b98cf-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="b98cf-171">Пример ответа на сообщение об ошибке при выполнении операции с раснапоминаниями</span><span class="sxs-lookup"><span data-stu-id="b98cf-171">GetReminders operation error response example</span></span>

<span data-ttu-id="b98cf-172">В приведенном ниже примере показан ответ об ошибке для запроса на операцию " **Пронапомнить** ".</span><span class="sxs-lookup"><span data-stu-id="b98cf-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="b98cf-173">Это ответ на запрос, в котором Дата окончания предшествует дате начала.</span><span class="sxs-lookup"><span data-stu-id="b98cf-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b98cf-174">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b98cf-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b98cf-175">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="b98cf-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="b98cf-176">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b98cf-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b98cf-177">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b98cf-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b98cf-178">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b98cf-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b98cf-179">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b98cf-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b98cf-180">См. также</span><span class="sxs-lookup"><span data-stu-id="b98cf-180">See also</span></span>


- [<span data-ttu-id="b98cf-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b98cf-181">PerformReminderAction</span></span>](performreminderaction.md)
    

