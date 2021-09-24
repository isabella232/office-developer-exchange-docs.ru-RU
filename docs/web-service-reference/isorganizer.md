---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: Элемент IsOrganizer указывает значение Boolean, которое указывает, является ли этот человек организатором собрания.
ms.openlocfilehash: a60485146e333e69391dc1771b2c72ef25043a8b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518269"
---
# <a name="isorganizer"></a>IsOrganizer

Элемент **IsOrganizer** указывает значение Boolean, которое указывает, является ли этот человек организатором собрания. 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
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
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое **значение, истинное** для **элемента IsOrganizer,** указывает, что элемент календаря или сообщение собрания был создан пользователем. Значение false **указывает,** что элемент календаря или сообщение собрания не были созданы bv пользователем. 
  
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

