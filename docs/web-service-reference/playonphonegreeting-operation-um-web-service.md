---
title: Операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Операция PlayOnPhoneGreeting исходящего звонка и воспроизведения один из двух приветствие сообщения по телефону.
ms.openlocfilehash: 85ba76c7638911678c1ef1aef88f47fdab2c6a4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834828"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция PlayOnPhoneGreeting исходящего звонка и воспроизведения один из двух приветствие сообщения по телефону.
  
## <a name="playonphonegreeting-request-example"></a>Пример запроса PlayOnPhoneGreeting

### <a name="description"></a>Описание

В следующем примере запрос PlayOnPhoneGreeting показано, как для формирования запроса на выполнение исходящего звонка и воспроизведение обычных приветственное сообщение на телефон.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>Пример успешного ответа PlayOnPhoneGreeting

### <a name="description"></a>Описание

В следующем примере ответа PlayOnPhoneGreeting показано ответа на запрос PlayOnPhoneGreeting.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (веб-служба единой системы обмена СООБЩЕНИЯМИ)](greetingtype-um-web-service.md)
  
[dialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](dialstring-um-web-service.md)
