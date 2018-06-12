---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: Элемент OofSettings содержит параметры об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834649"
---
# <a name="oofsettings"></a>OofSettings

Элемент **OofSettings** содержит параметры об отсутствии на работе Office (отсутствие на работе). 
  
[GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
[OofSettings](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Содержит состояние пользователя об отсутствии на работе.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе.  <br/> |
|[Продолжительность (UserOofSettings)](duration-useroofsettings.md) <br/> |Содержит во время выполнения, для которого включен состояние об отсутствии на работе, если элемент [OofState](oofstate.md) задано значение **Запланировано**. Если элемент [OofState](oofstate.md) — это значение **включено** или **отключено**, значение этого элемента игнорируется.  <br/> |
|[InternalReply](internalreply.md) <br/> |Содержит ответа об отсутствии на работе, для других пользователей в домене или доверенном домене пользователя.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Содержит отправлено адресам за пределами домена или доверенных доменов получателя ответов об отсутствии на работе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Содержит параметры об отсутствии на работе для пользователя и результатов ответа.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

