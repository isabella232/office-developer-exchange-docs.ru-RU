---
title: Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: Операция SetPlayOnPhoneDialString задает телефонным строку, используемую по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ) и операции PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция SetPlayOnPhoneDialString задает телефонным строку, используемую по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) , а [операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Пример запроса SetPlayOnPhoneDialString

### <a name="description"></a>Описание

В следующем примере запрос SetPlayOnPhoneDialString показано, как для формирования запроса, чтобы задать строку звонков по умолчанию для почтового ящика.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Пример успешного ответа SetPlayOnPhoneDialString

### <a name="description"></a>Описание

В следующем примере ответа SetPlayOnePhoneDialString показано ответа на запрос SetPlayOnPhoneDialString.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](dialstring-um-web-service.md)

