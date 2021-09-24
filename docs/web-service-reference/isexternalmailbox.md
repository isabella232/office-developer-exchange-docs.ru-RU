---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: Элемент IsExternalMailbox указывает, является ли почтовый ящик внешним для организации.
ms.openlocfilehash: f2435356a7315c51f3d99aeedf0ae2b21500981c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524233"
---
# <a name="isexternalmailbox"></a>IsExternalMailbox

Элемент **IsExternalMailbox указывает,** является ли почтовый ящик внешним для организации. 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SearchableMailbox](searchablemailbox.md)
  
## <a name="text-value"></a>Текстовое значение

Значение текста, **истинное** для **элемента IsExternalMailbox,** указывает на то, что почтовый ящик находится во внешней организации. Значение false **указывает,** что почтовый ящик находится в организации. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

