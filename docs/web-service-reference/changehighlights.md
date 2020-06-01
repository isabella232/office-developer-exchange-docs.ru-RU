---
title: чанжехигхлигхтс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: Элемент Чанжехигхлигхтс указывает, что изменилось между двумя версиями сообщения с приглашением на собрание.
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463281"
---
# <a name="changehighlights"></a>чанжехигхлигхтс

Элемент **чанжехигхлигхтс** указывает, что изменилось между двумя версиями сообщения с приглашением на собрание. 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 **чанжехигхлигхтстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[хаслокатиончанжед](haslocationchanged.md) <br/> |Указывает, изменилось ли свойство Location на собрании.  <br/> |
|[Location](location.md) <br/> |Представляет место собрания или встречи.  <br/> |
|[хасстарттимечанжед](hasstarttimechanged.md) <br/> |Указывает, изменилось ли время начала собрания.  <br/> |
|[Начало](start.md) <br/> |Представляет начало длительности.  <br/> |
|[хасендтимечанжед](hasendtimechanged.md) <br/> |Указывает, изменилось ли время окончания собрания.  <br/> |
|[Оканчиваться](end-ex15websvcsotherref.md) <br/> |Представляет конец длительности.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

