---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: Элемент HasEndTimeChanged определяет, изменился ли время окончания собрания.
ms.openlocfilehash: 046bb302d6f7052c6f1757ce393583b305311e2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833805"
---
# <a name="hasendtimechanged"></a>HasEndTimeChanged

Элемент **HasEndTimeChanged** определяет, изменился ли время окончания собрания. 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
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
|[ChangeHighlights](changehighlights.md) <br/> |Указывает, что был изменен между двумя версиями собрания сообщение запроса.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **HasEndTimeChanged** указывает, что изменилось время окончания собрания. Значение **false** указывает, что время окончания собрания не был изменен. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
