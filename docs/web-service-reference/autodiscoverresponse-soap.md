---
title: Аутодисковерреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: Элемент Аутодисковерреспонсе (SOAP) представляет базовый элемент для всех ответов, возвращаемых службой автообнаружения.
ms.openlocfilehash: 81fd557578bde9552d07e24386c93903e44a9afa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463967"
---
# <a name="autodiscoverresponse-soap"></a>Аутодисковерреспонсе (SOAP)

Элемент **аутодисковерреспонсе (SOAP)** представляет базовый элемент для всех ответов, возвращаемых службой автообнаружения. 
  
- [Аутодисковерреспонсе (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **аутодисковерреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Усерреспонсес (SOAP)](userresponses-soap.md) <br/> |Представляет коллекцию элементов [усерреспонсе (SOAP)](userresponse-soap.md) .  <br/> |
|[Усерсеттинжеррорс (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию элементов [усерсеттинжеррор (SOAP)](usersettingerror-soap.md) .  <br/> |
|[Усерсеттингс (SOAP)](usersettings-soap.md) <br/> |Представляет коллекцию элементов [усерсеттинг (SOAP)](usersetting-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
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

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)
- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

