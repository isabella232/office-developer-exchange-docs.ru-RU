---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: Элемент EndDateTime указывает Дата и время окончания для правила или поиска.
ms.openlocfilehash: ad596c6441e7bdb10b4e886a8d0f3ba183c43c3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762351"
---
# <a name="enddatetime"></a>EndDateTime

Элемент **EndDateTime** указывает Дата и время окончания для правила или поиска. 
  
```XML
<EndDateTime/>
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
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Содержит критерии для типов сообщений для поиска.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее даты/времени является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

