---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: Элемент IsHidden содержит значение Boolean, которое указывает, следует ли скрывать или отображаться в качестве элемента persona.
ms.openlocfilehash: 7ff24eaa5e8e7b25c87af0bf299fcca0d88dc0b6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532790"
---
# <a name="ishidden"></a>IsHidden

Элемент **IsHidden** содержит значение Boolean, которое указывает, следует ли скрывать или отображаться в качестве элемента persona. 
  
```XML
<IsHidden>true | false</IsHidden>
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
|[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |Указывает экземпляр в массиве атрибутов элемента **Persona.**  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текста,  истинное для **элемента IsHidden,** указывает на то, что указанный в нем контакт должен быть скрыт или отображаться в составе персоны. Значение false **указывает** на то, что указанный в нем контакт не должен скрываться или отображаться как часть персоны. 
  
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

