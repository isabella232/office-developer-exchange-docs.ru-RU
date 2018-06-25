---
title: Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: Операция SetOofStatus задает значение, указывающее, следует ли воспроизводиться приветствие об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835445"
---
# <a name="setoofstatus-operation-um-web-service"></a>Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция SetOofStatus задает значение, указывающее, следует ли воспроизводиться приветствие об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.
  
## <a name="setoofstatus-request-example"></a>Пример запроса SetOofStatus

### <a name="description"></a>Описание

В следующем примере запрос SetOofStatus показано, как для формирования запроса, чтобы включить приветствие об отсутствии на работе для почтового ящика.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Пример успешного ответа SetOofStatus

### <a name="description"></a>Описание

В следующем примере ответа SetOofStatus показано ответа на запрос SetOofStatus.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatusresponse-um-web-service.md)
  
[Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)](status-um-web-servicesetoofstatus.md)

