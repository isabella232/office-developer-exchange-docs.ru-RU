---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: Элемент ItemChange содержит идентификатор элемента и обновления, чтобы применить к элементу.
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834145"
---
# <a name="itemchange"></a>ItemChange

Элемент **ItemChange** содержит идентификатор элемента и обновления, чтобы применить к элементу. 
  
[UpdateItem](updateitem.md)
  
[ItemChanges](itemchanges.md)
  
[ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
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
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange. Этот элемент является обязательным, если элемент [OccurrenceItemId](occurrenceitemid.md) или [RecurringMasterItemId](recurringmasteritemid.md) не используется.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Определяет одно вхождение повторяющегося элемента. Этот элемент является обязательным, если используется. Этот элемент является обязательным, если элемент [RecurringMasterItemId](recurringmasteritemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Идентифицирует элемент шаблона повторения, указав один из его появления связанные элементы идентификаторов. Этот элемент является обязательным, если используется. Этот элемент является обязательным, если элемент [OccurrenceItemId](occurrenceitemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[Обновления (элемент)](updates-item.md) <br/> |Содержит массив, определяющий добавьте, Установка и удаление изменения свойств элемента. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |Содержит массив элементов [ItemChange](itemchange.md) , чтобы указать элементы и обновления, чтобы применить к элементам.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Замечания

Можно использовать только один элемент [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md)или [RecurringMasterItemId](recurringmasteritemid.md) в элементе **ItemChange** . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateItem Operation](updateitem-operation.md)

