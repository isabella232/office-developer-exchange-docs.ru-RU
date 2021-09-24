---
title: Users (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Элемент Users представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.
ms.openlocfilehash: eabf0d2cd38396e907ca467596c2e55d1eb78e02
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538522"
---
# <a name="users-soap"></a>Users (SOAP)

Элемент **Users** представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры. 
  
```XML
<Users>
   <User/>
</Users>
```

 **Пользовательские**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[User (SOAP)](user-soap.md) <br/> |Представляет адрес электронной почты пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Представляет запрос на извлечение указанных параметров для одного или более пользователей.  <br/> |
|[Request (SOAP)](request-soap.md) <br/> |Содержит запрашиваемую конфигурацию параметров и целевых пользователей.  <br/> |
   
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

