---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: Элемент AutodiscoverResponse (SOAP) представляет базовый элемент для всех ответов, возвращаемого службой автооткрытия.
ms.openlocfilehash: 71bbb0f1aa6602a260c163ccfdfd3c3d38442e31
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514874"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

Элемент **AutodiscoverResponse (SOAP)** представляет базовый элемент для всех ответов, возвращаемого службой автооткрытия. 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Представляет коллекцию [элементов UserResponse (SOAP).](userresponse-soap.md)  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию элементов [UserSettingError (SOAP).](usersettingerror-soap.md)  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Представляет коллекцию элементов [UserSetting (SOAP).](usersetting-soap.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

