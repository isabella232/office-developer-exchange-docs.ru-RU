---
title: Операция отключения (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: Операция отключения завершает вызов, идентифицируемый заданным CallId (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529072"
---
# <a name="disconnect-operation-um-web-service"></a>Операция отключения (веб-служба единой системы обмена сообщениями)

Операция отключения завершает вызов, идентифицируемый заданным [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md).
  
## <a name="disconnect-request-example"></a>Пример запроса на отключение

### <a name="description"></a>Description

В приведенном ниже примере запроса на отключение показано, как сформировать запрос на отключение вызова.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>Пример отклика об успешном отключении

### <a name="description"></a>Description

В приведенном ниже примере ответа на отключение показан ответ на запрос на отключение.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также

- [Отключение (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md) 
- [Дисконнектреспонсе (веб-служба единой системы обмена сообщениями)](disconnectresponse-um-web-service.md) 
- [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)

