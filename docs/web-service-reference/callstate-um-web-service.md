---
title: CallState (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: Элемент CallState содержит значение, которое указывает состояние вызова.
ms.openlocfilehash: 9435124e98cfb75beab5917c1e832096ca193e0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519970"
---
# <a name="callstate-um-web-service"></a>CallState (веб-служба единой системы обмена сообщениями)

Элемент **CallState** содержит значение, которое указывает состояние вызова. 
  
[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)
  
[CallState (веб-служба единой системы обмена сообщениями)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md) <br/> |Определяет ответ на операцию [GetCallInfo (веб-служба um).](getcallinfo-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Ниже перечислены возможные значения.
  
- Idle
    
- Connecting
    
- Оповещено
    
- Подключение
    
- Отключено
    
- Входящие
    
- Перенос
    
- Переададка
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetCallInfo (веб-служба единой системы обмена сообщениями)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (веб-служба единой системы обмена сообщениями)](getcallinforesponse-um-web-service.md)

