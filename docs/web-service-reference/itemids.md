---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: Элемент ItemIds содержит уникальные удостоверения элементов, элементов возникновения и повторяющихся основных элементов, которые используются для удаления, отправки, получения, перемещения или копирования элементов в Exchange магазине.
ms.openlocfilehash: 7341b8214b4d61564bd87707a9d8c76fbca07628
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522889"
---
# <a name="itemids"></a>ItemIds
  
Элемент **ItemIds** содержит уникальные удостоверения элементов, элементов возникновения и повторяющихся основных элементов, которые используются для удаления, отправки, получения, перемещения или копирования элементов в Exchange магазине.
  
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
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Определяет одно возникновение повторяющегося элемента.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Определяет мастер-элемент повторения, определяя идентификаторы одного из связанных с ним элементов возникновения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Определяет запрос на удаление элементов в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Корневой элемент, который определяет запрос на отправку элементов в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Определяет запрос на получения элементов из Exchange магазина.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элементов в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элементов в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteItem](deleteitem-operation.md)
- [Операция SendItem](senditem-operation.md) 
- [Операция GetItem](getitem-operation.md)
- [Операция MoveItem](moveitem-operation.md)
- [Операция CopyItem](copyitem-operation.md)
- [Операция FindConversation](findconversation-operation.md)

