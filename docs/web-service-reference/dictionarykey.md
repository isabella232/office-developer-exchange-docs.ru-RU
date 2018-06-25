---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: Элемент DictionaryKey указывает ключ словаря для свойства словаря.
ms.openlocfilehash: 7e706f16fe155278ea56f303ffbb5971c1779879
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762097"
---
# <a name="dictionarykey"></a>DictionaryKey

Элемент **DictionaryKey** указывает ключ словаря для свойства словаря. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тип (UserConfiguration)](type-userconfiguration.md) <br/> | Указывает тип объекта dictionary.<br/><br/>Тип может иметь одно из следующих значений string:<br/><br/>-Даты и времени  <br/>-Boolean  <br/>-Байтовое  <br/>-Строка  <br/>-Integer32  <br/>-UnsignedInteger32  <br/>-Integer64  <br/>-UnsignedInteger64  <br/>-StringArray  <br/>-ByteArray  <br/> |
|[Значение (UserConfiguration)](value-userconfiguration.md) <br/> |Указывает значение объекта dictionary как строку.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Задает содержимое свойства запись одного словаря.  <br/> |
   
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

