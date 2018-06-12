---
title: Действие (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Элемент Action содержит действие, выполняемое в беседу, заданный элементом ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761323"
---
# <a name="action-conversationactiontypetype"></a>Действие (ConversationActionTypeType)

Элемент **Action** содержит действие, выполняемое в беседу, заданный элементом [ConversationId](conversationid.md) . 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Действие (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие должен применяться к разговора.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Действие** указывает действие, которое будет выполняться в беседе. Ниже приведены возможные текстовые значения и соответствующие действия. 
  
- **AlwaysCategorize** - текущих элементов и новых элементов в окне беседы будет автоматически с категориями, обнаруженных в элементе [категорий](categories-ex15websvcsotherref.md) . 
    
- Автоматически удалять **AlwaysDelete** - текущих элементов и новые элементы в беседе. Режим удаления задается с помощью элемента [DeleteType](deletetype.md) . 
    
- **AlwaysMove** - текущих элементов и новые элементы в беседе перемещается автоматически в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) . 
    
- **Удаление** - текущие элементы в окне беседы будет удалено. Последующие элементы в беседе, не удаляются. Режим удаления задается с помощью элемента [DeleteType](deletetype.md) . 
    
- **Перемещение** - текущего элементы в беседе будут перемещены в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) . Не будут перемещаться последующие элементы в беседе. 
    
- **Копия** - текущего элементы в беседе предстоит скопировать в папку, указанную в элементе [DestinationFolderId](destinationfolderid.md) . Последующие элементы в беседе, не копируются. 
    
- **SetReadState** - текущие элементы в окне беседы будут иметь их состояние чтения задать. Состояние чтения задано в элементе [IsRead](isread.md) . 
    
- **Флаг** - текущие элементы в окне беседы будут иметь флаг, определенный элемент [флаг](flag.md) . 
    
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

