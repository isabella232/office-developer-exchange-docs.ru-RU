---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: Элемент EmailAddressAttributedValue указывает экземпляр массива адресов электронной почты и связанных с ними атрибуций.
ms.openlocfilehash: 2b5e9b431b6a62c63e815bfee190c923f454c867
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519767"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

Элемент **EmailAddressAttributedValue** указывает экземпляр массива адресов электронной почты и связанных с ними атрибуций. 
  
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
|[Value (EmailAddressType)](value-emailaddresstype.md) <br/> |Указывает значение **emailAddress,** связанного с массивом атрибуций.  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Указывает массив атрибуций для связанного с ним **элемента Value.**  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанной персоны.  <br/> |
|[Emails2](emails2.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанной персоны.  <br/> |
|[Emails3](emails3.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанной персоны.  <br/> |
   
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

