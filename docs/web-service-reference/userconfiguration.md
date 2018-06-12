---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: Элемент UserConfiguration определяет объект конфигурации одного пользователя.
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840413"
---
# <a name="userconfiguration"></a>UserConfiguration

Элемент **UserConfiguration** определяет объект конфигурации одного пользователя. 
  
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
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Этот элемент должен использоваться при создании объекта конфигурации пользователя.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Определяет идентификатор элемента объекта конфигурации пользователя.  <br/> |
|[Словарь](dictionary.md) <br/> |Определяет набор записи словаря свойства для объекта конфигурации пользователя.  <br/> |
|[XmlData](xmldata.md) <br/> |Содержит контент свойства XML данных для объекта конфигурации пользователя.  <br/> |
|[BinaryData](binarydata.md) <br/> |Свойство содержимым для объекта конфигурации пользователя двоичных данных.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Представляет запрос на создание объекта конфигурации пользователя.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Представляет ответа, которое возвращает объект конфигурации пользователя.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Представляет запрос на обновление объекта конфигурации пользователя.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

