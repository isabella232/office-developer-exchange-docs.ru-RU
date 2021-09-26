---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: Элемент UserSettingError представляет ошибку, возвращаемую в результате попытки получить параметр пользователя.
ms.openlocfilehash: 6ae3bd62e886df0b8641daa1aeb94fa7a10a7851
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542612"
---
# <a name="usersettingerror-soap"></a>UserSettingError (SOAP)

Элемент **UserSettingError** представляет ошибку, возвращаемую в результате попытки получить параметр пользователя. 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 **UserSettingError**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемый службой автооткрытия.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Respresents сообщение, связанное с кодом ошибки, который возвращается службой автооткрытия.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Представляет имя параметра пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию сведений о параметрах, которые не удалось вернуть.  <br/> |
   
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



[Элементы XML автооткрытия SOAP для Exchange 2013 г.](soap-autodiscover-xml-elements-for-exchange-2013.md)

