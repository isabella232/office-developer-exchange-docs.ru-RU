---
title: OofStatus (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: Элемент OofStatus содержит значение, которое разнонарисовка состояния единой системы обмена сообщениями Office для пользователя, который делает запрос на операцию GetUMProperties (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 4e899317defdb4ac4c27c3fdc17d7b7222dff6a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539271"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (веб-служба единой системы обмена сообщениями)

Элемент **OofStatus** содержит значение, которое содержит значение единой системы обмена сообщениями вне Office состояния для пользователя, который делает запрос [на операцию GetUMProperties (веб-службы](getumproperties-operation-um-web-service.md) единой системы обмена сообщениями). 
  
[GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (веб-служба единой системы обмена сообщениями)](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md) <br/> |Определяет ответ на запрос [операции GetUMProperties (веб-служба um).](getumproperties-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение Boolean. Ниже перечислены возможные значения.
  
- Верно
    
- Неверно
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUMProperties (веб-служба единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)

