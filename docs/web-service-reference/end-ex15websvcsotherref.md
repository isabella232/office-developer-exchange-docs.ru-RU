---
title: End
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: Последний элемент представляет конец длительность.
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762342"
---
# <a name="end"></a>End

**Последний** элемент представляет конец длительность. 
  
```xml
<End/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первого появления повторяющегося элемента календаря.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнего вхождения повторяющегося элемента календаря.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Вхождение](occurrence.md) <br/> |Представляет измененной вхождения повторяющегося элемента календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет конец длительность.
  
## <a name="remarks"></a>Замечания

Операция UpdateItem можно задать время [Start](start.md) и **End** объекта хранилища Exchange. В запросе UpdateItem можно задать время [начала](start.md) без предоставления время **окончания** . Это может вызвать ошибку, если время [начала](start.md) позднее время **окончания** . Обратите внимание, что клиентские приложения должны выполнить настройку время **окончания** , изменения, время [начала](start.md) для сохранения во время выполнения. 
  
 **Примечание** [Запуск](start.md) и **конечной** дат повторяющегося элемента шаблона, у которых дата, равный первого появления еженедельно повторяющейся информации смещение часового пояса будут потеряны. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[WeeklyRecurrence](weeklyrecurrence.md)
  
 **End**


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

