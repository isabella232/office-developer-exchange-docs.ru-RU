---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: Элемент SortBy содержит свойство Item, используемое для сортировки результатов поиска.
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835518"
---
# <a name="sortby"></a>SortBy

Элемент **SortBy** содержит свойство Item, используемое для сортировки результатов поиска. 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **фиелдордертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Порядок  <br/> |Текстовое значение атрибута **Order** — это порядок сортировки. Текстовое значение по **возрастанию** указывает на то, что результаты представлены в возрастающем порядке. Текстовое значение "по **убыванию** " указывает на то, что результаты представлены в убывающем порядке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[Фиелдури](fielduri.md) | [индекседфиелдури](indexedfielduri.md)
  
### <a name="parent-elements"></a>Родительские элементы

[SearchMailboxes](searchmailboxes.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

