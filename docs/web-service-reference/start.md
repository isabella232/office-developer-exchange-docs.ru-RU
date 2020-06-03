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
ms.openlocfilehash: 0daf9c1422f7ba3894f9785aacac58263c5e721e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457216"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [виклирекурренце](weeklyrecurrence.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

