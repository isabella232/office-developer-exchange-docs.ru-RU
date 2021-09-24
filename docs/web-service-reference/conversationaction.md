---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: Элемент ConversationAction содержит одно действие, которое необходимо применить к одному диалогу.
ms.openlocfilehash: 04af68b4ad8442160792fd3aa9f3259058a0f3a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531108"
---
# <a name="conversationaction"></a>ConversationAction

Элемент **ConversationAction** содержит одно действие, которое необходимо применить к одному диалогу. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 **ConversationActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Action (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Содержит действие для выполнения в беседе, указанной элементом [ConversationId.](conversationid.md) Этот элемент должен присутствовать.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор беседы, который будет иметь действие, указанное элементом [Action (ConversationActionType),](action-conversationactiontypetype.md) примененным к элементам в беседе. Этот элемент должен присутствовать.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, которая ориентирована на действия, которые используют папки. Этот элемент должен присутствовать при копировании, удалении, перемещении и настройке состояния чтения в элементах беседы в целевой папке.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Содержит дату и время последней синхронизации беседы. Этот элемент должен присутствовать при попытке удалить все элементы в разговоре, который был получен до указанного времени.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Указывает, отправляется ли ответ сразу после начала обработки действия на сервере или после завершения действия. Этот элемент должен присутствовать для асинхронного ответа на запрошенное действие.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Указывает папку назначения для копирования и перемещения действий.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, определяя категории, к которым относятся элементы в беседе.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Указывает флаг, который позволяет удалять все новые элементы в беседе.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли прочитано сообщение.  <br/> |
|[DeleteType](deletetype.md) <br/> |Указывает, как удаляются элементы в беседе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Содержит коллекцию бесед и действий, которые необходимо применить к ним.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**Текстовые значения элемента ConversationAction**

|**Значение**|**Описание**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Всегда классифицировать беседу.  <br/> |
|AlwaysDelete  <br/> |Всегда удаляйте беседу.  <br/> |
|AlwaysMove  <br/> |Всегда перемещай беседу.  <br/> |
|Удалить  <br/> |Удаление беседы.  <br/> |
|Move  <br/> |Перемещение беседы.  <br/> |
|Copy  <br/> |Скопируйте беседу.  <br/> |
|SetReadState  <br/> |Установите состояние чтения беседы.  <br/> |
|SetRetentionPolicy  <br/> |Установите политику хранения для беседы.  <br/> |
   
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



[Операция ApplyConversationAction](applyconversationaction-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

