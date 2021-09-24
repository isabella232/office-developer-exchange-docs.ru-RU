---
title: Daylight
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: Элемент Daylight представляет дату и время, когда время меняется от стандартного времени к летнему времени.
ms.openlocfilehash: 750d7cb97d9e2967d3477a93ae833229d20619dc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517219"
---
# <a name="daylight"></a>Daylight

Элемент **Daylight** представляет дату и время, когда время меняется от стандартного времени к летнему времени. 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
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
|[Offset](offset.md) <br/> |Описывает смещение [из BaseOffset](baseoffset.md). Базовый смещение в дополнение к этому смещению определяет время в зависимости от того, является ли это стандартным или летнее время.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительный шаблон повторяющихся периодов для шаблона даты перехода часовых поясов.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Представляет дату, когда время меняется от стандартного или летнего времени.  <br/> |
|[Time (TimeChangeType)](time-timechangetype.md) <br/> |Описывает время, когда время меняется между стандартным временем и летнее время.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Представляет часовой пояс расположения, где проходит собрание.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

