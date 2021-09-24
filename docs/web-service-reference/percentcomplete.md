---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: Элемент PercentComplete описывает состояние завершения задачи.
ms.openlocfilehash: 48e6163377d51d64f63e966c525def48f930733e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519249"
---
# <a name="percentcomplete"></a>PercentComplete

Элемент **PercentComplete** описывает состояние завершения задачи. 
  
```xml
<PercentComplete/>
```

 **двойной**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение, представляю которое представляет ряд от 0 до 100.
  
## <a name="remarks"></a>Заметки

Параметр **PercentComplete** до 100 имеет тот же эффект, что и настройка элемента [CompleteDate](completedate.md) или настройка элемента [Status](status.md) для **завершения**. В запросе, который задает по крайней мере два из этих свойств, последнее обработанное свойство определяет значение, запредельное для этих элементов. Например, если **PercentComplete** 100, [CompleteDate](completedate.md) — 1 января 2007 г., а состояние нестареется, а свойства будут [](status.md) передаваться в этом порядке, то будет установлен статус задачи notStarted, [CompleteDate](completedate.md) — **null** и **PercentComplete** — 0. [](status.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание задач](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Удаление задач](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

