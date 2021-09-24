---
title: Операция GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Сведения об операции GetReminders EWS.
ms.openlocfilehash: e47dbb6ffceac3535bb72f93ee27bbb3f3f259e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513565"
---
# <a name="getreminders-operation"></a>Операция GetReminders

Сведения об операции **GetReminders** EWS. 
  
Операция **GetReminders** Exchange веб-служб (EWS) извлекает напоминания для элементов календаря и задач. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Использование операции GetReminders

Операция **GetReminders** получает напоминания для текущих и будущих элементов календаря и задач в почтовом ящике пользователя в зависимости от значений элементов, переданных в запросе. Операция может получить все текущие и будущие элементы календаря, а также задачи с набором напоминаний. Частные элементы календаря включены в ответы. Задачи без напоминаний не включаются в ответы, а также сообщения электронной почты с напоминаниями или последующими флагами. 
  
Чтобы получить все текущие напоминания, рекомендуется  установить [для ReminderType](remindertype.md) все и [endTime](endtime-remindermessagedatatype.md) текущее время. 
  
Если [элементы BeginTime](begintime.md) и **EndTime** включены в запрос, ответ включает напоминания для любых элементов календаря и задач, которые возникают между ними, имеют напоминание о том, что происходит между **BeginTime** и **EndTime**.
  
В следующей таблице описывается поведение элемента **ReminderType** при включении элементов **BeginTime** и **EndTime.** 
  
|Значение элемента ReminderType** **|**Описание**|
|:-----|:-----|
|Все  <br/> |Напоминания, которые возникают между **BeginTime** и **EndTime**.  <br/> |
|Current  <br/> |Напоминания, возвращающиеся всеми, а также напоминания, которые являются более ранними, чем запрашиваемое окно времени, если событие продолжается, а также все встречи независимо от возраста.   <br/> |
|Старый  <br/> |Напоминания, возвращенные **all**, минус события, которые еще не завершены, за вычетом всех встреч. Элементы **BeginTime** и **EndTime** должны быть настроены для использования **старого** значения.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Заготчики операции GetReminders

В **операции GetReminders** можно использовать заглавные таблицы SOAP, указанные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Пример запроса на операцию GetReminders

В следующем примере запроса на операцию **GetReminders** показано, как получить первые пять элементов календаря, которые происходят между **BeginTime** и **EndTime.**
  
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

В примере тела запроса SOAP содержатся следующие элементы:
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
Тело SOAP также может содержать следующие элементы:
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Успешный ответ на операцию GetReminders

В следующем примере показан успешный ответ на запрос на операцию **GetReminders.** Ответ содержит напоминание для элемента календаря "Собрание команды" и напоминание для задачи "Задача отправить заметки о собрании". 
  
> [!NOTE]
> Для сохранения читаемости были сокращены идентификаторы. 
  
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

Тело SOAP ответа содержит следующие элементы:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Reminders](reminders.md)
    
- [Reminder](reminder.md)
    
- [Тема](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Пример ответа на ошибку операции GetReminders

В следующем примере показан ответ на ошибку запроса на операцию **GetReminders.** Это ответ на запрос, в котором дата окончания была раньше даты начала. 
  
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

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные коды ошибок, общие для EWS и специфические для этой операции, см. [в ответе.](responsecode.md)
  
## <a name="see-also"></a>См. также


- [PerformReminderAction](performreminderaction.md)
    

