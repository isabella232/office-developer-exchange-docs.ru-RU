---
title: TelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- TelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 5d32ae22-bb9f-4352-a251-d516b66ff35b
description: Элемент TelephoneAccessFolderEmail содержит значение, указывающий идентификатор папки электронной почты из которых единой системы обмена сообщениями будет читать сообщения по телефону, содержащихся в ответ на запрос GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: e564e8ed44c3132ef32039e92982ff935c3e49e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840145"
---
# <a name="telephoneaccessfolderemail-um-web-service"></a>TelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **TelephoneAccessFolderEmail** содержит значение, указывающий идентификатор папки электронной почты из которых единой системы обмена сообщениями будет читать сообщения по телефону, содержащихся в ответ на [GetUMProperties операции (веб-служба единой системы обмена СООБЩЕНИЯМИ) ](getumproperties-operation-um-web-service.md)запроса. 
  
[GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumpropertiesresponse-um-web-service.md)
  
[TelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](telephoneaccessfolderemail-um-web-service.md)
  
```xml
<TelephoneAccessFolderEmail/>
```

 **string**
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

Текстовое значение является обязательным.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getumproperties-operation-um-web-service.md)
  
[Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md)

