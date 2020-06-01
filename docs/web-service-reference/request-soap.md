---
title: Запрос (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: Элемент Request содержит запрошенные параметры конфигурации и целевые пользователи.
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448991"
---
# <a name="request-soap"></a>Запрос (SOAP)

Элемент **request** содержит запрошенные параметры конфигурации и целевые пользователи. 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
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

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетусерсеттингсрекуестмессаже (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |Представляет запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
   
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

