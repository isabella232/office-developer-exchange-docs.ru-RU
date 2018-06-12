---
title: Начало
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: Элемент Пуск представляет Пуск длительность.
ms.openlocfilehash: 8d013990e650b497abfa947938a69eed3fed7474
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835545"
---
# <a name="start"></a>Начало

Элемент **Начать** представляет Пуск длительность. 
  
```xml
<Start/>
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
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Представляет удаленных вхождение повторяющегося элемента календаря.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первого появления повторяющегося элемента календаря.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнего вхождения повторяющегося элемента календаря.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Вхождение](occurrence.md) <br/> |Представляет измененной вхождения повторяющегося элемента календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет начало длительность.
  
## <a name="remarks"></a>Замечания

Операция UpdateItem можно задать время [Start](start.md) и [End](end-ex15websvcsotherref.md) объекта хранилища Exchange. В запросе UpdateItem можно задать время **начала** без предоставления время **окончания** . Это может вызвать ошибку, если время **начала** позднее время **окончания** . Обратите внимание, что клиентские приложения должны выполнить настройку время **окончания** изменения, время **начала** для сохранения во время выполнения. 
  
> [!NOTE]
> [Запуск](start.md) и [конечной](end-ex15websvcsotherref.md) дат повторяющегося элемента шаблона, у которых дата, равный первого появления еженедельно повторяющейся информации смещение часового пояса будут потеряны. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

