---
title: Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: Элемент Жеткаллинфореспонсе определяет ответ на запрос для операции GetCallInfo (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762711"
---
# <a name="getcallinforesponse-um-web-service"></a>Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)

Элемент **жеткаллинфореспонсе** определяет ответ на запрос для [операции GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) . 
  
[Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **умкаллинфо**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|каллстате  <br/> |Содержит значение, указывающее состояние вызова, для которого требуется [Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) .  <br/> |
|евенткаусе  <br/> |Содержит значение, указывающее причину события для вызова, для которого в [операции GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) запрошены сведения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[Каллстате (веб-служба единой системы обмена сообщениями)](callstate-um-web-service.md)
  
[Евенткаусе (веб-служба единой системы обмена сообщениями)](eventcause-um-web-service.md)

