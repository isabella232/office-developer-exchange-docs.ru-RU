---
title: Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: Операция IsUMEnabled определяет, включен ли почтовый ящик для единой системы обмена сообщениями.
ms.openlocfilehash: 2c637711fc34a1d1ccc484b14be3199632aaaaa3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514461"
---
# <a name="isumenabled-operation-um-web-service"></a>Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)

Операция IsUMEnabled определяет, включен ли почтовый ящик для единой системы обмена сообщениями.
  
## <a name="isumenabled-request-example"></a>Пример запроса IsUMEnabled

### <a name="description"></a>Описание

В следующем примере запроса IsUMEnabled показано, как сформировать запрос, чтобы определить, включен ли почтовый ящик для единой системы обмена сообщениями.
  
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

### <a name="description"></a>Описание

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
  
[IsUMEnabledResponse (веб-служба единой системы обмена сообщениями)](isumenabledresponse-um-web-service.md)


[XML-элементы единой веб-службы обмена сообщениями для Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

