---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: Элемент IsWritable указывает, можно ли запись базовым контакт или получателя Active Directory для.
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834158"
---
# <a name="iswritable"></a>IsWritable

Элемент **IsWritable** указывает, можно ли запись базовым контакт или получателя Active Directory для. 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Атрибуты (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **IsWritable** указывает, что контакт или объект Active Directory для доступа на запись. Значение **false** указывает, что контакт или объект Active Directory недоступна для записи. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

