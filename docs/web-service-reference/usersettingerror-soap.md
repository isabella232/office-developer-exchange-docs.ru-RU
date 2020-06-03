---
title: Усерсеттинжеррор (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: Элемент Усерсеттинжеррор представляет ошибку, которая возвращается в результате попытки получить параметр пользователя.
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468609"
---
# <a name="usersettingerror-soap"></a>Усерсеттинжеррор (SOAP)

Элемент **усерсеттинжеррор** представляет ошибку, которая возвращается в результате попытки получить параметр пользователя. 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 **усерсеттинжеррор**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Респресентс сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[Свойства settingname (SOAP)](settingname-soap.md) <br/> |Представляет имя параметра пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Усерсеттинжеррорс (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию сведений о параметрах, которые не удалось вернуть.  <br/> |
   
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



[XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

