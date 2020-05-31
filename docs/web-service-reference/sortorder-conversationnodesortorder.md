---
title: SortOrder (Конверсатионнодесортордер)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: Элемент SortOrder указывает порядок сортировки, используемый для результатов запроса GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835520"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (Конверсатионнодесортордер)

Элемент **SortOrder** указывает порядок сортировки, используемый для результатов запроса **GetConversationItems** . 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **конверсатионнодесортордер**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SortOrder** — это порядок, в котором упорядочиваются обсуждения. Текстовое значение **триордерасцендинг** указывает, что беседы упорядочиваются в соответствии с деревом бесед в возрастающем порядке. Текстовое значение **триордердесцендинг** указывает, что беседы упорядочиваются по дереву бесед в порядке убывания. Текстовое значение **датеордерасцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в возрастающем порядке. Текстовое значение **датеордердесцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в убывающем порядке. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

