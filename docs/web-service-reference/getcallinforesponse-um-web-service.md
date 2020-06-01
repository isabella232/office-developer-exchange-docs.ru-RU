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
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461207"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|каллстате  <br/> |Содержит значение, указывающее состояние вызова, для которого требуется [Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) .  <br/> |
|евенткаусе  <br/> |Содержит значение, указывающее причину события для вызова, для которого в [операции GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md) запрошены сведения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[Каллстате (веб-служба единой системы обмена сообщениями)](callstate-um-web-service.md)
  
[Евенткаусе (веб-служба единой системы обмена сообщениями)](eventcause-um-web-service.md)

