---
title: Определение часового пояса
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: Элемент определение часового пояса указывает периодов и переходы, определяющие часового пояса.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840200"
---
# <a name="timezonedefinition"></a>Определение часового пояса

Элемент **Определение часового пояса** указывает периодов и переходы, определяющие часового пояса. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Представляет уникальный идентификатор часового пояса.  <br/> |
|Имя  <br/> |Представляет описательное имя часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Периоды](periods.md) <br/> |Представляет массив элементов [периода времени](period.md) , которые определяют смещение времени на различных этапах часового пояса.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Представляет массив [TransitionsGroup](transitionsgroup.md) элементов, которые задают переходы часового пояса.  <br/> |
|[Переходы между](transitions.md) <br/> |Представляет массив переходы часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Представляет собой массив из определения часового пояса.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Представляет определение часового пояса по умолчанию, который будет использоваться для областей свойства даты и времени объектов, которые создаются, обновить и получить с помощью веб-служб Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

