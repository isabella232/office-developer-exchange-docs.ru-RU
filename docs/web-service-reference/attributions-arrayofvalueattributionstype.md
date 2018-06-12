---
title: Атрибуты (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: Атрибуты элемента указывает массив атрибуты для его связанное значение элемента.
ms.openlocfilehash: a64510cacb9923682418ca8a9b203c765a129bdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761529"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Атрибуты (ArrayOfValueAttributionsType)

**Атрибуты** элемента указывает массив атрибуты для его связанное **значение** элемента. 
  
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
|[Атрибуты (строка)](attribution-string.md) <br/> |Задает строку, используемую для определения атрибута.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Указывает содержимое основного текста элемента.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Указывает экземпляр массив адресов электронной почты и их связанные атрибуты.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Задает расширенные свойства для пользователя.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Указывает экземпляр массив номеров телефонов и их связанные атрибуты.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Указывает экземпляр массив почтовых адресов и их связанные атрибуты.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Указывает экземпляр массив строковых данных для элемента пользователя.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Задает экземпляр в массиве атрибутов, связанных с элементом пользователя.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

