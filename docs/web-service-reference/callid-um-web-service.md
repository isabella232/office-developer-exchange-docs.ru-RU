---
title: CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: Элемент CallId содержит значение, представляющее идентификатор звонка в GetCallInfo (единой системы обмена СООБЩЕНИЯМИ запрос веб-службы) или отключить (единой системы обмена СООБЩЕНИЯМИ запрос веб-службы).
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761662"
---
# <a name="callid-um-web-service"></a>CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **CallId** содержит значение, представляющее идентификатор звонка в запросе [GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-um-web-service.md) или запрос на [Отключение (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-um-web-service.md) . 
  
[GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-um-web-service.md)
  
[CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md)
  
[Отключите (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-um-web-service.md)
  
[CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-um-web-service.md) <br/> |Определяет запрос на получение сведений о звонка.  <br/> |
|[Отключите (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-um-web-service.md) <br/> |Определяет запрос на отключение вызова.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет идентификатор для звонка.
  
## <a name="remarks"></a>Замечания

Для первоначальные звонка, используйте [операцию PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) или [PlayOnPhoneGreeting операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md). Используйте значение текста, который возвращается в [PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphoneresponse-um-web-service.md) или [PlayOnPhoneGreetingResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreetingresponse-um-web-service.md) элементов для **CallId** элемент Текстовое значение. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md)
  
[Отключите операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-operation-um-web-service.md)
  
[Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md)
  
[Операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md)

