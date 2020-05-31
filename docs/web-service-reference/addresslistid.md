---
title: аддресслистид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: Элемент Аддресслистид указывает идентификатор списка адресов.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761359"
---
# <a name="addresslistid"></a>аддресслистид

Элемент **аддресслистид** указывает идентификатор списка адресов. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **аддресслистидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Идентификатор списка адресов строкового типа. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[контекстфолдерид](contextfolderid.md) <br/> |Указывает папку, предназначенную для действий, в которых используются папки. Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Задает идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[дестинатионфолдерид](destinationfolderid.md) <br/> |Указывает целевую папку для действий по копированию и перемещению.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Указывает идентификатор папки, в которую будут перемещены элементы электронной почты  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

