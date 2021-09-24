---
title: GetCallInfoResponse (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: Элемент GetCallInfoResponse определяет ответ на запрос операции GetCallInfo (веб-служба um).
ms.openlocfilehash: 4b631bdee87e57c1612e906c725adabb9f9ce63e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526191"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (веб-служба единой системы обмена сообщениями)

Элемент **GetCallInfoResponse** определяет ответ на запрос [операции GetCallInfo (веб-служба um).](getcallinfo-operation-um-web-service.md) 
  
[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)
  
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
|CallState  <br/> |Содержит значение, которое указывает состояние вызова, для которого запрашивается информация для [операции GetCallInfo (веб-служба](getcallinfo-operation-um-web-service.md) um).  <br/> |
|EventCause  <br/> |Содержит значение, которое указывает причину события для вызова, для которого операция [GetCallInfo (веб-служба um)](getcallinfo-operation-um-web-service.md) запрашивает информацию.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[CallState (веб-служба единой системы обмена сообщениями)](callstate-um-web-service.md)
  
[EventCause (веб-служба единой системы обмена сообщениями)](eventcause-um-web-service.md)

