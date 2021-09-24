---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: Элемент SearchArchiveOnly указывает, ведется ли поиск только архивного почтового ящика для неиндексируемых элементов.
ms.openlocfilehash: a4766e101394bb83a0dcebdfe5b92f576f4a4160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521683"
---
# <a name="searcharchiveonly"></a>SearchArchiveOnly

Элемент **SearchArchiveOnly** указывает, ведется ли поиск только архивного почтового ящика для неиндексируемых элементов. 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое **значение, истинное** для элемента **SearchArchiveOnly,** указывает на то, что поиск неиндексируемых элементов выполняется только в почтовом ящике архива. Текстовое значение **false** указывает, что поиск выполняется в основном почтовом ящике и архивном почтовом ящике. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

