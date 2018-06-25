---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: Элемент PercentComplete описывает состояние завершения задачи.
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834717"
---
# <a name="percentcomplete"></a>PercentComplete

Элемент **PercentComplete** описывает состояние завершения задачи. 
  
```xml
<PercentComplete/>
```

 **Двойная**
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

Текстовое значение, которое представляет собой целое число между 0 и 100 является обязательным.
  
## <a name="remarks"></a>Замечания

Установка **PercentComplete** 100 имеет тот же эффект, как установка элемент [CompleteDate](completedate.md) или установка элемент [состояние](status.md) значение **завершено**. В запросе, что наборов по крайней мере два из этих свойств, последнего обработанного свойство определяет значение, заданное для этих элементов. К примеру Если **PercentComplete** равно 100, [CompleteDate](completedate.md) — 1 января 2007 г и имеет [состояние](status.md) NotStarted и свойства, передаваемых в следующем порядке, влияние будет присвоено [состояние](status.md) задачи NotStarted, [ CompleteDate](completedate.md) **значение null**, а **PercentComplete** 0. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание задач](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Удаление задачи](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

