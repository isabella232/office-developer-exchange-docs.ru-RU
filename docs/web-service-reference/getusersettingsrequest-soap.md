---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: Элемент GetUserSettingsRequest представляет запрос на извлечение указанных параметров для одного или более пользователей.
ms.openlocfilehash: ccbcd67d4fdcb98be08acfecbf2ae066a91d65d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547395"
---
# <a name="getusersettingsrequest-soap"></a>GetUserSettingsRequest (SOAP)

Элемент **GetUserSettingsRequest** представляет запрос на извлечение указанных параметров для одного или более пользователей. 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Users (SOAP)](users-soap.md) <br/> |Представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена параметров запрашиваемой конфигурации.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Указывает конкретную версию сервера, которую поставщик хотел бы использовать.  <br/> |
   
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



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)

