---
title: Операция GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Найдите сведения о веб-служб Exchange GetReminders операции.
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762901"
---
# <a name="getreminders-operation"></a><span data-ttu-id="b265a-103">Операция GetReminders</span><span class="sxs-lookup"><span data-stu-id="b265a-103">GetReminders operation</span></span>

<span data-ttu-id="b265a-104">Найдите сведения о **GetReminders** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b265a-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="b265a-105">Операции веб-служб Exchange (EWS) **GetReminders** извлекает напоминания для элементов календаря и задачи.</span><span class="sxs-lookup"><span data-stu-id="b265a-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="b265a-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b265a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="b265a-107">С помощью операции GetReminders</span><span class="sxs-lookup"><span data-stu-id="b265a-107">Using the GetReminders operation</span></span>

<span data-ttu-id="b265a-108">Операция **GetReminders** получает напоминаний для текущие и будущие календаря и задачи в почтовом ящике пользователя, в зависимости от значения элемента, передается в запросе.</span><span class="sxs-lookup"><span data-stu-id="b265a-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="b265a-109">Операции можно извлечь все элементы текущие и будущие календаря, а также задачи, которые оповещение.</span><span class="sxs-lookup"><span data-stu-id="b265a-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="b265a-110">Элементы календаря закрытый включены в ответы.</span><span class="sxs-lookup"><span data-stu-id="b265a-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="b265a-111">Без напоминания не включены в ответы, ни с напоминаний по электронной почте или задач исполнению флаги.</span><span class="sxs-lookup"><span data-stu-id="b265a-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="b265a-112">Для получения всех текущего напоминаний, рекомендуется установить [ReminderType](remindertype.md) для **всех** и [время окончания](endtime-remindermessagedatatype.md) для текущего времени.</span><span class="sxs-lookup"><span data-stu-id="b265a-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="b265a-113">Если элементы [BeginTime](begintime.md) и **время окончания** включены в запрос, ответ содержит напоминаний для любого календаря и элементы задачи, которые происходят между напоминание, что происходит между **BeginTime** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b265a-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="b265a-114">В следующей таблице описываются поведение элемента **ReminderType** , когда элементы **BeginTime** и **EndTime** включены.</span><span class="sxs-lookup"><span data-stu-id="b265a-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="b265a-115">ReminderType ** элемент значение **</span><span class="sxs-lookup"><span data-stu-id="b265a-115">****ReminderType** element value**</span></span>|<span data-ttu-id="b265a-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b265a-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b265a-117">Все</span><span class="sxs-lookup"><span data-stu-id="b265a-117">All</span></span>  <br/> |<span data-ttu-id="b265a-118">Напоминания, которые происходят между **BeginTime** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b265a-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="b265a-119">Текущая платформа</span><span class="sxs-lookup"><span data-stu-id="b265a-119">Current</span></span>  <br/> |<span data-ttu-id="b265a-120">Напоминания, возвращаемые **все**, плюс напоминания ранее запрошенные временной интервал, если событие по-прежнему текущего, а также все встречи вне зависимости от срока хранения.</span><span class="sxs-lookup"><span data-stu-id="b265a-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="b265a-121">Старый</span><span class="sxs-lookup"><span data-stu-id="b265a-121">Old</span></span>  <br/> |<span data-ttu-id="b265a-122">Напоминания, возвращаемые **все**, за вычетом события, которые еще не завершена, минус все встречи.</span><span class="sxs-lookup"><span data-stu-id="b265a-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="b265a-123">Элементы **BeginTime** и **EndTime** должен иметь значение использовать **старое** значение.</span><span class="sxs-lookup"><span data-stu-id="b265a-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="b265a-124">Заголовки SOAP GetReminders операции</span><span class="sxs-lookup"><span data-stu-id="b265a-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="b265a-125">Операция **GetReminders** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b265a-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b265a-126">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="b265a-126">**Header name**</span></span>|<span data-ttu-id="b265a-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b265a-127">**Element**</span></span>|<span data-ttu-id="b265a-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b265a-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b265a-129">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="b265a-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b265a-130">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="b265a-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b265a-131">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="b265a-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b265a-132">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b265a-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b265a-133">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="b265a-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b265a-134">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="b265a-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b265a-135">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b265a-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b265a-136">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b265a-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b265a-137">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b265a-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b265a-138">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b265a-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b265a-139">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="b265a-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b265a-140">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b265a-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b265a-141">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b265a-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b265a-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b265a-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b265a-143">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="b265a-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b265a-144">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="b265a-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="b265a-145">Пример запроса GetReminders операции</span><span class="sxs-lookup"><span data-stu-id="b265a-145">GetReminders operation request example</span></span>

