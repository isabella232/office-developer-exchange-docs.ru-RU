---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: Элемент OccurrenceItemId определяет одно возникновение повторяющегося элемента.
ms.openlocfilehash: ac6fc081e67f3897880ad30fcc1b62fe2e844459
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515420"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

Элемент **OccurrenceItemId** определяет одно возникновение повторяющегося элемента. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**RecurringMasterId** <br/> |Определяет повторяющийся мастер повторяющегося элемента. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Определяет определенную версию повторяющегося мастера или возникновения элемента. Если изменяется либо повторяющийся мастер, либо любое из его появлений, **изменяется ChangeKey.** **ChangeKey является** одинаковым для повторяющегося мастера и всех случаев.  <br/> |
|**InstanceIndex** <br/> |Определяет индекс возникновения элемента. Этот атрибут является обязательным. Это значение представляет собой integer.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
|[ItemIds](itemids.md) <br/> | Содержит уникальные удостоверения элементов, элементов возникновения и повторяющихся элементов, используемых для удаления, отправки, получения, перемещения или копирования элементов в Exchange магазине. <br/><br/>Ниже приводится выражение XPath к этому элементу: <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**ПРИМЕЧАНИЕ.** [Операция MoveItem и](moveitem-operation.md) [операция CopyItem](copyitem-operation.md) работают только с одними элементами календаря и повторяющимися мастер-элементами. В этих операциях недействительны вхождения элементов.           |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления, которые необходимо применить к элементу.<br/><br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере определяется четвертое появление повторяющегося элемента с удостоверением 34vswe4.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [RecurringMasterItemId](recurringmasteritemid.md)
- [Операция FindConversation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

