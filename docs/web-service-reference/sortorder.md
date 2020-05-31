---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: Элемент SortOrder определяет порядок сортировки элементов в запросе FindItem или FindConversation.
ms.openlocfilehash: e20e5eab7972616c90079786abd78a0f7fedfebe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835519"
---
# <a name="sortorder"></a>SortOrder

Элемент **SortOrder** определяет порядок сортировки элементов в запросе **FindItem** или **FindConversation** . 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 **нонемптяррайоффиелдордерстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдордер](fieldorder.md) <br/> |Представляет одно поле для сортировки результатов и указывает направление сортировки. Можно включить один или несколько из этих элементов. Элементы [фиелдордер](fieldorder.md) применяются в порядке, указанном для сортировки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:`/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[Операция FindConversation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

