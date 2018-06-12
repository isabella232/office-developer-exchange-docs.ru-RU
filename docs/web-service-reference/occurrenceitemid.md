---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: Элемент OccurrenceItemId определяет одно вхождение повторяющегося элемента.
ms.openlocfilehash: e3d7b6efc49775f54219ce0dc0ec39a34a95f8fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834639"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

Элемент **OccurrenceItemId** определяет одно вхождение повторяющегося элемента. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Определяет повторяющиеся главных повторяющегося элемента. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Идентифицирует определенной версии образца повторения или вхождения элемента. Если изменить хозяином повторяющиеся или любой из его вхождения, изменяется **ChangeKey** . **ChangeKey** подходит и для повторяющихся master и все вхождения.  <br/> |
|**InstanceIndex** <br/> |Определяет индекс экземпляра элемента. Этот атрибут является обязательным. Это значение представляет собой целое число.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
|[Что ItemID](itemids.md) <br/> | Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange. <br/><br/>Ниже приведены выражения XPath для этого элемента. <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**Примечание**: [операция MoveItem](moveitem-operation.md) и [операции CopyItem](copyitem-operation.md) возможен только с элементами одного календаря и повторяющиеся основные элементы. Недопустимые вхождения элемента с помощью этих операций.           |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления для применения к элементу.<br/><br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

Следующий пример определяет четвертый вхождение повторяющегося элемента, который имеет 34vswe4 удостоверений.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [RecurringMasterItemId](recurringmasteritemid.md)
- [FindConversation Operation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

