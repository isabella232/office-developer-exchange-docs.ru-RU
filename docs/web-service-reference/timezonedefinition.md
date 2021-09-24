---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: Элемент TimeZoneDefinition указывает периоды и переходы, определяющие часовой пояс.
ms.openlocfilehash: 6f2b580d2c3e31826ca74034cfda938cff71ee53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538816"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

Элемент **TimeZoneDefinition** указывает периоды и переходы, определяющие часовой пояс. 
  
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
|[Periods](periods.md) <br/> |Представляет массив элементов [Period,](period.md) определяющие смещение времени на разных этапах часового пояса.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Представляет массив элементов [TransitionsGroup,](transitionsgroup.md) которые указывают переходы часового пояса.  <br/> |
|[Transitions](transitions.md) <br/> |Представляет массив переходов часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Представляет массив определений часового пояса.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Представляет определение часового пояса по умолчанию, которое должно использоваться для скопить свойства DateTime объектов, которые создаются, обновляются и извлекаются с помощью Exchange веб-служб (EWS).  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

