---
title: Операция PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Сведения об операции PerformReminderAction EWS.
ms.openlocfilehash: ca547c401100afdfd9d846ca3bfddf710efd2797
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515308"
---
# <a name="performreminderaction-operation"></a>Операция PerformReminderAction

Сведения об операции **PerformReminderAction** EWS. 
  
Операция **PerformReminderAction** Exchange Веб-службы (EWS) инициирует действие увольнения или snooze на напоминание. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Использование операции PerformReminderAction

С помощью **операции PerformReminderAction** можно отклонять или отклонять (задерживать) напоминания, возвращаемые операцией [GetReminders.](getreminders-operation.md) Чтобы отобразить напоминание, установите Значение [ActionType](actiontype-reminderactiontype.md) для **Snooze** и установите значение [NewReminderTime](newremindertime.md) на время позже текущего [ReminderTime,](remindertime.md)в противном случае **Сервер NewReminderTime** игнорируется сервером. Если напоминание является событием повторяющегося собрания, и действие **Snooze** будет приниматься на напоминание с **помощью NewReminderTime,** которое прошло напоминание о следующем возникновении, это напоминание фактически отклоняться. 
  
Чтобы отклонять напоминание, установите **ActionType** для **увольнения.** При обработке запроса сервер изменяет значение [IsReminderSet](isreminderset.md) для элемента **True** на **false.**
  
### <a name="performreminderaction-operation-soap-headers"></a>PerformReminderAction operation SOAP headers

Операция **PerformReminderAction** может использовать заглавные таблицы SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Пример запроса операции PerformReminderAction

В следующем примере запроса на операцию **PerformReminderAction** показано, как отладить текущее напоминание и установить новое время напоминания. Обратите внимание, что необходимо включить **ChangeKey** для [ItemId](itemid.md) и **NewReminderTime,** которые должны быть заданы на время позже, чем время **reminderTime,** возвращенное операцией [GetReminders.](getreminders-operation.md) 
  
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
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> Значение **ItemId** было сокращено для сохранения читаемости. 
  
Тело SOAP запроса содержит следующие элементы:
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Успешный ответ операции PerformReminderAction

В следующем примере показан успешный ответ на запрос **операции PerformReminderAction.** Элемент **UpdatedItemIds содержит** **ItemIds** обновленного элемента календаря. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Тело SOAP ответа содержит следующие элементы:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ItemId](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Пример ответа на ошибку операции PerformReminderAction

В следующем примере показан ответ на запрос **операции PerformReminderAction,** когда на сервере не было сделано никаких изменений. Это ответ, в котором был отправлен запрос, но не было возвращено **updatedItemIds,** что означает, что никакие напоминания не были изменены. 
  
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
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Дополнительные коды ошибок, которые являются общими для EWS, см. [в рубрике ResponseCode.](responsecode.md)
  
## <a name="see-also"></a>См. также


- [Операция GetReminders](getreminders-operation.md)
    

