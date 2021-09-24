---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: Элемент IncludeNonIndexableItems содержит значение Boolean, указывав, следует ли включать элементы, которые нельзя индексировать.
ms.openlocfilehash: 33ff8c59c3ef1d9a91f87870e0a876c5a39ce795
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514601"
---
# <a name="includenonindexableitems"></a>IncludeNonIndexableItems

Элемент **IncludeNonIndexableItems** содержит значение **Boolean,** указывав, следует ли включать элементы, которые нельзя индексировать. 
  
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

Текстовое значение **true** для элемента **IncludeNonIndexableItems** указывает на то, что элементы, которые нельзя индексировать, включаются в личные почтовые ящики. Значение false **указывает,** что элементы, которые нельзя индексировать, не включаются в почтовые ящики. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

