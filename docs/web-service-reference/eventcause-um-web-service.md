---
title: EventCause (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: Элемент EventCause содержит значение, которое указывает причину события вызова в ответ на запрос операции GetCallInfo (веб-службы um).
ms.openlocfilehash: 203cefa1a70294bec4d6f4b41aa157da6e639fce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546576"
---
# <a name="eventcause-um-web-service"></a>EventCause (веб-служба единой системы обмена сообщениями)

Элемент **EventCause** содержит значение, которое указывает причину события вызова в ответ на запрос [операции GetCallInfo (веб-службы um).](getcallinfo-operation-um-web-service.md) 
  
[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)
  
[EventCause (веб-служба единой системы обмена сообщениями)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md) <br/> |Определяет ответ на запрос [операции GetCallInfo (веб-службы um).](getcallinfo-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ниже перечислены возможные значения.
  
- Нет
    
- UserBusy
    
- NoAnswer
    
- Другие
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)

