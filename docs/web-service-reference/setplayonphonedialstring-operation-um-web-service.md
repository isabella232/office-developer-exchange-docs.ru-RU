---
title: Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: Операция SetPlayOnPhoneDialString задает строку набора номера для использования в качестве по умолчанию для операции PlayOnPhone (веб-служба UM) и операции PlayOnPhoneGreeting (веб-служба UM).
ms.openlocfilehash: 89f83d7b0a1d56cb0adeccbf4fa0bb67f1197253
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531911"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)

Операция SetPlayOnPhoneDialString задает строку набора номера для использования в качестве по умолчанию для операции [PlayOnPhone (веб-служба UM)](playonphone-operation-um-web-service.md) и [операции PlayOnPhoneGreeting (веб-служба UM).](playonphonegreeting-operation-um-web-service.md)
  
## <a name="setplayonphonedialstring-request-example"></a>Пример запроса SetPlayOnPhoneDialString

### <a name="description"></a>Описание

В следующем примере запроса SetPlayOnPhoneDialString показано, как сформировать запрос для настройки строки набора по умолчанию для почтового ящика.
  
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

В следующем примере ответа SetPlayOnePhoneDialString показан ответ на запрос SetPlayOnPhoneDialString.
  
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
  
[SetPlayOnPhoneDialStringResponse (веб-служба единой системы обмена сообщениями)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (веб-служба единой системы обмена сообщениями)](dialstring-um-web-service.md)

