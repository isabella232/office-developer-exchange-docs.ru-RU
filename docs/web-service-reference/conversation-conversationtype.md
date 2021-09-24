---
title: Conversation (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: Элемент Conversation представляет собой один разговор.
ms.openlocfilehash: 7ce75fad17589f4d9a3ca52bcb2041eb1d1f4d2e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515959"
---
# <a name="conversation-conversationtype"></a>Conversation (ConversationType)

Элемент **Conversation** представляет собой один разговор. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversations](conversations-ex15websvcsotherref.md)
  
[Беседы (ConversationType)](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 **ConversationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет тему беседы. Этот элемент доступен только для чтения.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Содержит список получателей беседы, совокупный из определенной папки. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Содержит список получателей беседы, агрегированных в почтовом ящике. Этот элемент доступен только для чтения.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Содержит список всех людей, отправивших сообщения, которые в настоящее время нечитаются в этом разговоре в текущей папке. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Содержит список всех людей, которые отправили сообщения, которые в настоящее время нечитаются в этом разговоре во всех папках в почтовом ящике.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в текущей папке. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в почтовом ящике.  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |Содержит время доставки последнего сообщения, полученного в этом разговоре в текущей папке.  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |Содержит время доставки последнего сообщения, которое было получено в этом разговоре во всех папках в почтовом ящике.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, определяющая категории, которые применяются к всем предметам беседы в текущей папке.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Содержит список категорий для всех элементов беседы в почтовом ящике.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Содержит агрегированное состояние флага для элементов беседы в текущей папке.  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |Содержит агрегированное состояние флага для всех элементов беседы в почтовом ящике.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Содержит значение, которое указывает, имеет ли вложение по крайней мере один элемент беседы в текущей папке.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Содержит значение, которое указывает, имеет ли вложение по крайней мере один элемент беседы в почтовом ящике.  <br/> |
|[MessageCount](messagecount.md) <br/> |Содержит общее количество элементов беседы в текущей папке.  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |Содержит общее количество элементов беседы в почтовом ящике.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Содержит количество непрочитанные элементы беседы в папке.  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |Содержит количество всех непрочитанные элементы беседы в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Содержит размер беседы, рассчитанный из размера всех элементов беседы в текущей папке.  <br/> |
|[GlobalSize](globalsize.md) <br/> |Содержит размер беседы, вычисляемой из размера всех элементов беседы в почтовом ящике.  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов разговорных элементов в текущей папке.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов разговорных элементов в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Содержит совокупное значение для всех элементов беседы в текущей папке.  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |Содержит совокупное значение для всех элементов беседы в почтовом ящике.  <br/> |
|[ItemIds](itemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в текущей папке.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы](conversations-ex15websvcsotherref.md) <br/> |Содержит массив бесед, возвращаемого в **ответе FindConversation.**  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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



[FindConversation Operation](findconversation-operation.md)
  
[Операция ApplyConversationAction](applyconversationaction-operation.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

