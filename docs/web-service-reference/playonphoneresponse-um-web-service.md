---
title: PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: Элемент PlayOnPhoneResponse определяет ответа на запрос PlayOnPhone операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834832"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **PlayOnPhoneResponse** определяет ответ на запрос [операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) . 
  
[PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение является идентификатором звонка для значения [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md) в запрос [GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) или в запросе на [операции отключения (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-operation-um-web-service.md) . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md)

