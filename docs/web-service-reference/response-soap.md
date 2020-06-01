---
title: Отклик (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Элемент Response содержит ответ на операцию GetUserSettings (SOAP), операцию Жетдомаинсеттингс (SOAP) или запрос операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456418"
---
# <a name="response-soap"></a>Отклик (SOAP)

Элемент **Response** содержит ответ на [операцию GetUserSettings (SOAP)](getusersettings-operation-soap.md), [операцию жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)или запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 **жетусерсеттингсреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[Усерреспонсес (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрошенного пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетусерсеттингсреспонсемессаже (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |Определяет ответ на [жетусерсеттингсрекуест (SOAP)](getusersettingsrequest-soap.md) <br/> |
|[Жетдомаинсеттингсреспонсемессаже (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Определяет ответ на [жетдомаинсеттингсрекуест (SOAP)](getdomainsettingsrequest-soap.md).  <br/> |
|[Жетфедератионинформатионреспонсемессаже (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Определяет ответ на [жетфедератионинформатионрекуест (SOAP)](getfederationinformationrequest-soap.md).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

