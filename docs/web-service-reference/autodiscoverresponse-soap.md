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
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761534"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Усерреспонсес (SOAP)](userresponses-soap.md) <br/> |Представляет коллекцию элементов [усерреспонсе (SOAP)](userresponse-soap.md) .  <br/> |
|[Усерсеттинжеррорс (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию элементов [усерсеттинжеррор (SOAP)](usersettingerror-soap.md) .  <br/> |
|[Усерсеттингс (SOAP)](usersettings-soap.md) <br/> |Представляет коллекцию элементов [усерсеттинг (SOAP)](usersetting-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)
- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

