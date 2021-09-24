---
title: Операция GetUMProperties (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, который делает запрос.
ms.openlocfilehash: 8d051196e83e1f927692b517e1ab3e95bb0060db
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515819"
---
# <a name="getumproperties-operation-um-web-service"></a>Операция GetUMProperties (веб-служба единой системы обмена сообщениями)

Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, который делает запрос.
  
## <a name="getumproperties-request-example"></a>Пример запроса GetUMProperties

### <a name="description"></a>Описание

В следующем примере запроса GetUMProperties показано, как сформировать запрос для получения свойств единой системы обмена сообщениями почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Пример успешного ответа GetUMProperties

### <a name="description"></a>Описание

В следующем примере ответа GetUMProperties показан ответ на запрос GetUMProperties.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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



[GetUMProperties (веб-служба единой системы обмена сообщениями)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)

