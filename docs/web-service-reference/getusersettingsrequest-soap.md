---
title: Жетусерсеттингсрекуест (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: Элемент Жетусерсеттингсрекуест представляет запрос на получение указанных параметров для одного или нескольких пользователей.
ms.openlocfilehash: 353facb5d0bbf922a23b33cbaf6f9d2e7d82bd6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530164"
---
# <a name="getusersettingsrequest-soap"></a>Жетусерсеттингсрекуест (SOAP)

Элемент **жетусерсеттингсрекуест** представляет запрос на получение указанных параметров для одного или нескольких пользователей. 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 **жетусерсеттингсрекуест**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Пользователи (SOAP)](users-soap.md) <br/> |Представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.  <br/> |
|[Рекуестедсеттингс (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена запрошенных параметров конфигурации.  <br/> |
|[Рекуестедверсион (SOAP)](requestedversion-soap.md) <br/> |Указывает конкретную версию сервера, которую необходимо использовать поставщику.  <br/> |
   
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



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)

