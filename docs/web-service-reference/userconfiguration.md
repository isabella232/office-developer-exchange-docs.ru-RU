---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: Элемент UserConfiguration определяет один объект конфигурации пользователя.
ms.openlocfilehash: 3821cabf777143de4a68d20a90cb78acedcff552
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538557"
---
# <a name="userconfiguration"></a>UserConfiguration

Элемент **UserConfiguration** определяет один объект конфигурации пользователя. 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 **UserConfigurationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Этот элемент необходимо использовать при создании объекта конфигурации пользователя.  <br/> |
|[ItemId](itemid.md) <br/> |Определяет идентификатор объекта конфигурации пользователя.  <br/> |
|[Словарь](dictionary.md) <br/> |Определяет набор записей свойств словаря для объекта конфигурации пользователя.  <br/> |
|[XmlData](xmldata.md) <br/> |Содержит содержимое свойства XML для объекта конфигурации пользователя.  <br/> |
|[BinaryData](binarydata.md) <br/> |Содержит содержимое свойства двоичных данных для объекта конфигурации пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Представляет запрос на создание объекта конфигурации пользователя.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Представляет ответ, возвращая объект конфигурации пользователя.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Представляет запрос на обновление объекта конфигурации пользователя.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

