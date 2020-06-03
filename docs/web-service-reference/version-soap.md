---
title: Версия (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 47c9216e-6bfe-48c8-a27a-26f70db8e8d5
description: Элемент Version представляет описание версии серверного продукта.
ms.openlocfilehash: d7e6983c837b2818b7d11e1777015ec583968242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531030"
---
# <a name="version-soap"></a>Версия (SOAP)

Элемент **Version** представляет описание версии серверного продукта. 
  
```XML
<Version/>
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
|[Серверверсионинфо (SOAP)](serverversioninfo-soap.md) <br/> |Содержит версию сервера, который обработал запрос.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение элемента **Version** — это описание версии серверного продукта. 
  
## <a name="remarks"></a>Примечания

Элемент **Version** находится в заголовке SOAP ответа. 
  
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

