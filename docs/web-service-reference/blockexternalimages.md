---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: Элемент BlockExternalImages указывает, заблокированы ли внешние изображения в текстовых телах HTML.
ms.openlocfilehash: 82ddb7e53f351324783fa39e3b76c9c0534b8193
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543585"
---
# <a name="blockexternalimages"></a>BlockExternalImages

Элемент **BlockExternalImages** указывает, заблокированы ли внешние изображения в текстовых телах HTML. 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Определяет свойства папок, которые необходимо включить в ответ GetFolder, FindFolder или SyncFolderHierarchy.  <br/> |
|[ItemShape](itemshape.md) <br/> |Определяет свойства и содержимое элемента, которые необходимо включить в ответ GetItem, FindItem или SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое **значение, истинное** для **элемента BlockExternalImages,** указывает на блокировку внешних изображений в htmL-телах. Значение false **указывает,** что внешние изображения разрешены. 
  
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

