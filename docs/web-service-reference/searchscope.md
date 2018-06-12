---
title: Область поиска
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: Элемент область поиска определяет область поиска.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835315"
---
# <a name="searchscope"></a>Область поиска

Элемент **область поиска** определяет область поиска. 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **MailboxSearchLocationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MailboxSearchScope](mailboxsearchscope.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **область поиска** указывает тип почтового ящика, поиск поиск обнаружения. Текстовое значение **PrimaryOnly** указывает, что выполняется поиск основного почтового ящика. Текстовое значение **ArchiveOnly** указывает, что выполняется поиск в архивный почтовый ящик. Текстовое значение **всех** указывает, что и первичной и поиск архивных почтовых ящиков. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

