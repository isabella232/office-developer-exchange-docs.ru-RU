---
title: Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
ms.openlocfilehash: 31f59887041aac02e5876b596931902373870203
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521419"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)

Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Пример запроса SetMissedCallNotificationEnabled

### <a name="description"></a>Описание

В следующем примере запроса SetMissedCallNotificationEnabled показано, как сформировать запрос, чтобы включить уведомления о пропущенных вызовах.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Пример успешного ответа SetMissedCallNotificationEnabled

### <a name="description"></a>Описание

В следующем примере ответа PlayOnPhoneGreeting показан ответ на запрос SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (веб-служба единой системы обмена сообщениями)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

