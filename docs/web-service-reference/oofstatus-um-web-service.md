---
title: OofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: Элемент OofStatus содержит значение, indicaties состояние единой системы обмена сообщениями нет на работе для пользователя, который осуществляет запрос GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834650"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **OofStatus** содержит значение, indicaties состояние единой системы обмена сообщениями нет на работе для пользователя, который делает запрос [GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)](oofstatus-um-web-service.md)
  
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
|[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md) <br/> |Определяет ответ на запрос [операции GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение типа Boolean текст является обязательным. Ниже перечислены возможные значения.
  
- Истина
    
- Ложь
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md)

