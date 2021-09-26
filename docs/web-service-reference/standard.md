---
title: Стандартный
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Элемент Standard представляет дату и время, когда время меняется с летнего времени на обычное.
ms.openlocfilehash: 8e44bc458f109975acd3d48c80726654b70373e8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544670"
---
# <a name="standard"></a>Стандартный

Элемент **Standard** представляет дату и время, когда время меняется с летнего времени на обычное. 
  
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
|[Offset](offset.md) <br/> |Описывает смещение [из BaseOffset](baseoffset.md). Вместе с **элементом BaseOffset** элемент **Offset** определяет, является ли время стандартным или летнее.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Описывает относительный год назад шаблон для даты перехода часовых поясов.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Представляет дату, когда время меняется от стандартного времени или летнего времени.  <br/> |
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

