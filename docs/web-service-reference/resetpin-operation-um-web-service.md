---
title: Операция ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: Операция ResetPIN изменений ПИН-кода (телефонного интерфейса пароль) в новое значение в случайном порядке.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835146"
---
# <a name="resetpin-operation-um-web-service"></a>Операция ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Операция ResetPIN изменений ПИН-кода (телефонного интерфейса пароль) в новое значение в случайном порядке.
  
## <a name="remarks"></a>Замечания

Операция ResetPIN создает новый ПИН-код на основе политик ПИН-кода. Если операция выполнена успешно, в почтовый ящик пользователя, отправляется сообщение электронной почты, содержащее новый ПИН-код. В случае сбоя операции, он будет исключение, который содержит сведения о сбое.
  
## <a name="resetpin-request-example"></a>Пример запроса ResetPIN

### <a name="description"></a>Описание

В следующем примере запрос ResetPIN показано, как для формирования запроса для сброса ПИН-код для почтового ящика.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Пример успешного ответа ResetPIN

### <a name="description"></a>Описание

В следующем примере ответа ResetPIN показано ответа на запрос ResetPIN.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)](resetpin-um-web-service.md)
  
[ResetPINResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](resetpinresponse-um-web-service.md)

