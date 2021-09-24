---
title: CallId (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: Элемент CallId содержит значение, которое представляет идентификатор вызова в запросе GetCallInfo (веб-служба um) или в запросе Disconnect (веб-служба um).
ms.openlocfilehash: c19f1061d81bf7683fd2c84fb1c6968826046be6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522034"
---
# <a name="callid-um-web-service"></a>CallId (веб-служба единой системы обмена сообщениями)

Элемент **CallId** содержит значение, которое представляет идентификатор вызова в [запросе GetCallInfo (веб-служба um)](getcallinfo-um-web-service.md) или [в запросе Disconnect (веб-служба um).](disconnect-um-web-service.md) 
  
[GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-um-web-service.md)
  
[CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)
  
[Disconnect (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md)
  
[CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-um-web-service.md) <br/> |Определяет запрос для получения сведений о вызове.  <br/> |
|[Disconnect (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md) <br/> |Определяет запрос на отключение вызова.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет идентификатор для вызова.
  
## <a name="remarks"></a>Заметки

Для инициалации вызова используйте операцию [PlayOnPhone (веб-служба um)](playonphone-operation-um-web-service.md) или [операцию PlayOnPhoneGreeting (веб-служба um).](playonphonegreeting-operation-um-web-service.md) Используйте текстовое значение, возвращаемое в [элементах PlayOnPhoneResponse (веб-служба um)](playonphoneresponse-um-web-service.md) или [PlayOnPhoneGreetingResponse (веб-служба um)](playonphonegreetingresponse-um-web-service.md) для текстового значения элемента **CallId.** 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[Операция Disconnect (веб-служба единой системы обмена сообщениями)](disconnect-operation-um-web-service.md)
  
[Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md)
  
[Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md)

