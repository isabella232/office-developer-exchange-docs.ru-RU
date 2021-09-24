---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: Элемент ItemChange содержит идентификатор элемента и обновления, которые необходимо применить к элементу.
ms.openlocfilehash: 8ace3cf78eb902e48529a0534e39ce7d584bd164
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537751"
---
# <a name="itemchange"></a>ItemChange

Элемент **ItemChange** содержит идентификатор элемента и обновления, которые необходимо применить к элементу. 
  
- [UpdateItem](updateitem.md) 
- [ItemChanges](itemchanges.md)
- [ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

**ItemChangeType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине. Этот элемент необходим, если элемент [OccurrenceItemId](occurrenceitemid.md) или [RecurringMasterItemId](recurringmasteritemid.md) не используется.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Определяет одно возникновение повторяющегося элемента. Этот элемент необходим, если используется. Этот элемент необходим, если элемент [RecurringMasterItemId](recurringmasteritemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Определяет мастер-элемент повторения, определяя идентификаторы одного из связанных с ним элементов возникновения. Этот элемент необходим, если используется. Этот элемент необходим, если элемент [OccurrenceItemId](occurrenceitemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[Updates (Item)](updates-item.md) <br/> |Содержит массив, который определяет приложения, набор и удаление изменений свойств элементов. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |Содержит массив элементов [ItemChange,](itemchange.md) определяющие элементы и обновления для применения к элементам.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Заметки

В элементе **ItemChange** можно использовать только один элемент [ItemId,](itemid.md) [OccurrenceItemId](occurrenceitemid.md)или [RecurringMasterItemId.](recurringmasteritemid.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateItem](updateitem-operation.md)

