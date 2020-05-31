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
description: Элемент Start представляет начало длительности.
ms.openlocfilehash: 8d013990e650b497abfa947938a69eed3fed7474
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835545"
---
# <a name="start"></a>Начало

Элемент **Start** представляет начало длительности. 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[делетедоккурренце](deletedoccurrence.md) <br/> |Представляет удаленное вхождение повторяющегося элемента календаря.  <br/> |
|[фирстоккурренце](firstoccurrence.md) <br/> |Представляет первое вхождение повторяющегося элемента календаря.  <br/> |
|[ластоккурренце](lastoccurrence.md) <br/> |Представляет последнее вхождение повторяющегося элемента календаря.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Экземпляр](occurrence.md) <br/> |Представляет один измененный экземпляр повторяющегося элемента календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет начало длительности.
  
## <a name="remarks"></a>Примечания

Для операции UpdateItem можно задать время [начала](start.md) и [окончания](end-ex15websvcsotherref.md) для элемента хранилища Exchange. В запросе UpdateItem время **начала** может быть задано без указания времени **окончания** . Это может привести к ошибке, если время **начала** позже времени **окончания** . Имейте в виду, что клиентские приложения должны выполнить корректировку до времени **окончания** при изменении времени **начала** , чтобы сохранить длительность. 
  
> [!NOTE]
> Сведения о смещении часового пояса теряются, если даты [начала](start.md) и [окончания](end-ex15websvcsotherref.md) повторяющегося элемента шаблона не имеют даты, равной первому появлению еженедельного расписания повторения. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [виклирекурренце](weeklyrecurrence.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

