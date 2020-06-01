---
title: Операция GetCallInfo (веб-служба единой системы обмена сообщениями)
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
description: Операция GetCallInfo возвращает состояние исходящего вызова, указанного в параметре CallId (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461242"
---
# <a name="getcallinfo-operation-um-web-service"></a>Операция GetCallInfo (веб-служба единой системы обмена сообщениями)

Операция GetCallInfo возвращает состояние исходящего вызова, указанного в параметре [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Пример запроса GetCallInfo

### <a name="description"></a>Описание

В следующем примере запроса GetCallInfo показано, как сформировать запрос для получения сведений об указанном исходящем вызове.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Пример успешного ответа GetCallInfo

### <a name="description"></a>Описание

В приведенном ниже примере ответа GetCallInfo показан ответ на запрос GetCallInfo.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-um-web-service.md)
  
[Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)
  
[CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)
  
[Каллстате (веб-служба единой системы обмена сообщениями)](callstate-um-web-service.md)
  
[Евенткаусе (веб-служба единой системы обмена сообщениями)](eventcause-um-web-service.md)

