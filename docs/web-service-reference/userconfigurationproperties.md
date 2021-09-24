---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: Элемент UserConfigurationProperties указывает типы свойств для получения в операции GetUserConfiguration.
ms.openlocfilehash: 0aed3ffc680ac881410469fe762349739ba924a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515007"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

Элемент **UserConfigurationProperties** указывает типы свойств для получения в операции GetUserConfiguration. 
  
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
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Указывает запрос на получения объекта конфигурации пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **UserConfigurationProperties.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Id  <br/> |Указывает свойство идентификатора.  <br/> |
|Dictionary  <br/> |Указывает типы свойств словаря.  <br/> |
|XmlData  <br/> |Указывает типы свойств XML-данных.  <br/> |
|BinaryData  <br/> |Указывает типы свойств двоичных данных.  <br/> |
|Все  <br/> |Указывает идентификатор, словарь, XML-данные и типы свойств двоичных данных.  <br/> |
   
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

