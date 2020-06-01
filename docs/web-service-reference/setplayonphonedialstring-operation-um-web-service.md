---
title: Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)
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
description: Операция SetPlayOnPhoneDialString задает строку набора номера, используемую по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена сообщениями) и операции PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458644"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)

Операция SetPlayOnPhoneDialString задает строку набора номера, используемую по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md) и [операции PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Пример запроса SetPlayOnPhoneDialString

### <a name="description"></a>Описание

В следующем примере запроса SetPlayOnPhoneDialString показано, как сформировать запрос на установку строки набора номера по умолчанию для почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Пример успешного ответа SetPlayOnPhoneDialString

### <a name="description"></a>Описание

В приведенном ниже примере ответа Сетплайонефонедиалстринг показан ответ на запрос SetPlayOnPhoneDialString.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)](setplayonphonedialstring-um-web-service.md)
  
[Сетплайонфонедиалстрингреспонсе (веб-служба единой системы обмена сообщениями)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (веб-служба единой системы обмена сообщениями)](dialstring-um-web-service.md)

