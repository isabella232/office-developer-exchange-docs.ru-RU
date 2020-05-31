---
title: Рекуестедсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: Элемент Рекуестедсеттингс содержит имена запрошенных параметров конфигурации.
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835136"
---
# <a name="requestedsettings-soap"></a>Рекуестедсеттингс (SOAP)

Элемент **рекуестедсеттингс** содержит имена запрошенных параметров конфигурации. 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 **рекуестедсеттингс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Параметр (SOAP)](setting-soap.md) <br/> |Представляет параметр конфигурации, который необходимо вернуть.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетусерсеттингсрекуест (SOAP)](getusersettingsrequest-soap.md) <br/> |Представляет запрос на получение указанных параметров для одного или нескольких пользователей.  <br/> |
|[Запрос (SOAP)](request-soap.md) <br/> |Содержит запрошенные параметры конфигурации и конечных пользователей.  <br/> |
|[Жетдомаинсеттингсрекуест (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