<span data-ttu-id="b265a-146">Приведенный ниже запрос операции **GetReminders** показано, как получить первые пять календаря элементов, которые происходят между **BeginTime** и **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="b265a-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="b265a-147">Пример запроса SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b265a-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b265a-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="b265a-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="b265a-149">Время окончания</span><span class="sxs-lookup"><span data-stu-id="b265a-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="b265a-150">ReminderType</span><span class="sxs-lookup"><span data-stu-id="b265a-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="b265a-151">SOAP body также может содержать следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b265a-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="b265a-152">BeginTime</span><span class="sxs-lookup"><span data-stu-id="b265a-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="b265a-153">MaxItems</span><span class="sxs-lookup"><span data-stu-id="b265a-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="b265a-154">Успешные операции ответа GetReminders</span><span class="sxs-lookup"><span data-stu-id="b265a-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="b265a-155">В следующем примере показано успешного ответа на запрос операции **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="b265a-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="b265a-156">Ответ содержит напоминания для элемента «Командное собрания» календарь и напоминания для задачи «Задачи для отправки заметок».</span><span class="sxs-lookup"><span data-stu-id="b265a-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b265a-157">Идентификаторы URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b265a-157">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b265a-158">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b265a-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b265a-159">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="b265a-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="b265a-160">Напоминания</span><span class="sxs-lookup"><span data-stu-id="b265a-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="b265a-161">Памятки</span><span class="sxs-lookup"><span data-stu-id="b265a-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="b265a-162">Subject</span><span class="sxs-lookup"><span data-stu-id="b265a-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="b265a-163">Location</span><span class="sxs-lookup"><span data-stu-id="b265a-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="b265a-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="b265a-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="b265a-165">Дата начала</span><span class="sxs-lookup"><span data-stu-id="b265a-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="b265a-166">Дата окончания</span><span class="sxs-lookup"><span data-stu-id="b265a-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="b265a-167">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b265a-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b265a-168">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="b265a-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="b265a-169">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="b265a-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="b265a-170">ИД ПОЛЬЗОВАТЕЛЯ</span><span class="sxs-lookup"><span data-stu-id="b265a-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="b265a-171">Пример ответа об ошибке GetReminders операции</span><span class="sxs-lookup"><span data-stu-id="b265a-171">GetReminders operation error response example</span></span>

<span data-ttu-id="b265a-172">В следующем примере показано ошибочный ответ на запрос операции **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="b265a-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="b265a-173">Это ответ на запрос, в котором дата окончания раньше, чем дата начала.</span><span class="sxs-lookup"><span data-stu-id="b265a-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b265a-174">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b265a-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b265a-175">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="b265a-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="b265a-176">MessageText</span><span class="sxs-lookup"><span data-stu-id="b265a-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b265a-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b265a-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b265a-178">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b265a-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b265a-179">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b265a-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b265a-180">См. также</span><span class="sxs-lookup"><span data-stu-id="b265a-180">See also</span></span>


- [<span data-ttu-id="b265a-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b265a-181">PerformReminderAction</span></span>](performreminderaction.md)
    

