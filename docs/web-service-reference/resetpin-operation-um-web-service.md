---
title: Операция ResetPIN (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: Операция ResetPIN меняет ПИН-код (пароль TUI) на новое случайное значение.
ms.openlocfilehash: 12f1e5719184df84f6c29ab3d02cc362f87abc76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539110"
---
# <a name="resetpin-operation-um-web-service"></a>Операция ResetPIN (веб-служба единой системы обмена сообщениями)

Операция ResetPIN меняет ПИН-код (пароль TUI) на новое случайное значение.
  
## <a name="remarks"></a>Заметки

Операция ResetPIN создает новый ПИН-код на основе политик ПИН-кода. Если операция будет успешной, в почтовый ящик пользователя отправляется сообщение электронной почты с новым ПИН-кодом. В случае сбоя операции будет забрасываться исключение, содержа которое содержит сведения о сбое.
  
## <a name="resetpin-request-example"></a>Пример запроса resetPIN

### <a name="description"></a>Описание

В следующем примере запроса ResetPIN показано, как сформировать запрос для сброса ПИН-кода для почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Пример успешного ответа resetPIN

### <a name="description"></a>Описание

В следующем примере ответа ResetPIN показан ответ на запрос ResetPIN.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[ResetPIN (веб-служба единой системы обмена сообщениями)](resetpin-um-web-service.md)
  
[ResetPINResponse (веб-служба единой системы обмена сообщениями)](resetpinresponse-um-web-service.md)

