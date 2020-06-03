---
title: сиктокондитионпажеитемвиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: Элемент Сиктокондитионпажеитемвиев определяет условие, которое используется для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и инструкций поиска для поиска FindItem или FindConversation.
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466838"
---
# <a name="seektoconditionpageitemview"></a>сиктокондитионпажеитемвиев

Элемент **сиктокондитионпажеитемвиев** определяет условие, которое используется для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и инструкций поиска для поиска **FindItem** или **FindConversation** . 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **сиктокондитионпажевиевтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|басепоинт  <br/> |Текстовое значение атрибута **басепоинт** — это базовая точка, с которой начнется поиск. Текстовое значение **start указывает на** то, что поиск начнется с начала набора результатов. Текстовое значение **End** указывает на то, что поиск начнется в конце набора результатов.  <br/> |
|максентриесретурнед  <br/> |Текстовое значение атрибута **максентриесретурнед** — максимальное количество элементов, которые могут быть возвращены в наборе результатов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[Condition (Рестриктионтипе)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindConversation](findconversation.md)  |  [FindItem](finditem.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

