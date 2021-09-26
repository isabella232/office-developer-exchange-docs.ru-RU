---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: Элемент OofSettings содержит параметры Out of Office (OOF).
ms.openlocfilehash: 0a612cacb69464dfda3c1f235c32f569d3e45775
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543172"
---
# <a name="oofsettings"></a>OofSettings

Элемент **OofSettings** содержит параметры Out of Office (OOF). 
  
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
|[OofState](oofstate.md) <br/> |Содержит состояние OOF пользователя.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Содержит значение, которое определяет, кому отправляются внешние сообщения OOF.  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> |Содержит продолжительность, для которой включен статус OOF, если элемент [OofState](oofstate.md) настроен **на Scheduled**. Если элемент [OofState](oofstate.md) заданной для включения или **отключения,** значение этого элемента игнорируется.   <br/> |
|[InternalReply](internalreply.md) <br/> |Содержит ответ OOF, отправленный другим пользователям в домене пользователя или доверенного домена.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Содержит ответ OOF, отправленный на адреса, не в домены получателя или доверенные домены.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Содержит результаты ответа и параметры OOF для пользователя.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

