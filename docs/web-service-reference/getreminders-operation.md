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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762901"
---
# <a name="getreminders-operation"></a>Операция GetReminders

Найдите сведения о **GetReminders** операции веб-служб Exchange. 
  
Операции веб-служб Exchange (EWS) **GetReminders** извлекает напоминания для элементов календаря и задачи. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>С помощью операции GetReminders

Операция **GetReminders** получает напоминаний для текущие и будущие календаря и задачи в почтовом ящике пользователя, в зависимости от значения элемента, передается в запросе. Операции можно извлечь все элементы текущие и будущие календаря, а также задачи, которые оповещение. Элементы календаря закрытый включены в ответы. Без напоминания не включены в ответы, ни с напоминаний по электронной почте или задач исполнению флаги. 
  
Для получения всех текущего напоминаний, рекомендуется установить [ReminderType](remindertype.md) для **всех** и [время окончания](endtime-remindermessagedatatype.md) для текущего времени. 
  
Если элементы [BeginTime](begintime.md) и **время окончания** включены в запрос, ответ содержит напоминаний для любого календаря и элементы задачи, которые происходят между напоминание, что происходит между **BeginTime** и **EndTime**.
  
В следующей таблице описываются поведение элемента **ReminderType** , когда элементы **BeginTime** и **EndTime** включены. 
  
|ReminderType ** элемент значение **|**Описание**|
|:-----|:-----|
|Все  <br/> |Напоминания, которые происходят между **BeginTime** и **EndTime**.  <br/> |
|Текущая платформа  <br/> |Напоминания, возвращаемые **все**, плюс напоминания ранее запрошенные временной интервал, если событие по-прежнему текущего, а также все встречи вне зависимости от срока хранения.  <br/> |
|Старый  <br/> |Напоминания, возвращаемые **все**, за вычетом события, которые еще не завершена, минус все встречи. Элементы **BeginTime** и **EndTime** должен иметь значение использовать **старое** значение.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Заголовки SOAP GetReminders операции

Операция **GetReminders** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Этот заголовок можно применять к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Пример запроса GetReminders операции

Приведенный ниже запрос операции **GetReminders** показано, как получить первые пять календаря элементов, которые происходят между **BeginTime** и **EndTime**.
  
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

Пример запроса SOAP body содержит следующие элементы:
  
- [GetReminders](getreminders.md)
    
- [Время окончания](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
SOAP body также может содержать следующие элементы:
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Успешные операции ответа GetReminders

В следующем примере показано успешного ответа на запрос операции **GetReminders** . Ответ содержит напоминания для элемента «Командное собрания» календарь и напоминания для задачи «Задачи для отправки заметок». 
  
> [!NOTE]
> Идентификаторы URL-были сокращены, чтобы сохранить удобочитаемость. 
  
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

Ответ SOAP body содержит следующие элементы:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Напоминания](reminders.md)
    
- [Памятки](reminder.md)
    
- [Subject](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [Дата начала](startdate.md)
    
- [Дата окончания](enddate-remindertype.md)
    
- [Идентификатор элемента](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [ИД ПОЛЬЗОВАТЕЛЯ](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Пример ответа об ошибке GetReminders операции

В следующем примере показано ошибочный ответ на запрос операции **GetReminders** . Это ответ на запрос, в котором дата окончания раньше, чем дата начала. 
  
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

Ошибка ответ SOAP body содержит следующие элементы:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также


- [PerformReminderAction](performreminderaction.md)
    

