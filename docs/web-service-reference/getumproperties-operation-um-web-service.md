---
title: Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, отправившего запрос.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833678"
---
# <a name="getumproperties-operation-um-web-service"></a>Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, отправившего запрос.
  
## <a name="getumproperties-request-example"></a>Пример запроса GetUMProperties

### <a name="description"></a>Описание

В следующем примере запрос GetUMProperties показано, как для формирования запроса для получения свойства почтового ящика единой системы обмена сообщениями.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Пример успешного ответа GetUMProperties

### <a name="description"></a>Описание

В следующем примере ответа GetUMProperties показано ответа на запрос GetUMProperties.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md)

