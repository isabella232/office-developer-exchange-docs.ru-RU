---
title: Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: Операция GetCallInfo возвращает состояние исходящих вызовов, который указан с CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762707"
---
# <a name="getcallinfo-operation-um-web-service"></a>Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция GetCallInfo возвращает состояние исходящих вызовов, который указан с [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Пример запроса GetCallInfo

### <a name="description"></a>Описание

В следующем примере запрос GetCallInfo показано, как для формирования запроса для получения сведений об указанном исходящих вызовов.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Пример успешного ответа GetCallInfo

### <a name="description"></a>Описание

В следующем примере ответа GetCallInfo показано ответ на запрос GetCallInfo.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinforesponse-um-web-service.md)
  
[CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md)
  
[CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callstate-um-web-service.md)
  
[EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)](eventcause-um-web-service.md)

