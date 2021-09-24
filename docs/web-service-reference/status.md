---
title: Статус
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: Элемент Status представляет состояние элемента задачи.
ms.openlocfilehash: 5ec50e3f0c06ad3ec8301ddbe8e7bd249b1e8fe9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525542"
---
# <a name="status"></a>Статус

Элемент **Status** представляет состояние элемента задачи. 
  
```xml
<Status/>
```

 **TaskStatusType**
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

Требуется текстовое значение. Возможные текстовые значения для этого элемента:
  
- NotStarted
    
- InProgress
    
- Завершено
    
- WaitingOnOthers
    
- Отложенный
    
## <a name="remarks"></a>Заметки

Параметр [CompleteDate имеет](completedate.md) тот же эффект, что и параметр [PercentComplete](percentcomplete.md) до 100 или **Состояние** **завершено.** В запросе, который задает по крайней мере два из этих свойств, последнее обработанное свойство определяет значение, запредельное для этих элементов. Например, если **PercentComplete** 100, **CompleteDate** — это 1/1/2007, а состояние нестареется, а свойства будут передаваться  в этом порядке, эффект будет в том, чтобы установить состояние задачи для NotStarted, **CompleteDate** до **null** и **PercentComplete** до 0.  
  
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

