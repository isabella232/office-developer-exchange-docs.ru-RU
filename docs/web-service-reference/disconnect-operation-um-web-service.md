---
title: Отключите операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Операции отключения завершение работы звонок, который идентифицируется с указанным CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762134"
---
# <a name="disconnect-operation-um-web-service"></a>Отключите операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операции отключения завершение работы звонок, который идентифицируется с указанным [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md).
  
## <a name="disconnect-request-example"></a>Отключите пример запроса

### <a name="description"></a>Описание

В следующем примере запрос на отключение показано, как для формирования запроса, чтобы прервать вызов.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>Пример успешного ответа Disconnect

### <a name="description"></a>Описание

В следующем примере ответа Disconnect показано ответа на запрос отключения.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также

- [Отключите (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-um-web-service.md) 
- [DisconnectResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnectresponse-um-web-service.md) 
- [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md)

