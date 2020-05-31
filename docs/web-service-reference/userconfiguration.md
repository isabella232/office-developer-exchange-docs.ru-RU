---
title: усерконфигуратион
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
description: Элемент Усерконфигуратион определяет один объект конфигурации пользователя.
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840413"
---
# <a name="userconfiguration"></a>усерконфигуратион

Элемент **усерконфигуратион** определяет один объект конфигурации пользователя. 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 **усерконфигуратионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[усерконфигуратионнаме](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Этот элемент должен использоваться при создании объекта конфигурации пользователя.  <br/> |
|[Идентификатор](itemid.md) <br/> |Определяет идентификатор элемента объекта конфигурации пользователя.  <br/> |
|[Dictionary](dictionary.md) <br/> |Определяет набор записей свойств словаря для объекта конфигурации пользователя.  <br/> |
|[XmlData](xmldata.md) <br/> |Содержит содержимое свойства XML-данных для объекта конфигурации пользователя.  <br/> |
|[бинаридата](binarydata.md) <br/> |Содержит двоичное содержимое свойства данных для объекта конфигурации пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Представляет запрос на создание объекта конфигурации пользователя.  <br/> |
|[жетусерконфигуратионреспонсемессаже](getuserconfigurationresponsemessage.md) <br/> |Представляет ответ, возвращающий объект конфигурации пользователя.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Представляет запрос на обновление объекта конфигурации пользователя.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

