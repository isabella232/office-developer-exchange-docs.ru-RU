---
title: GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Элемент GetCallInfoResponse определяет ответа на запрос GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762711"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **GetCallInfoResponse** определяет ответ на запрос [операции GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|CallState  <br/> |Содержит значение, указывающее состояние звонка для которого сведения Запрошенная [операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .  <br/> |
|EventCause  <br/> |Содержит значение, которое указывает причину события для звонка для которого сведения Запрошенная [операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md)
  
[CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callstate-um-web-service.md)
  
[EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)](eventcause-um-web-service.md)

