---
title: Bias (UTC)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bias
api_type:
- schema
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: Элемент Bias представляет общий смещение от скоординированного универсального времени (UTC). Это значение представлено в минутах.
ms.openlocfilehash: c7dc50d13eecab72d06927ce02762e57ec2f8a3e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543655"
---
# <a name="bias-utc"></a>Bias (UTC)

Элемент **Bias** представляет общий смещение от скоординированного универсального времени (UTC). Это значение представлено в минутах. 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZone (доступность)](timezone-availability.md) <br/> | Контейнер, который определяет сведения о дате запроса. Этот элемент содержит сведения о переходе между стандартным временем и летнее время.  <br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет собой integer.
  
## <a name="remarks"></a>Заметки

Второй элемент [Смещения](bias.md) в схеме представляет смещение от смещения координированное универсальное время (UTC). 
  
## <a name="example"></a>Пример

В следующем примере показана часть XML-запроса, который определяет смещение в 8 часов от UTC в клиентских приложениях.
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)  
- [Bias](bias.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

