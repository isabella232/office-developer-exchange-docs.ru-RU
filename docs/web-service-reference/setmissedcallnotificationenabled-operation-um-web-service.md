---
title: Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)
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
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467398"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)

Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Пример запроса SetMissedCallNotificationEnabled

### <a name="description"></a>Description

В следующем примере запроса SetMissedCallNotificationEnabled показано, как сформировать запрос на включение уведомлений о пропущенных звонках.
  
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

### <a name="description"></a>Description

В приведенном ниже примере ответа PlayOnPhoneGreeting показан ответ на запрос SetMissedCallNotificationEnabled.
  
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
  
[Сетмисседкаллнотификатионенабледреспонсе (веб-служба единой системы обмена сообщениями)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

