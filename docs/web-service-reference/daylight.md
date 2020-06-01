---
title: Переход
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: Элемент "лето" представляет дату и время изменения времени со стандартного времени на летнее.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457461"
---
# <a name="daylight"></a>Переход

Элемент " **лето** " представляет дату и время изменения времени со стандартного времени на летнее. 
  
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
|[Offset](offset.md) <br/> |Описывает смещение от [басеоффсет](baseoffset.md). Основное смещение в дополнение к этому смещению определяет время в зависимости от того, является ли оно стандартным или летним.  <br/> |
|[релативэйеарлирекурренце](relativeyearlyrecurrence.md) <br/> |Описывает относительный ежегодный шаблон повторения для шаблона даты перехода часового пояса.  <br/> |
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

