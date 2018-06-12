---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: Что ItemID элемент содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834155"
---
# <a name="itemids"></a>ItemIds
  
**Что ItemID** элемент содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов. 
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Определяет одно вхождение повторяющегося элемента.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Идентифицирует элемент шаблона повторения, указав один из его появления связанные элементы идентификаторов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Определяет запрос на удаление элементов в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Корневой элемент, который определяет запрос на отправку элементов в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Определяет запрос на получение элементов из хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элементов в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос для копирования элементов в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteItem](deleteitem-operation.md)
- [SendItem Operation](senditem-operation.md) 
- [GetItem Operation](getitem-operation.md)
- [MoveItem Operation](moveitem-operation.md)
- [CopyItem Operation](copyitem-operation.md)
- [FindConversation Operation](findconversation-operation.md)

