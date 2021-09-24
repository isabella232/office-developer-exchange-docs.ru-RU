---
title: Операция Disconnect (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: Операция Disconnect завершает вызов, который определяется указанной веб-службой CallId (веб-служба um).
ms.openlocfilehash: 42e069233fbfc255d43983571c0bb28475a1fe90
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522014"
---
# <a name="disconnect-operation-um-web-service"></a>Операция Disconnect (веб-служба единой системы обмена сообщениями)

Операция Отключение завершает вызов, который определяется указанной [службой CallId (веб-служба um).](callid-um-web-service.md)
  
## <a name="disconnect-request-example"></a>Пример запроса на отключение

### <a name="description"></a>Описание

В следующем примере запроса на отключение показано, как сформировать запрос на отключение вызова.
  
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

## <a name="successful-disconnect-response-example"></a>Успешный пример ответа на отключение

### <a name="description"></a>Описание

В следующем примере ответа на отключение показан ответ на запрос Отключение.
  
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

- [Disconnect (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md) 
- [DisconnectResponse (веб-служба единой системы обмена сообщениями)](disconnectresponse-um-web-service.md) 
- [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)

