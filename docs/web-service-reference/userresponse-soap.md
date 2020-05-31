---
title: Усерреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: Элемент Усерреспонсе представляет ответ на запрос GetUserSettings для отдельного пользователя.
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840436"
---
# <a name="userresponse-soap"></a>Усерреспонсе (SOAP)

Элемент **усерреспонсе** представляет ответ на запрос GetUserSettings для отдельного пользователя. 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **усерреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[Редиректтаржет (SOAP)](redirecttarget-soap.md) <br/> |Содержит целевой объект URL-адреса перенаправления или адреса электронной почты.  <br/> |
|[Усерсеттинжеррорс (SOAP)](usersettingerrors-soap.md) <br/> |Представляет коллекцию сведений о параметрах, которые не удалось вернуть.  <br/> |
|[Усерсеттингс (SOAP)](usersettings-soap.md) <br/> |Запрошенные параметры для пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Аррайофусерреспонсе (SOAP)](arrayofuserresponse-soap.md) <br/> |Содержит массив ответов пользователя.  <br/> |
|[Усерреспонсес (SOAP)](userresponses-soap.md) <br/> |Содержит параметры конфигурации для каждого запрошенного пользователя.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

