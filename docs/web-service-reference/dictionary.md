---
title: словаря
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: Элемент Dictionary определяет набор записи словаря свойства для объекта конфигурации пользователя.
ms.openlocfilehash: 151abfe7a9a9ae05b8b61af87c33675e025920ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762093"
---
# <a name="dictionary"></a>словаря

Элемент **Dictionary** определяет набор записи словаря свойства для объекта конфигурации пользователя. 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 **UserConfigurationDictionaryType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Задает содержимое свойства запись одного словаря.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserConfiguration](userconfiguration.md) <br/> |Определяет объект конфигурации одного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

