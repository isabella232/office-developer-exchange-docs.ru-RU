---
title: итемидс
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
description: Элемент Итемидс содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834155"
---
# <a name="itemids"></a>итемидс
  
Элемент **итемидс** содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**нонемптяррайофбасеитемидстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы. 
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.  <br/> |
|[оккурренцеитемид](occurrenceitemid.md) <br/> |Определяет один экземпляр повторяющегося элемента.  <br/> |
|[рекуррингмастеритемид](recurringmasteritemid.md) <br/> |Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Определяет запрос на удаление элементов в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Корневой элемент, определяющий запрос на отправку элементов в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Определяет запрос на получение элементов из хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элементов в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элементов в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CopyItem` <br/> |
   
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

- [Операция DeleteItem](deleteitem-operation.md)
- [Операция SendItem](senditem-operation.md) 
- [Операция GetItem](getitem-operation.md)
- [Операция MoveItem](moveitem-operation.md)
- [Операция CopyItem](copyitem-operation.md)
- [Операция FindConversation](findconversation-operation.md)

