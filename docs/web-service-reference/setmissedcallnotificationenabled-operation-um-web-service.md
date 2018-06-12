---
title: Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Пример запроса SetMissedCallNotificationEnabled

### <a name="description"></a>Описание

В следующем примере запрос SetMissedCallNotificationEnabled показано, как для формирования запроса, чтобы включить уведомления о пропущенных вызовах.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Пример успешного ответа SetMissedCallNotificationEnabled

### <a name="description"></a>Описание

В следующем примере ответа PlayOnPhoneGreeting показано ответа на запрос SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

