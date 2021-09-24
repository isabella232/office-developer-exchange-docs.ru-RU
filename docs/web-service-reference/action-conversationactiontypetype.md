---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Элемент Action содержит действие для выполнения беседы, указанной элементом ConversationId.
ms.openlocfilehash: e75d9d5df75894d1de9831b0022269e7ace4fa63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514895"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

Элемент **Action** содержит действие для выполнения беседы, указанной элементом [ConversationId.](conversationid.md) 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Action (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие, которое необходимо применить к одному разговору.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Action** указывает, какое действие будет выполняться во время беседы. Ниже следующую возможность текстовых значений и соответствующих действий: 
  
- **AlwaysCategorize** — текущие элементы и новые элементы в беседе будут автоматически задатки с категориями, которые определены в [элементе Categories.](categories-ex15websvcsotherref.md) 
    
- **AlwaysDelete** — текущие элементы и новые элементы в беседе будут автоматически удалены. Режим удаления устанавливается элементом [DeleteType.](deletetype.md) 
    
- **AlwaysMove** — текущие элементы и новые элементы в беседе будут автоматически перемещены в папку, идентифицированную [элементом DestinationFolderId.](destinationfolderid.md) 
    
- **Удаление** . Текущие элементы в беседе будут удалены. Последующие элементы в беседе не будут удалены. Режим удаления устанавливается элементом [DeleteType.](deletetype.md) 
    
- **Move** . Текущие элементы в беседе будут перемещены в папку, идентифицированную [элементом DestinationFolderId.](destinationfolderid.md) Последующие элементы в беседе не будут перемещены. 
    
- **Скопируйте** . Текущие элементы в беседе будут скопированы в папку, идентифицированную элементом [DestinationFolderId.](destinationfolderid.md) Последующие элементы в беседе не будут скопированы. 
    
- **SetReadState** . Текущие элементы в беседе будут иметь набор состояния чтения. Состояние чтения устанавливается [элементом IsRead.](isread.md) 
    
- **Флаг** . Текущие элементы в беседе будут иметь набор флага, определенный [элементом Флаг.](flag.md) 
    
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

