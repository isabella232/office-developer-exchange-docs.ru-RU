---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: Элемент EndWallClock указывает время окончания собрания в часовом поясе расположения, в котором происходит собрания.
ms.openlocfilehash: 10e4a2bde50354b2f2752751c01a6a70aa084d05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762356"
---
# <a name="endwallclock"></a>EndWallClock

Элемент **EndWallClock** указывает время окончания собрания в часовом поясе расположения, в котором происходит собрания. 
  
```XML
<EndWallClock></EndWallClock>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Пользователь](persona.md) <br/> |Задает набор пользователя данные, возвращаемые запросом **GetPersona** .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **EndWallClock** — это строковое значение, задающее идентификатор часового пояса. 
  
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

