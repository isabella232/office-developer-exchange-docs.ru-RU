---
title: уфсеттингс
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
description: Элемент Уфсеттингс содержит параметры заместителя (отсутствие на работе).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834649"
---
# <a name="oofsettings"></a>уфсеттингс

Элемент **уфсеттингс** содержит параметры заместителя (отсутствие на работе). 
  
[жетусеруфсеттингсреспонсе](getuseroofsettingsresponse.md)
  
[уфсеттингс](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 **усеруфсеттингс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[уфстате](oofstate.md) <br/> |Содержит состояние отсутствия на работе пользователя.  <br/> |
|[екстерналаудиенце](externalaudience.md) <br/> |Содержит значение, определяющее, кому отправляются внешние сообщения об отсутствии на работе.  <br/> |
|[Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md) <br/> |Содержит время, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**". Если для элемента [уфстате](oofstate.md) задано значение **Enabled** или **disabled**, значение этого элемента игнорируется.  <br/> |
|[интерналрепли](internalreply.md) <br/> |Содержит ответ о нерабочем месте, отправленный другим пользователям в домене пользователя или доверенном домене.  <br/> |
|[екстерналрепли](externalreply.md) <br/> |Содержит ответ о нерабочем месте, отправленный на адреса, не входящие в домен получателя или доверенные домены.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетусеруфсеттингсреспонсе](getuseroofsettingsresponse.md) <br/> |Содержит результаты ответа и параметры отсутствия на отсутствие для пользователя.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

