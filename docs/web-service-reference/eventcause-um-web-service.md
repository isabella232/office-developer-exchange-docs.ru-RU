---
title: EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: Элемент EventCause содержит значение, указывающее, вызвавшего событие звонок в ответ на запрос GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762393"
---
# <a name="eventcause-um-web-service"></a>EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **EventCause** содержит значение, указывающее, вызвавшего событие звонок в ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinforesponse-um-web-service.md)
  
[EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)](eventcause-um-web-service.md)
  
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
|[GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinforesponse-um-web-service.md) <br/> |Определяет ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Ниже перечислены возможные значения.
  
- Нет
    
- UserBusy
    
- NoAnswer
    
- Other (другие)
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinforesponse-um-web-service.md)

