---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: Элемент SeekToConditionPageItemView определяет условие, используемое для определения конца поиска, начального индекса поиска, максимального возврата записей и направлений поиска для поиска FindItem или FindConversation.
ms.openlocfilehash: 6f4797a6b90456a50922db1c829757711816273e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546107"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

Элемент **SeekToConditionPageItemView** определяет условие, используемое для определения конца поиска, начального индекса поиска, максимального возврата записей и направлений поиска для поиска **FindItem** или **FindConversation.** 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|BasePoint  <br/> |Текстовое значение атрибута **BasePoint** — это базовая точка, с которой начнется поиск. Текстовое значение **Beginning** указывает, что поиск начнется в начале набора результатов. Текстовое значение **End** указывает, что поиск начнется в конце набора результатов.  <br/> |
|MaxEntriesReturned  <br/> |Текстовое значение **атрибута MaxEntriesReturned** — это максимальное количество элементов, которые могут быть возвращены в наборе результатов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[Condition (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindConversation](findconversation.md)  |  [FindItem](finditem.md)
  
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
   

