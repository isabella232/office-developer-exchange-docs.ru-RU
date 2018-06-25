---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: Элемент UserConfigurationProperties Указывает типы свойств для получения в GetUserConfiguration операции.
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840416"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

Элемент **UserConfigurationProperties** Указывает типы свойств для получения в GetUserConfiguration операции. 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Определяет запрос на получение объекта конфигурации пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **UserConfigurationProperties** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Id  <br/> |Задает свойство идентификатора.  <br/> |
|словаря  <br/> |Указывает типы свойств словаря.  <br/> |
|XmlData  <br/> |Указывает типы данных свойств XML.  <br/> |
|BinaryData  <br/> |Указывает типы свойств двоичных данных.  <br/> |
|Все  <br/> |Указывает идентификатор, словаря, XML-данных и типы свойств двоичных данных.  <br/> |
   
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

