---
title: Начало
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: Элемент Start представляет начало продолжительности.
ms.openlocfilehash: 7342e285e57a165ec4a9ba0b8551bfbe045d3b9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521272"
---
# <a name="start"></a>Начало

Элемент **Start** представляет начало продолжительности. 
  
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
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Представляет удаленный случай повторяющегося элемента календаря.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первое появление повторяющегося элемента календаря.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнее появление повторяющегося элемента календаря.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Occurrence](occurrence.md) <br/> |Представляет одно измененное возникновение повторяющегося элемента календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет начало продолжительности.
  
## <a name="remarks"></a>Заметки

Операция UpdateItem может установить [](end-ex15websvcsotherref.md) время [начала](start.md) и окончания элемента магазина Exchange. В запросе UpdateItem **можно** установить время запуска без установки **конечного** времени. Это может привести к ошибке, **если** время начала более позднее, чем **время окончания.** Чтобы сохранить продолжительность, клиентские  приложения должны  выполнять корректировки в конечный период времени при смене времени начала. 
  
> [!NOTE]
> Сведения о смещении часового [](end-ex15websvcsotherref.md) пояса теряются, если даты начала и окончания повторяющегося элемента не имеют даты, равной первому появлению еженедельного шаблона повторения. [](start.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

