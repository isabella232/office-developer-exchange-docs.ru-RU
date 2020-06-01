---
title: рекуррингдайтранситион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: Элемент Рекуррингдайтранситион представляет переход часового пояса, который выполняется в один день каждого года.
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468469"
---
# <a name="recurringdaytransition"></a>рекуррингдайтранситион

Элемент **рекуррингдайтранситион** представляет переход часового пояса, который выполняется в один день каждого года. 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 **рекуррингдайтранситионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[To](to.md) <br/> |Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.  <br/> |
|[тимеоффсет](timeoffset.md) <br/> |Представляет смещение длительности от времени в формате UTC для смены часового пояса.  <br/> |
|[Month (переход часового пояса)](month-time-zone-transition.md) <br/> |Представляет месяц, в который происходит переход часового пояса.  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |Представляет день недели, в который происходит переход часового пояса.  <br/> |
|[Вхождение (переход часового пояса)](occurrence-time-zone-transition.md) <br/> |Представляет число дней недели в месяце, в котором происходит переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Выполняет](transitions.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
|[транситионсграуп](transitionsgroup.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
   
## <a name="remarks"></a>Примечания

Примером перехода по часовым поясам, которые могут быть представлены элементом [рекуррингдайтранситион](recurringdaytransition.md) , является переход, который выполняется на второй вторник февраля каждого года. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

