---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: Элемент IndexedFieldURI определяет отдельных членов словаря.
ms.openlocfilehash: 851d0d4296e926ab21e5bd1b842d5a215c27308a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539628"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

Элемент **IndexedFieldURI** определяет отдельных членов словаря. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**FieldURI** <br/> |Определяет словарь, содержащий возвращаемого участника. Этот атрибут является обязательным.  <br/> |
|**FieldIndex** <br/> |Определяет члена словаря для возврата. Этот атрибут является обязательным.  <br/> |
   
#### <a name="fielduri-attribute"></a>Атрибут FieldURI

|**Значение**|**Описание**|
|:-----|:-----|
|item:InternetMessageHeader  <br/> |Представляет заглавную часть сообщения элемента.  <br/> |
|contacts:ImAddress  <br/> |Представляет адрес обмена мгновенными сообщениями контакта.  <br/> |
|contacts:PhysicalAddress:Street  <br/> |Представляет уличный адрес контакта.  <br/> |
|contacts:PhysicalAddress:City  <br/> |Представляет город контакта.  <br/> |
|contacts:PhysicalAddress:State  <br/> |Представляет состояние контакта.  <br/> |
|contacts:PhysicalAddress:Country  <br/> |Представляет страну или регион контакта.  <br/> |
|contacts:PhysicalAddress:PostalCode  <br/> |Представляет почтовый код контакта.  <br/> |
|contacts:PhoneNumber  <br/> |Представляет телефонный номер контакта.  <br/> |
|contacts:EmailAddress  <br/> |Представляет адрес электронной почты контакта.  <br/> |
|distributionlist:Members:Member  <br/> |Представляет члена списка рассылки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Определяет дополнительные свойства для получения, набора или создания.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Представляет свойство, которое используется для определения порядка сгруппи-ных элементов для сгруппенного набора результатов FindItem.  <br/> |
|[GroupBy](groupby.md) <br/> |Указывает произвольную группу для запросов FindItem.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

