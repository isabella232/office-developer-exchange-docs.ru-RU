---
title: Год
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: Элемент Year используется для определения часового пояса, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: cc83f9b2137f151f3f8ef0ceaf603ec036989961
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465172"
---
# <a name="year"></a>Год

Элемент **year** используется для определения часового пояса, который изменяется в зависимости от года. Этот элемент является необязательным. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<Year/>
```

**строка**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> |Представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (UTC)](bias-utc.md) .  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (UTC](bias-utc.md) ) в регионах, где наблюдается летнее время.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент year принимает строку, представляющую год. Год имеет формат гггг.
  
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

