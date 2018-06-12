---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: Элемент EmailAddressAttributedValue указывает экземпляр массива адреса электронной почты и их связанные атрибуты.
ms.openlocfilehash: 3bcbb5c0a2bc9a2dc24516b5fc62e6e3363a360b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762291"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

Элемент **EmailAddressAttributedValue** указывает экземпляр массива адреса электронной почты и их связанные атрибуты. 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение (EmailAddressType)](value-emailaddresstype.md) <br/> |Указывает, что значение **EmailAddress** , связанной с массивом атрибуты.  <br/> |
|[Атрибуты (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Указывает массив атрибуты для его связанное **значение** элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Указывает массив значений электронной почты и идентификаторы их атрибуты источника для связанного пользователя.  <br/> |
|[Emails2](emails2.md) <br/> |Указывает массив значений электронной почты и идентификаторы их атрибуты источника для связанного пользователя.  <br/> |
|[Emails3](emails3.md) <br/> |Указывает массив значений электронной почты и идентификаторы их атрибуты источника для связанного пользователя.  <br/> |
   
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

