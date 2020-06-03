---
title: усерконфигуратионпропертиес
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
description: Элемент Усерконфигуратионпропертиес указывает типы свойств, которые необходимо получить в операции GetUserConfiguration.
ms.openlocfilehash: af6bee64516a7410d96ecc7581e8e819f550ddc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466495"
---
# <a name="userconfigurationproperties"></a>усерконфигуратионпропертиес

Элемент **усерконфигуратионпропертиес** указывает типы свойств, которые необходимо получить в операции GetUserConfiguration. 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **усерконфигуратионпропертитипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Указывает запрос на получение объекта конфигурации пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **усерконфигуратионпропертиес** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Id  <br/> |Задает свойство идентификатора.  <br/> |
|Dictionary  <br/> |Задает типы свойств словаря.  <br/> |
|XmlData  <br/> |Определяет типы свойств данных XML.  <br/> |
|бинаридата  <br/> |Задает типы свойств двоичных данных.  <br/> |
|Все  <br/> |Задает идентификатор, словарь, XML-данные и типы свойств двоичных данных.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

