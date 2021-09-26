---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: Элемент SortOrder указывает порядок сортировки, используемый в результате запроса GetConversationItems.
ms.openlocfilehash: 0091968f1359b0cf744525139b5c6a8cf1687d81
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544677"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

Элемент **SortOrder** указывает порядок сортировки, используемый в результате запроса **GetConversationItems.** 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SortOrder** — это порядок, в котором упорядочены беседы. Текстовое значение **TreeOrderAscending** указывает, что беседы заказываться в соответствии с деревом беседы в порядке восходящей. Текстовое значение **TreeOrderDescending** указывает, что беседы заказываться в соответствии с деревом беседы в порядке убывания. Текстовое значение **DateOrderAscending** указывает, что беседы заказываться в соответствии с датой беседы в порядке восходящей. Текстовое значение **DateOrderDescending** указывает, что беседы заказываться в соответствии с датой беседы в порядке убывания. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

