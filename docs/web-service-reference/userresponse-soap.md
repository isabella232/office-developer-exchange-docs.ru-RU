---
title: Ответ пользователя (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: Элемент ответ пользователя представляет ответ на запрос GetUserSettings для отдельного пользователя.
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19840436"
---
# <a name="userresponse-soap"></a>Ответ пользователя (SOAP)

Элемент **ответ пользователя** представляет ответ на запрос GetUserSettings для отдельного пользователя. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **Ответ пользователя**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Код ошибки (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемые службой автообнаружения.  <br/> |
|[Сообщение об ошибке (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Содержит целевой перенаправления URL-адрес или адрес электронной почты.  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию сведений о параметрах, которые не будут получены.  <br/> |
|[Параметры пользователя (SOAP)](usersettings-soap.md) <br/> |Запрошенный параметры пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |Содержит массив ответов пользователя.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрошенного пользователя.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

