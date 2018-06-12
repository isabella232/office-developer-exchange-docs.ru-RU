---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: Элемент CompleteDate представляет дату, на котором был выполнен элемента.
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761693"
---
# <a name="completedate"></a>CompleteDate

Элемент **CompleteDate** представляет дату, на котором был выполнен элемента. 
  
```xml
<CompleteDate/>
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
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[Флаг](flag.md) <br/> |Задает флаг для элемента почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, которое представляет дату и время является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Установка **CompleteDate** имеет тот же эффект, что и установка [PercentComplete](percentcomplete.md) [состояние](status.md) значение **завершено**или 100. В запросе, что наборов по крайней мере два из этих свойств, последнего обработанного свойство определяет значение, заданное для этих элементов. Например [PercentComplete](percentcomplete.md) равно 100, **CompleteDate** — 1 января 2007 г и имеет [состояние](status.md) **NotStarted**и свойства, передаваемых в указанном порядке, влияние нужно задать [состояние](status.md) задачи для **NotStarted **, [CompleteDate](completedate.md) **значение null**, а [PercentComplete](percentcomplete.md) 0. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
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

