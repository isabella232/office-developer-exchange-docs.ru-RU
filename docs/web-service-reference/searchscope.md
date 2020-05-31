---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: Элемент SearchScope указывает область поиска.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835315"
---
# <a name="searchscope"></a>SearchScope

Элемент **SearchScope** указывает область поиска. 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **маилбокссеарчлокатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[маилбокссеарчскопе](mailboxsearchscope.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SearchScope** указывает тип почтового ящика, в котором выполняется поиск поиска обнаружения. Текстовое значение **PrimaryOnly** указывает на то, что выполняется поиск основного почтового ящика. Текстовое значение **ArchiveOnly** указывает на то, что выполняется поиск архивного почтового ящика. Текстовое значение **ALL** означает, что поиск выполняется как в основном, так и в архивных почтовых ящиках. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

