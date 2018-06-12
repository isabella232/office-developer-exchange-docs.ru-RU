---
title: Код ошибки (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: Элемент ErrorCode представляет код ошибки, возвращаемые службой автообнаружения.
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762378"
---
# <a name="errorcode-soap"></a>Код ошибки (SOAP)

Элемент **ErrorCode** представляет код ошибки, возвращаемые службой автообнаружения. 
  
```XML
<ErrorCode/>
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
|[Ответ (SOAP)](response-soap.md) <br/> |Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md).  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Представляет ошибку, который возвращается при получении параметров пользователя.  <br/> |
|[Ответ пользователя (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет код ошибки для возврату ошибки службы автообнаружения. В следующей таблице перечислены возможные значения для элемента **код ошибки** . 
  
|**Текстовое значение кода ошибки**|**Описание**|
|:-----|:-----|
|NoError  <br/> |Ошибок не было.  <br/> |
|RedirectAddress  <br/> |Необходимо выполнить перенаправление адреса электронной почты, возвращаемые автообнаружения, вызывающего абонента.  <br/> |
|RedirectUrl  <br/> |Необходимо выполнить перенаправление URL-адреса, возвращаемые автообнаружения, вызывающего абонента.  <br/> |
|InvalidUser  <br/> |Пользователь, который был передан в запросе является недопустимым.  <br/> |
|InvalidRequest  <br/> |Недопустимый запрос.  <br/> |
|InvalidSetting  <br/> |Указанный параметр является недопустимым.  <br/> |
|SettingIsNotAvailable  <br/> |Указанный параметр недоступен.  <br/> |
|ServerBusy  <br/> |Сервер занят обработать запрос.  <br/> |
|InvalidDomain  <br/> |Запрошенный домен не является допустимым.  <br/> |
|NotFederated  <br/> |Организации не федеративными.  <br/> |
|InternalServerError  <br/> |Существует Внутренняя ошибка сервера.  <br/> |
   
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

