---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Стандартный элемент представляет дату и время изменения времени с летнего времени на стандартное время.
ms.openlocfilehash: c121e959f243d982cfe50ed6b4ef39a82dae2cc8
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353436"
---
# <a name="standard"></a>Standard

**Стандартный** элемент представляет дату и время изменения времени с летнего времени на стандартное время. 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

**TimeChangeType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**TimeZoneName** <br/> |Описывает имя часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Смещение](offset.md) <br/> |Описание смещения от [BaseOffset](baseoffset.md). Вместе с **BaseOffset** элемент элемент **смещение** определяет, является ли время стандартное время или летнее время.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительное ежегодно повторяющейся для даты перехода часового пояса.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Представляет дату, когда время изменяется с стандартное или летнее время.  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |Описание момента изменения времени между зимнего и летнего времени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Представляет часовой пояс расположение, где размещен собрания.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

