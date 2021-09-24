---
title: UserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: Элемент UserResponse представляет ответ на запрос GetUserSettings для отдельного пользователя.
ms.openlocfilehash: 8def0183a5c2e212e80699a3c2f58c64f67ce690
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538543"
---
# <a name="userresponse-soap"></a>UserResponse (SOAP)

Элемент **UserResponse** представляет ответ на запрос GetUserSettings для отдельного пользователя. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **UserResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемый службой автооткрытия.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, который возвращается службой автооткрытия.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Содержит цель URL-адреса перенаправления или адреса электронной почты.  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию сведений о параметрах, которые не удалось вернуть.  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Запрашиваемая настройка для пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |Содержит массив ответов пользователей.  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрашиваемой пользователя.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия SOAP для Exchange 2013 г.](soap-autodiscover-xml-elements-for-exchange-2013.md)

