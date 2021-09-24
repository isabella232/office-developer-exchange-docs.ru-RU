---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: Элемент ErrorCode представляет код ошибки, который возвращается службой автооткрытия.
ms.openlocfilehash: fa40cb8b7a2ec80ecf752058f540969013748d39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530775"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

Элемент **ErrorCode** представляет код ошибки, который возвращается службой автооткрытия. 
  
```XML
<ErrorCode/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Представляет базовый тип для всех ответов, возвращаемого службой автооткрытия.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Содержит заданные параметры для указанного домена.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Содержит ответ на вызов [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Содержит ответ на запрос [операции GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[Response (SOAP)](response-soap.md) <br/> |Содержит ответ на запрос [операции GetUserSettings (SOAP).](getusersettings-operation-soap.md)  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Представляет ошибку, возвращаемую при искомом параметре пользователя.  <br/> |
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет код ошибки для ответа на ошибку автонаруже. В следующей таблице перечислены возможные текстовые значения элемента **ErrorCode.** 
  
|**Текстовое значение кода ошибки**|**Описание**|
|:-----|:-----|
|NoError  <br/> |Ошибки не было.  <br/> |
|RedirectAddress  <br/> |Вызываемая должна следовать перенаправлению адресов электронной почты, возвращенным автонаружением.  <br/> |
|RedirectUrl  <br/> |Вызываемая должна следовать перенаправлению URL-адресов, возвращенным автонаружением.  <br/> |
|InvalidUser  <br/> |Пользователь, переданный в запросе, является недействительным.  <br/> |
|InvalidRequest  <br/> |Запрос недействителен.  <br/> |
|InvalidSetting  <br/> |Указанный параметр недействителен.  <br/> |
|SettingIsNotAvailable  <br/> |Указанный параметр не доступен.  <br/> |
|ServerBusy  <br/> |Сервер слишком занят для обработки запроса.  <br/> |
|InvalidDomain  <br/> |Запрашиваемая доменная область не является допустимой.  <br/> |
|NotFederated  <br/> |Организация не является федераированной.  <br/> |
|InternalServerError  <br/> |Существует внутренняя ошибка сервера.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

