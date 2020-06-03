---
title: Операция по отмене подписки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: Операция unsubscribe используется для завершения подписки на уведомления по запросу. Используйте эту операцию вместо времени ожидания подписки. Эта операция допустима только для уведомлений о опрашивающей репликации.
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468028"
---
# <a name="unsubscribe-operation"></a>Операция по отмене подписки

Операция unsubscribe используется для завершения подписки на уведомления по запросу. Используйте эту операцию вместо времени ожидания подписки. Эта операция допустима только для уведомлений о опрашивающей репликации.
  
## <a name="unsubscribe-request-example"></a>Пример запроса unsubscribe

### <a name="description"></a>Description

В следующем примере показано SOAP-сообщение SOAP, отправляемое для отмены подписки клиента из службы уведомлений.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a>Элементы запроса отменять подписку

В запросе используются следующие элементы:
  
- [Отмена подписки](unsubscribe.md)
    
- [SubscriptionId (Events)](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a>Пример успешного отклика отмены подписки

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос отказа от подписки.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a>Элементы отклика для отмены подписки

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [Отмена подписки](unsubscribe.md)
    
- [респонсемессажес](responsemessages.md)
    
- [унсубскрибереспонсемессаже](unsubscriberesponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a>Пример отклика об отмене подписки

### <a name="description"></a>Description

Следующий пример ответа об отказе от подписки возникает в ответ на попытку отменить подписку с помощью идентификатора подписки, который не удается найти в хранилище Exchange.
  
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
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a>Элементы отклика на сообщение об ошибке отклика

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [унсубскрибереспонсе](unsubscriberesponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [унсубскрибереспонсемессаже](unsubscriberesponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции подписки](subscribe-operation.md)
- [Операция GetEvents](getevents-operation.md)
- [Использование подписок по запросу](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

