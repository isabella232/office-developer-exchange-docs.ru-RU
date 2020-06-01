---
title: Подорганизатор
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: Элемент, который указывает, является ли этот пользователь организатором собрания.
ms.openlocfilehash: 45b7a66068dc00f6e60b7380240bea6836282fd4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466565"
---
# <a name="isorganizer"></a>Подорганизатор

Элемент **, который указывает** , является ли этот пользователь организатором собрания. 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для **элемента "," указывает** на то, что пользователь создал элемент календаря или сообщение о собрании. Значение **false** указывает, что элемент календаря или сообщение о собрании не были созданы БВ пользователем. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

