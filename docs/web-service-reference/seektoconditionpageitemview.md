---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: Элемент SeekToConditionPageItemView определяет условие, используемое для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для поиска FindItem или FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835328"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

Элемент **SeekToConditionPageItemView** определяет условие, используемое для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для **FindItem** или **FindConversation **поиска. 
  
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
|Базисная точка  <br/> |Текстовое значение атрибута **Базисная точка** точка базовый, из которой будет начинаться поиск. Текстовое значение **начала** указывает, что поиск начнется в начале набора результатов. Текстовое значение **End** указывает, что поиск начинается в конце набора результатов.  <br/> |
|MaxEntriesReturned  <br/> |Текстовое значение атрибута **MaxEntriesReturned** — это максимальное число элементов, которые могут возвращаться в наборе результатов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[Условие (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindConversation](findconversation.md) | [FindItem](finditem.md)
  
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
   

