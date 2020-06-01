---
title: мержедфрибусинтервалинминутес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: Элемент Мержедфрибусинтервалинминутес представляет разницу во времени между двумя последовательными слотами в представлении Фрибусимержед.
ms.openlocfilehash: 6228ee5b66202634e6bb3b6c1ad6b8897a109d58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468791"
---
# <a name="mergedfreebusyintervalinminutes"></a>мержедфрибусинтервалинминутес

Элемент **мержедфрибусинтервалинминутес** представляет разницу во времени между двумя последовательными слотами в представлении **фрибусимержед** . 
  
[жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
[фрибусивиевоптионс](freebusyviewoptions.md)
  
[мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусивиевоптионс](freebusyviewoptions.md) <br/> |Указывает тип сведений о доступности, возвращаемых в ответе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение представляет время в минутах. Значение по умолчанию  30 минут. Шесть минут — это минимальный интервал и один день (1440 минут) — это максимальный интервал для этого элемента.
  
## <a name="remarks"></a>Примечания

Это значение используется только в том случае, если элемент [рекуестедвиев](requestedview.md) равен **мержедонли**, **фрибусимержед**или **детаиледмерже**. Это тип данных Integer. Поток, содержащий интервалы, заданные этим элементом, возвращается в элементе [мержедфрибуси](mergedfreebusy.md) . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[Операция GetUserOofSettings](getuseroofsettings-operation.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

