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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458308"
---
# <a name="getreminders-operation"></a>Операция GetReminders

Найдите сведения об операции **с помощью** службы EWS. 
  
Операция веб- **служб Exchange (** EWS) получает напоминания для элементов календаря и задач. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Использование операции "распоминать"

Операция **по** распамятке получает напоминания о текущем и будущем календаре и элементах задач в почтовом ящике пользователя в зависимости от значений элементов, переданных в запросе. Эта операция может получать все текущие и будущие элементы календаря, а также задачи, для которых задано напоминание. В ответы включаются элементы закрытого календаря. Задачи без напоминаний не включаются в отклики, а также не используются электронные письма с отметками и напоминаниями. 
  
Чтобы получить все текущие напоминания, рекомендуется установить для параметра [реминдертипе](remindertype.md) значение **ALL** , а для свойства [EndTime](endtime-remindermessagedatatype.md) — текущее время. 
  
Если в запрос включены элементы [бегинтиме](begintime.md) и **EndTime** , ответ включает в себя напоминания для всех элементов календаря и задач, которые происходят между **бегинтиме** и **EndTime**.
  
В следующей таблице описывается поведение элемента **реминдертипе** при включении элементов **бегинтиме** и **EndTime** . 
  
|Значение элемента Реминдертипе * * * *|**Описание**|
|:-----|:-----|
|Все  <br/> |Напоминания, происходящие между **бегинтиме** и **EndTime**.  <br/> |
|Current  <br/> |Напоминания, возвращенные **всеми**, а также напоминания, предшествующие запрошенному окну времени, если событие продолжает выполняться, а также все встречи, независимо от возраста.  <br/> |
|Ранее  <br/> |Напоминания, возвращаемые **всеми**, за вычетом событий, которые еще не выполнены, за вычетом всех встреч. Для элементов **бегинтиме** и **EndTime** необходимо задать **старое** значение.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Заголовков SOAP операции с раснапоминаниями

В операции " **Пронапомнить** " могут использоваться заголовки SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Пример запроса операции с раснапоминаниями

В приведенном ниже примере запроса операции " **Пронапомниться** " показано, как получить первые пять элементов календаря, которые происходят между **бегинтиме** и **EndTime**.
  
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

В примере сообщения SOAP Request содержатся следующие элементы:
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [реминдертипе](remindertype.md)
    
В теле SOAP также могут содержаться следующие элементы:
  
- [бегинтиме](begintime.md)
    
- [макситемс](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Успешный ответ на операцию

В приведенном ниже примере показан успешный ответ **на запрос по операции GetResponse** . Ответ содержит напоминание о задаче "собрание группы" и напоминание о задаче "задача по отправке заметок о собраниях". 
  
> [!NOTE]
> Идентификаторы сокращены для сохранения удобочитаемости. 
  
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

Тело SOAP отклика содержит следующие элементы:
  
- [жетреминдерсреспонсе](getremindersresponse.md)
    
- [Reminders](reminders.md)
    
- [Reminder](reminder.md)
    
- [Тема](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [Идентификатор](itemid.md)
    
- [рекуррингмастеритемид](recurringmasteritemid.md)
    
- [реминдерграуп](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Пример ответа на сообщение об ошибке при выполнении операции с раснапоминаниями

В приведенном ниже примере показан ответ об ошибке для запроса на операцию " **Пронапомнить** ". Это ответ на запрос, в котором Дата окончания предшествует дате начала. 
  
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

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жетреминдерсреспонсе](getremindersresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также


- [PerformReminderAction](performreminderaction.md)
    

