---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: Элемент AddressListId указывает идентификатор списка адресов.
ms.openlocfilehash: 5348c6877e24fcc0c8873df1098f8a8e30fe4c1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541562"
---
# <a name="addresslistid"></a>AddressListId

Элемент **AddressListId** указывает идентификатор списка адресов. 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 **AddressListIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Идентификатор списка строки. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, которая ориентирована на действия, которые используют папки. Этот элемент должен присутствовать при копировании, удалении, перемещении и настройке состояния чтения в элементах беседы в целевой папке.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Указывает идентификатор папки, в которую копируется элемент электронной почты.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Указывает папку назначения для копирования и перемещения действий.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Указывает идентификатор папки, в которую перемещаются элементы электронной почты  <br/> |
   
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

