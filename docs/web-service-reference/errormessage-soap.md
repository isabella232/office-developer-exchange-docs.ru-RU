---
title: Сообщение об ошибке (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Сообщение об ошибке элемент представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762388"
---
# <a name="errormessage-soap"></a>Сообщение об ошибке (SOAP)

**Сообщение об ошибке** элемент представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения. 
  
```XML
<ErrorMessage/>
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
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Представляет базовый тип для всех ответов, возвращаемые службой автообнаружения.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для конкретного домена.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Содержит ответ на звонок [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Содержит ответ на запрос [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Ответ (SOAP)](response-soap.md) <br/> |Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Представляет ошибку, который возвращается при получении параметров пользователя.  <br/> |
|[Ответ пользователя (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет сообщение об ошибке.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

