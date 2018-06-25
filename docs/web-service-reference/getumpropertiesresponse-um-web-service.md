---
title: GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: Элемент GetUMPropertiesResponse определяет ответа на запрос GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833685"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **GetUMPropertiesResponse** определяет ответ на запрос [операции GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md)
  
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
|[MissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)](missedcallnotificationenabled-um-web-service.md) <br/> |Указывает, включены ли уведомления о пропущенных вызовах.  <br/> |
|[PlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonedialstring-um-web-service.md) <br/> |Содержит строку звонков по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) и [PlayOnPhoneGreeting операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (веб-служба единой системы обмена СООБЩЕНИЯМИ)](telephoneaccessnumbers-um-web-service.md) <br/> |Содержит список телефонных номеров, которые пользователь может использовать для доступа к единой системе обмена сообщениями по телефону.  <br/> |
|[TelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](telephoneaccessfolderemail-um-web-service.md) <br/> |Содержит идентификатор для папки электронной почты, из которого единой системы обмена сообщениями будет читать сообщения по телефону.  <br/> |
   
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



[Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md)

