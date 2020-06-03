---
title: Операция SetOofStatus (веб-служба единой системы обмена сообщениями)
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
description: Операция SetOofStatus задает значение, указывающее, следует ли воспроизводить приветствие "нет на месте" для пользователя, который отправляет запрос.
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467356"
---
# <a name="setoofstatus-operation-um-web-service"></a>Операция SetOofStatus (веб-служба единой системы обмена сообщениями)

Операция SetOofStatus задает значение, указывающее, следует ли воспроизводить приветствие "нет на месте" для пользователя, который отправляет запрос.
  
## <a name="setoofstatus-request-example"></a>Пример запроса SetOofStatus

### <a name="description"></a>Description

В приведенном ниже примере запроса SetOofStatus показано, как сформировать запрос на включение приветствия "нет на месте" для почтового ящика.
  
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

### <a name="description"></a>Description

В приведенном ниже примере ответа SetOofStatus показан ответ на запрос SetOofStatus.
  
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
  
[Сетуфстатусреспонсе (веб-служба единой системы обмена сообщениями)](setoofstatusresponse-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetOofStatus)](status-um-web-servicesetoofstatus.md)

