---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: Элемент ErrorCode представляет код ошибки, возвращенный службой автообнаружения.
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460094"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

Элемент **ErrorCode** представляет код ошибки, возвращенный службой автообнаружения. 
  
```XML
<ErrorCode/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Аутодисковерреспонсе (SOAP)](autodiscoverresponse-soap.md) <br/> |Представляет базовый тип для всех ответов, возвращаемых службой автообнаружения.  <br/> |
|[Домаинреспонсе (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для указанного домена.  <br/> |
|[Жетдомаинсеттингсреспонсе (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Содержит ответ на вызов [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
|[Жетфедератионинформатионреспонсе (SOAP)](getfederationinformationresponse-soap.md) <br/> |Содержит ответ на запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Отклик (SOAP)](response-soap.md) <br/> |Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md).  <br/> |
|[Усерсеттинжеррор (SOAP)](usersettingerror-soap.md) <br/> |Представляет ошибку, возвращаемую при получении параметра пользователя.  <br/> |
|[Усерреспонсе (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет код ошибки для ответа на сообщение об ошибке автообнаружения. В следующей таблице приведены возможные текстовые значения для элемента **ErrorCode** . 
  
|**Текстовое значение кода ошибки**|**Описание**|
|:-----|:-----|
|NoError  <br/> |Ошибка не обнаружена.  <br/> |
|RedirectAddress  <br/> |Вызывающий абонент должен следовать перенаправлению адресов электронной почты, которое было возвращено службой автообнаружения.  <br/> |
|RedirectUrl адресом  <br/> |Вызывающий абонент должен следовать перенаправлению URL-адреса, возвращенному службой автообнаружения.  <br/> |
|InvalidUser  <br/> |Недопустимый пользователь, переданный в запросе.  <br/> |
|InvalidRequest  <br/> |Недопустимый запрос.  <br/> |
|инвалидсеттинг  <br/> |Указан недопустимый параметр.  <br/> |
|сеттингиснотаваилабле  <br/> |Указанный параметр недоступен.  <br/> |
|ServerBusy  <br/> |Сервер перегружен и не может обработать запрос.  <br/> |
|инвалиддомаин  <br/> |Запрошенный домен не является допустимым.  <br/> |
|нотфедератед  <br/> |Организация не является Федеративной.  <br/> |
|интерналсервереррор  <br/> |Внутренняя ошибка сервера.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)
  
[Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)

