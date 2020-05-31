---
title: CallId (веб-служба единой системы обмена сообщениями)
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
description: Элемент CallId содержит значение, представляющее идентификатор вызова в запросе или отсоединении веб-службы единой системы обмена сообщениями в GetCallInfo (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761662"
---
# <a name="callid-um-web-service"></a>CallId (веб-служба единой системы обмена сообщениями)

Элемент **CallId** содержит значение, представляющее идентификатор вызова в запросе или [отсоединении](disconnect-um-web-service.md) веб-службы единой системы обмена сообщениями в [GetCallInfo (](getcallinfo-um-web-service.md) веб-служба единой системы обмена сообщениями). 
  
[GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-um-web-service.md)
  
[CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)
  
[Отключение (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md)
  
[CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-um-web-service.md) <br/> |Определяет запрос на получение сведений о вызове.  <br/> |
|[Отключение (веб-служба единой системы обмена сообщениями)](disconnect-um-web-service.md) <br/> |Определяет запрос на отключение вызова.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение представляет идентификатор для вызова.
  
## <a name="remarks"></a>Примечания

Для начального вызова используйте [операцию PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md) или [PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md). Используйте текстовое значение, возвращаемое в элементах [PlayOnPhoneResponse (веб-служба единой системы обмена сообщениями)](playonphoneresponse-um-web-service.md) или [плайонфонегритингреспонсе (веб-служба единой системы обмена сообщениями)](playonphonegreetingresponse-um-web-service.md) для текстового значения элемента **CallId** . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[Операция отключения (веб-служба единой системы обмена сообщениями)](disconnect-operation-um-web-service.md)
  
[Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md)
  
[Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md)

