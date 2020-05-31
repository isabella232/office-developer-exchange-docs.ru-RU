---
title: сеарчарчивеонли
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: Элемент Сеарчарчивеонли указывает, выполняется ли поиск только в архивном почтовом ящике для элементов, которые не индексируются.
ms.openlocfilehash: ac9d3262784d8052486c631ef3e99e650d4757c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835293"
---
# <a name="searcharchiveonly"></a>сеарчарчивеонли

Элемент **сеарчарчивеонли** указывает, выполняется ли поиск только в архивном почтовом ящике для элементов, которые не индексируются. 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **сеарчарчивеонли** указывает на то, что поиск неиндексируемого элемента выполняется только в архивном почтовом ящике. Текстовое значение **false** указывает на то, что выполняется поиск по основному почтовому ящику и архивному почтовому ящику. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

