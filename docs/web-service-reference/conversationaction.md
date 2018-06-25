---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: Элемент ConversationAction содержит одно действие должен применяться к разговора.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761811"
---
# <a name="conversationaction"></a>ConversationAction

Элемент **ConversationAction** содержит одно действие должен применяться к разговора. 
  
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
|[Действие (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Содержит действие, выполняемое в беседу, заданный элементом [ConversationId](conversationid.md) . Этот элемент должен быть указан.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор беседы, в которых будут действием, указанным с помощью элемента [действие (ConversationActionTypeType)](action-conversationactiontypetype.md) , применяется к элементам в беседе. Этот элемент должен быть указан.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, предназначенное для действий, использующих папок. Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Содержит дату и время последнего синхронизирована беседы. Этот элемент должен присутствовать при попытке удаления всех элементов в беседе, которые были получены до заданного времени.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Указывает, будет ли ответ сразу после начала действия обработки на сервере или ли ответ после завершения действия. Этот элемент необходим для ответа отправку асинхронных запрошенное действие.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Определяет папку назначения для копирования и перемещения действия.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, чтобы указать категории, к которым принадлежат элементы в беседе.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Задает флаг, который позволяет удалить для всех новых элементов в беседе.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, имеет ли чтение сообщения.  <br/> |
|[DeleteType](deletetype.md) <br/> |Показывает, как удалить элементы в беседе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Содержит коллекцию бесед и действий для применения к ним.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**ConversationAction элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Всегда классификации сообщений.  <br/> |
|AlwaysDelete  <br/> |Всегда удаляйте беседу.  <br/> |
|AlwaysMove  <br/> |Всегда перемещать беседу.  <br/> |
|Удаление  <br/> |Удалите беседу.  <br/> |
|перемещение.  <br/> |Перемещение беседу.  <br/> |
|Copy  <br/> |Скопируйте беседу.  <br/> |
|SetReadState  <br/> |Задайте состояние чтения беседы.  <br/> |
|SetRetentionPolicy  <br/> |Настройка политики хранения для беседы.  <br/> |
   
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



[Операция ApplyConversationAction](applyconversationaction-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

