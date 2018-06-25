---
title: Ответ (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Элемент ответа содержит ответ на операцию GetUserSettings (SOAP), операция GetDomainSettings (SOAP) или запрос операции (SOAP) GetFederationInformation.
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835179"
---
# <a name="response-soap"></a>Ответ (SOAP)

Элемент **ответа** содержит ответ на [операцию GetUserSettings (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)или запрос [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 **GetUserSettingsResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Код ошибки (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемые службой автообнаружения.  <br/> |
|[Сообщение об ошибке (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрошенного пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |Определяет ответ на [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Определяет ответ на [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).  <br/> |
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Определяет ответ на [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

