---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Элемент ErrorMessage представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.
ms.openlocfilehash: 4ebaf91fe26083cf241826e1fc16ac184fddf57c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530644"
---
# <a name="errormessage-soap"></a>ErrorMessage (SOAP)

Элемент **ErrorMessage** представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения. 
  
```XML
<ErrorMessage/>
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
|[Отклик (SOAP)](response-soap.md) <br/> |Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
|[Усерсеттинжеррор (SOAP)](usersettingerror-soap.md) <br/> |Представляет ошибку, возвращаемую при получении параметра пользователя.  <br/> |
|[Усерреспонсе (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет сообщение об ошибке.
  
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

