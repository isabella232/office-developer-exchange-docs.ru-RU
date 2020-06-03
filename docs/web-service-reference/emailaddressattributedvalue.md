---
title: емаиладдрессаттрибутедвалуе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: Элемент Емаиладдрессаттрибутедвалуе указывает экземпляр массива адресов электронной почты и связанные с ними атрибуты.
ms.openlocfilehash: 09fdd5921cef3d70a6da4b6d4d38f08834c5d482
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530693"
---
# <a name="emailaddressattributedvalue"></a>емаиладдрессаттрибутедвалуе

Элемент **емаиладдрессаттрибутедвалуе** указывает экземпляр массива адресов электронной почты и связанные с ними атрибуты. 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **емаиладдрессаттрибутедвалуетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение (EmailAddressType)](value-emailaddresstype.md) <br/> |Задает значение **EmailAddress** , связанное с массивом сопоставлений.  <br/> |
|[Атрибуты (Аррайофвалуеаттрибутионстипе)](attributions-arrayofvalueattributionstype.md) <br/> |Задает массив атрибутов для связанного элемента **value** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанного пользователя.  <br/> |
|[Emails2](emails2.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанного пользователя.  <br/> |
|[Emails3](emails3.md) <br/> |Указывает массив значений электронной почты и идентификаторы их исходных атрибутов для связанного пользователя.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

