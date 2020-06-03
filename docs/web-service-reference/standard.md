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
description: Стандартный элемент представляет дату и время изменения времени с летнего на стандартное время.
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467566"
---
# <a name="standard"></a>Standard

**Стандартный** элемент представляет дату и время изменения времени с летнего на стандартное время. 
  
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

**тимечанжетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**тимезоненаме** <br/> |Описывает имя часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Offset](offset.md) <br/> |Описывает смещение от [басеоффсет](baseoffset.md). В сочетании с элементом **басеоффсет** элемент **offset** определяет, является ли время стандартным или летним.  <br/> |
|[релативэйеарлирекурренце](relativeyearlyrecurrence.md) <br/> |Описывает относительный ежегодный шаблон повторения для даты смены часового пояса.  <br/> |
|[абсолутедате](absolutedate.md) <br/> |Представляет дату, когда время изменяется со стандартного или летнего времени.  <br/> |
|[Время (Тимечанжетипе)](time-timechangetype.md) <br/> |Описывает время, по истечении которого время меняется со стандартного времени на летнее.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[митингтимезоне](meetingtimezone.md) <br/> |Представляет часовой пояс для расположения, в котором размещается собрание.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

