---
title: Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: Операция IsUMEnabled определяет, включен ли для почтового ящика единая система обмена сообщениями.
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458238"
---
# <a name="isumenabled-operation-um-web-service"></a>Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)

Операция IsUMEnabled определяет, включен ли для почтового ящика единая система обмена сообщениями.
  
## <a name="isumenabled-request-example"></a>Пример запроса IsUMEnabled

### <a name="description"></a>Description

В приведенном ниже примере запроса IsUMEnabled показано, как сформировать запрос, чтобы определить, включен ли для почтового ящика единая система обмена сообщениями.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Пример успешного ответа IsUMEnabled

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос IsUMEnabled.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[IsUMEnabled (веб-служба единой системы обмена сообщениями)](isumenabled-um-web-service.md)
  
[Исуменабледреспонсе (веб-служба единой системы обмена сообщениями)](isumenabledresponse-um-web-service.md)


[XML-элементы веб-службы единой системы обмена сообщениями для Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

