---
title: Операции подписки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: Операция Subscribe используется для подписки клиентских приложений на Push-или опрашивающие уведомления. Важно знать, что структура сообщений запросов и ответов различается в зависимости от типа уведомления о событии.
ms.openlocfilehash: c40e0e434f698c6535ff5d03fd4d45a453959dd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467048"
---
# <a name="subscribe-operation"></a>Операции подписки

Операция Subscribe используется для подписки клиентских приложений на Push-или опрашивающие уведомления. Важно знать, что структура сообщений запросов и ответов различается в зависимости от типа уведомления о событии. 
  
## <a name="pull-subscription-subscribe-request-example"></a>Пример запроса на получение подписки по запросу

### <a name="description"></a>Описание

В приведенном ниже примере кода показано, как подписаться на подписку на уведомления о событиях опрашивающей репликации. Подписка информирует клиентское приложение о добавлении новой почты в папку "Входящие" и удалении элемента из папки "Входящие". Если клиент не запрашивает сведения о событиях в течение десяти минут, произойдет время ожидания подписки. Если срок действия подписки истечет, необходимо установить новую подписку, чтобы продолжить запрашивать уведомления.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a>Элементы запроса подписки по запросу на получение подписки

В запросе используются следующие элементы:
  
- [Подписаться](subscribe.md)
    
- [пуллсубскриптионрекуест](pullsubscriptionrequest.md)
    
- [фолдеридс](folderids.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [евенттипес](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [Timeout](timeout.md)
    
Чтобы найти другие варианты сообщения запроса операции Subscribe, изучите иерархию схемы. Начните с элемента [пуллсубскриптионрекуест](pullsubscriptionrequest.md) . 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a>Пример успешных откликов подписки по запросу

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на подписку по запросу. Ответ содержит идентификатор и водяной знак подписки, которые используются для получения массива событий, связанных с подпиской. Идентификатор подписки также используется для отказа от подписки клиента из подписки.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a>Элементы ответа на подписку по запросу

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [субскрибереспонсе](subscriberesponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [субскрибереспонсемессаже](subscriberesponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [SubscriptionId (Events)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a>Пример ответа на сообщение об ошибке подписки по запросу

### <a name="description"></a>Описание

В приведенном ниже примере показан ответ об ошибке запроса на подписку. Ошибка вызвана попыткой подписаться на уведомления с помощью делегированного доступа.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a>Элементы ответа об ошибке подписки по запросу

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [субскрибереспонсе](subscriberesponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [субскрибереспонсемессаже](subscriberesponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a>Пример запроса на принудительную подписку

### <a name="description"></a>Описание

В следующем примере кода показано, как подписаться на подписку на push-уведомления о событиях. Запрос определяет папки для мониторинга, типы событий для отслеживания, частоту уведомлений о состоянии и URL-адрес веб-службы клиента, которая прослушивает push-уведомления.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Клиентская веб-служба должна быть настроена перед отправкой запроса на подписку с Push-уведомлениями; в противном случае первое уведомление не будет отправлено в действительную конечную точку, а push-уведомление завершится с ошибками. Для получения дополнительных сведений обратитесь к разделу [пример приложения push-уведомлений](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).
  
При повторной подписку создается новый идентификатор [SubscriptionId (Events)](subscriptionid-getevents.md) . Использование водяного знака предыдущей подписки для повторной подписки на момент окончания предыдущей подписки. 
  
### <a name="push-subscription-request-elements"></a>Элементы запроса на принудительную подписку

В запросе используются следующие элементы:
  
- [Подписаться](subscribe.md)
    
- [пушсубскриптионрекуест](pushsubscriptionrequest.md)
    
- [фолдеридс](folderids.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [евенттипес](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [StatusFrequency](statusfrequency.md)
    
- [Адрес](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a>Пример успешной принудительной подписки

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на принудительную подписку. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a>Элементы ответа на принудительную подписку

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [субскрибереспонсе](subscriberesponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [субскрибереспонсемессаже](subscriberesponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [SubscriptionId (Events)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="see-also"></a>См. также



[Операция по отмене подписки](unsubscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)


[Использование подписок по запросу](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[Пример приложения для push-уведомлений](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

