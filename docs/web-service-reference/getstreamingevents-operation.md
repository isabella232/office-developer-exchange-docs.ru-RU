---
title: Операция GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Найдите сведения о веб-служб Exchange GetStreamingEvents операции.
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833673"
---
# <a name="getstreamingevents-operation"></a>Операция GetStreamingEvents

Найдите сведения о **GetStreamingEvents** операции веб-служб Exchange. 
  
Операция **GetStreamingEvents** используется потоковая передача клиенты подписки для запроса уведомлений с сервера клиентского доступа. Ответ **GetStreamingEvents** возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления. 
  
## <a name="getstreamingevents-request-example"></a>Пример запроса GetStreamingEvents

### <a name="description"></a>Описание

В следующем примере операция **GetStreamingEvents** показано, как запросить событий и элементы, связанные с подпиской, который идентифицируется по идентификатору подписки. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a>Элементы запроса GetStreamingEvents

В запросе используются следующие элементы:
  
- [GetStreamingEvents](getstreamingevents.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
- [ConnectionTimeout](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a>Пример успешного ответа GetStreamingEvents

### <a name="description"></a>Описание

В следующем примере ответа **GetStreamingEvents** показано уведомлений, отправленных в клиенте при получении нового сообщения электронной почты. Включает уведомления для следующих событий: CreatedEvent, NewMail и ModifiedEvent. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a>Элементы ответов GetStreamingEvents

В ответе используются следующие элементы:
  
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md)
    
- [NotesFolderPermissionLevel](notesfolderpermissionlevel.md)
    
- [Уведомление](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
Чтобы найти другие параметры в сообщении ответа **GetStreamingEvents** операции, изучите иерархия схемы. Запустите на элементе [уведомлений](notification-ex15websvcsotherref.md) . 
  
## <a name="getstreamingevents-error-response-example"></a>Пример ответа об ошибке GetStreamingEvents

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос **GetStreamingEvents** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Замечания

При обработке запроса **GetStreamingEvents** , сервера клиентского доступа необходимо выполнить следующие действия: 
  
1. [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) запроса подтверждения действительную подписку, размещенного на сервере клиентского доступа. Если он не установлен, **GetStreamingEvents** завершается неудачно. 
    
2. SMTP-адрес пользователя, прошедшего проверку подлинности для запроса проверяется на наличие прав олицетворения. Если нет, не удается выполнить запрос **GetStreamingEvents** . 
    
3. Очередь подписки будет опрошен на наличие событий, ожидающих отправляются клиенту. Если очередь не является пустым, первые 50 события из очереди, которые извлекаются из очереди и кодируются в уведомление.
    
4. Если события не обнаружены в очереди, [StatusEvent](statusevent.md) создан и кодируются в ответ уведомлений. 
    
5. Уведомление ответ возвращается клиенту.
    
6. События, включенные в уведомлении, удаляются из очереди подписки, водяной знак последнего локального сервера клиентского доступа для подписки на задано значение водяной знак последнего события, который возвращается.
    
7. Сброс таймера времени ожидания для подписки.
    
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)

