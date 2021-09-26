---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: Элемент RecurringDayTransition представляет переход часовой пояс, который происходит в один день каждый год.
ms.openlocfilehash: 3b567e5b906ec00bd71deb1c85f8049bb6de8e3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542885"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

Элемент **RecurringDayTransition** представляет переход часовой пояс, который происходит в один день каждый год. 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 **RecurringDayTransitionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[To](to.md) <br/> |Указывает период [или](period.md) [TransitionsGroup,](transitionsgroup.md) которые должны быть объектом перехода часового пояса.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Представляет смещение длительности от согласованного универсального времени (UTC) для перехода часового пояса.  <br/> |
|[Month (смена часовых поясов)](month-time-zone-transition.md) <br/> |Представляет месяц, в котором происходит переход часового пояса.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Представляет день недели, в который происходит переход часового пояса.  <br/> |
|[Occurrence (смена часовых поясов)](occurrence-time-zone-transition.md) <br/> |Представляет возникновение дня недели в месяце, когда происходит переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
   
## <a name="remarks"></a>Заметки

Примером перехода часового пояса, который может быть представлен элементом [RecurringDayTransition,](recurringdaytransition.md) является переход, который происходит во второй вторник февраля каждого года. 
  
Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

