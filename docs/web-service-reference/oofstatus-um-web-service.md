---
title: Уфстатус (веб-служба единой системы обмена сообщениями)
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
description: Элемент Уфстатус содержит значение, указывающее состояние выхода из системы для пользователя, который выполняет операцию GetUMProperties (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460577"
---
# <a name="oofstatus-um-web-service"></a>Уфстатус (веб-служба единой системы обмена сообщениями)

Элемент **уфстатус** содержит значение, указывающее состояние выхода из системы для пользователя, который выполняет [операцию GetUMProperties (веб-служба единой системы обмена](getumproperties-operation-um-web-service.md) сообщениями). 
  
[Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)
  
[Уфстатус (веб-служба единой системы обмена сообщениями)](oofstatus-um-web-service.md)
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md) <br/> |Определяет ответ на запрос [GetUMPropertiesной операции (веб-службы единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение Boolean. Ниже перечислены возможные значения.
  
- Верно.
    
- False
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUMProperties (веб-служба единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md)
  
[Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)

