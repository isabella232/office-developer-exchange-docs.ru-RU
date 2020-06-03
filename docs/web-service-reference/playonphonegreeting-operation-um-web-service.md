---
title: Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: Операция PlayOnPhoneGreeting выполняет исходящий вызов и воспроизводит одно из двух сообщений приветствия по телефону.
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528897"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)

Операция PlayOnPhoneGreeting выполняет исходящий вызов и воспроизводит одно из двух сообщений приветствия по телефону.
  
## <a name="playonphonegreeting-request-example"></a>Пример запроса PlayOnPhoneGreeting

### <a name="description"></a>Description

В приведенном ниже примере запроса PlayOnPhoneGreeting показано, как создать запрос на получение исходящего вызова и воссоздать сообщение обычного приветствия по телефону.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>Пример успешного ответа PlayOnPhoneGreeting

### <a name="description"></a>Description

В приведенном ниже примере ответа PlayOnPhoneGreeting показан ответ на запрос PlayOnPhoneGreeting.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-um-web-service.md)
  
[Плайонфонегритингреспонсе (веб-служба единой системы обмена сообщениями)](playonphonegreetingresponse-um-web-service.md)
  
[Гритингтипе (веб-служба единой системы обмена сообщениями)](greetingtype-um-web-service.md)
  
[dialString (веб-служба единой системы обмена сообщениями)](dialstring-um-web-service.md)

