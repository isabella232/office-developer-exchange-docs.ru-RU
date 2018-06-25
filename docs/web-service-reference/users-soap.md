---
title: Пользователи (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Элемент Users представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры.
ms.openlocfilehash: d7655f0020a315dcb32adbbc58610ca0e630c1fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840440"
---
# <a name="users-soap"></a>Пользователи (SOAP)

Элемент **Users** представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры. 
  
```XML
<Users>
   <User/>
</Users>
```

 **пользователи**;
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Пользователь (SOAP)](user-soap.md) <br/> |Представляет адрес электронной почты пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Представляет запрос для получения параметров указанного для одного или нескольких пользователей.  <br/> |
|[Запрос (SOAP)](request-soap.md) <br/> |Содержит параметры запрошенные конфигурации и к конечным пользователям.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)

