---
title: Операция SetOofStatus (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: Операция SetOofStatus задает значение, которое указывает, следует ли играть приветствие out of Office (OOF) для пользователя, который делает запрос.
ms.openlocfilehash: ce736e7d7bea39f65843923187af3ae616ae1c86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544754"
---
# <a name="setoofstatus-operation-um-web-service"></a>Операция SetOofStatus (веб-служба единой системы обмена сообщениями)

Операция SetOofStatus задает значение, которое указывает, следует ли играть приветствие out of Office (OOF) для пользователя, который делает запрос.
  
## <a name="setoofstatus-request-example"></a>Пример запроса SetOofStatus

### <a name="description"></a>Описание

В следующем примере запроса SetOofStatus показано, как сформировать запрос, чтобы включить Office для почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Пример успешного ответа SetOofStatus

### <a name="description"></a>Описание

В следующем примере ответа SetOofStatus показан ответ на запрос SetOofStatus.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (веб-служба единой системы обмена сообщениями)](setoofstatusresponse-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetOofStatus)](status-um-web-servicesetoofstatus.md)

