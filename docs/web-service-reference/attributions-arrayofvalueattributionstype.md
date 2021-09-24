---
title: Attributions (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: Элемент Attributions указывает массив атрибуций для связанного с ним элемента Value.
ms.openlocfilehash: e5483e8e7ef4745e8025106ae1f1c52e91987183
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529330"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Attributions (ArrayOfValueAttributionsType)

Элемент **Attributions** указывает массив атрибуций для связанного с ним элемента **Value.** 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Attribution (строка)](attribution-string.md) <br/> |Указывает строку, используемую для определения атрибута.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Указывает содержимое тела элемента.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Указывает экземпляр массива адресов электронной почты и связанных с ними атрибуций.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Указывает расширенные свойства для персоны.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Указывает экземпляр массива номеров телефонов и связанных с ними атрибуций.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Указывает экземпляр массива почтовых адресов и связанных с ними атрибуций.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Указывает экземпляр массива строковых данных для элемента persona.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Указывает экземпляр в массиве атрибутов, связанных с элементом persona.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

