---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: Элемент IncludeNonIndexableItems содержит логическое значение, которое указывает, следует ли включать элементы, которые не могут быть индексированы.
ms.openlocfilehash: ae91a3c6db82aea1d45940603d0ff2064d29f43f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833904"
---
# <a name="includenonindexableitems"></a>IncludeNonIndexableItems

Элемент **IncludeNonIndexableItems** содержит **логическое** значение, которое указывает, следует ли включать элементы, которые не могут быть индексированы. 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **IncludeNonIndexableItems** указывает, что элементы, которые не могут быть индексированы включены в почтовый ящик удержаний. Значение **false** указывает, что элементы, которые не могут быть индексированы не включаются в почтовый ящик удержаний. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   
