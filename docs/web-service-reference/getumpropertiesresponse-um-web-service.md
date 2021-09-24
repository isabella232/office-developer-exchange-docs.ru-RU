---
title: GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: Элемент GetUMPropertiesResponse определяет ответ на запрос на операцию GetUMProperties (веб-службы um).
ms.openlocfilehash: 97c3850d46369d4ab533629a8b24e199db3dd44a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522966"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)

Элемент **GetUMPropertiesResponse** определяет ответ на запрос [на операцию GetUMProperties (веб-службы um).](getumproperties-operation-um-web-service.md) 
  
[GetUMPropertiesResponse (веб-служба единой системы обмена сообщениями)](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **UMProperties**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)](missedcallnotificationenabled-um-web-service.md) <br/> |Указывает, включены ли пропущенные уведомления о вызове.  <br/> |
|[PlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)](playonphonedialstring-um-web-service.md) <br/> |Содержит строку набора по умолчанию, используемую для операции [PlayOnPhone (веб-служба UM)](playonphone-operation-um-web-service.md) и [операции PlayOnPhoneGreeting (веб-служба um).](playonphonegreeting-operation-um-web-service.md)  <br/> |
|[TelephoneAccessNumbers (веб-служба единой системы обмена сообщениями)](telephoneaccessnumbers-um-web-service.md) <br/> |Содержит список номеров телефонов, которые пользователь может использовать для доступа к единой системы обмена сообщениями по телефону.  <br/> |
|[TelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](telephoneaccessfolderemail-um-web-service.md) <br/> |Содержит идентификатор папки электронной почты, из которой единая система обмена сообщениями будет читать сообщения по телефону.  <br/> |
   
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



[Операция GetUMProperties (веб-служба единой системы обмена сообщениями)](getumproperties-operation-um-web-service.md)

