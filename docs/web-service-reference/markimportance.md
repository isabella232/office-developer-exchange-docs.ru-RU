---
title: MarkImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkImportance
api_type:
- schema
ms.assetid: 32b8b08f-65e9-4764-b40a-63245551f4a3
description: Элемент MarkImportance указывает важность, ставится отметка в сообщениях.
ms.openlocfilehash: 32b1fa63ef47327e7d3af717ed9f452e43b16380
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834356"
---
# <a name="markimportance"></a>MarkImportance

Элемент **MarkImportance** указывает важность, ставится отметка в сообщениях. 
  
```XML
<MarkImportance/>
```

 **ImportanceChoicesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Действия](actions.md) <br/> |Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для этого элемента есть только одно из следующих значений string:
  
- Low
    
- Обычный
    
- High
    
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

