---
title: Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: Операция PlayOnPhoneGreeting выполняет исходящие вызовы и воспроизводит одно из двух сообщений приветствия по телефону.
ms.openlocfilehash: 540cd44d35e70e2588446996aec19aeab17f83e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543137"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)

Операция PlayOnPhoneGreeting выполняет исходящие вызовы и воспроизводит одно из двух сообщений приветствия по телефону.
  
## <a name="playonphonegreeting-request-example"></a>Пример запроса на PlayOnPhoneGreeting

### <a name="description"></a>Описание

В следующем примере запроса PlayOnPhoneGreeting показано, как сформировать запрос, чтобы сделать исходящие вызовы и сыграть нормальное приветствие по телефону.
  
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

### <a name="description"></a>Описание

В следующем примере ответа PlayOnPhoneGreeting показан ответ на запрос PlayOnPhoneGreeting.
  
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
  
[PlayOnPhoneGreetingResponse (веб-служба единой системы обмена сообщениями)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (веб-служба единой системы обмена сообщениями)](greetingtype-um-web-service.md)
  
[dialString (веб-служба единой системы обмена сообщениями)](dialstring-um-web-service.md)

