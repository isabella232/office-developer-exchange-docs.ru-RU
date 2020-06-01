---
title: тимезонедефинитион
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
description: Элемент Тимезонедефинитион указывает точки и переходы, определяющие часовой пояс.
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466068"
---
# <a name="timezonedefinition"></a>тимезонедефинитион

Элемент **тимезонедефинитион** указывает точки и переходы, определяющие часовой пояс. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **тимезонедефинитионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Представляет уникальный идентификатор часового пояса.  <br/> |
|Имя  <br/> |Представляет описательное имя часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.  <br/> |
|[транситионсграупс](transitionsgroups.md) <br/> |Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.  <br/> |
|[Выполняет](transitions.md) <br/> |Представляет массив переходов часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[тимезонедефинитионс](timezonedefinitions.md) <br/> |Представляет массив определений часовых поясов.  <br/> |
|[тимезонеконтекст](timezonecontext.md) <br/> |Представляет определение часового пояса по умолчанию, которое будет использоваться для определения свойств DateTime объектов, которые создаются, обновляются и извлекаются с помощью веб-служб Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

