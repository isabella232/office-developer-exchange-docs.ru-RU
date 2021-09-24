---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: Элемент MakeItemImmutable указывает значение Boolean, которое указывает, следует ли делать элемент только для чтения.
ms.openlocfilehash: 0e1d28f19492bb6dc013957aa5957b59e791b24b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524828"
---
# <a name="makeitemimmutable"></a>MakeItemImmutable

Элемент **MakeItemImmutable** указывает значение Boolean, которое указывает, следует ли делать элемент только для чтения. 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[UpdateItemInRecoverableItems](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a>Текстовое значение

Значение **текста, истинное** для **элемента MakeItemImmutable,** указывает на то, что элемент должен быть только для чтения. Значение false **указывает,** что элемент позволяет получить доступ к записи чтения. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

