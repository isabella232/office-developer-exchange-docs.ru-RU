---
title: Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: Операция PlayOnPhone выполняет исходящий вызов и воспроизводит указанное сообщение по телефону, заданному элементом DialString.
ms.openlocfilehash: c5ff82bcd822aa2c659d1782ea4a1349d198bc80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466236"
---
# <a name="playonphone-operation-um-web-service"></a>Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)

Операция PlayOnPhone выполняет исходящий вызов и воспроизводит указанное сообщение по телефону, заданному элементом **DialString** . 
  
## <a name="playonphone-request-example"></a>Пример запроса PlayOnPhone

### <a name="description"></a>Описание

В приведенном ниже примере запроса PlayOnPhone показано, как создать запрос на получение исходящего вызова и прослушивание сообщения.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>Пример успешного ответа PlayOnPhone

### <a name="description"></a>Описание

В приведенном ниже примере ответа PlayOnPhone показан ответ на запрос PlayOnPhone.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (веб-служба единой системы обмена сообщениями)](playonphoneresponse-um-web-service.md)
  
[Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md)

