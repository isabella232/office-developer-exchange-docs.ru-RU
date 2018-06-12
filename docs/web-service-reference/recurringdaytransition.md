---
title: RecurringDayTransition
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
description: Элемент RecurringDayTransition представляет переход часового пояса, что происходит в тот же день каждый год.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835012"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

Элемент **RecurringDayTransition** представляет переход часового пояса, что происходит в тот же день каждый год. 
  
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
|[Задача](to.md) <br/> |Задает [период](period.md) или [TransitionsGroup](transitionsgroup.md) , который является целевым для перехода часового пояса.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Представляет смещение продолжительность в формате UTC для перехода часового пояса.  <br/> |
|[Месяц (часовой пояс переходов)](month-time-zone-transition.md) <br/> |Представляет месяц, в котором осуществляется часового пояса.  <br/> |
|[DayOfWeek (часовой пояс)](dayofweek-timezone.md) <br/> |Представляет день недели, на котором происходит переход часового пояса.  <br/> |
|[Вхождение (часовой пояс переходов)](occurrence-time-zone-transition.md) <br/> |Представляет экземпляр день недели, месяца, которая происходит переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Переходы между](transitions.md) <br/> |Представляет коллекцию переходы часового пояса.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Представляет коллекцию переходы часового пояса.  <br/> |
   
## <a name="remarks"></a>Замечания

Пример перехода часовой пояс, который может быть представлен элемент [RecurringDayTransition](recurringdaytransition.md) является переход, возникает во второй вторник февраля каждый год. 
  
Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
