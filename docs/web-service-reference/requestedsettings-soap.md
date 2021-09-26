---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: Элемент RequestedSettings содержит имена параметров запрашиваемой конфигурации.
ms.openlocfilehash: b8f3beabdd231d964cb5661a7cdd06f3860f0e06
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542829"
---
# <a name="requestedsettings-soap"></a>RequestedSettings (SOAP)

Элемент **RequestedSettings** содержит имена параметров запрашиваемой конфигурации. 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 **RequestedSettings**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Setting (SOAP)](setting-soap.md) <br/> |Представляет возвращаемую настройку конфигурации.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Представляет запрос на извлечение указанных параметров для одного или более пользователей.  <br/> |
|[Request (SOAP)](request-soap.md) <br/> |Содержит запрашиваемую конфигурацию параметров и целевых пользователей.  <br/> |
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Представляет запрос [на операцию GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

