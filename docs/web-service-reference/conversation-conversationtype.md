---
title: Беседы (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: Элемент Conversation представляет разговора.
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761812"
---
# <a name="conversation-conversationtype"></a>Беседы (ConversationType)

Элемент **Conversation** представляет разговора. 
  
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
|[ConversationTopic](conversationtopic.md) <br/> |Представляет раздел беседы. Этот элемент доступен только для чтения.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Содержит список получателей беседы, собранные из определенной папки. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Содержит список получателей беседы сводный в почтовый ящик. Этот элемент доступен только для чтения.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Содержит список всех людей, отправленные сообщения, которые в настоящее время непрочитанные сообщения в эту беседу в текущую папку. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Содержит список всех людей, отправленные сообщения, в настоящее время непрочитанные сообщения в беседе для всех папок в почтовом ящике.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в текущую папку. Этот элемент доступен только для чтения.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Содержит список всех отправителей беседы элементов в почтовом ящике.  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |Содержит время доставки сообщений, который был получен последний в эту беседу в текущую папку.  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |Содержит время доставки сообщений, который был получен последний беседы во всех папках в почтовом ящике.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, которые определяют категории, которые применяются ко всем элементам беседы в текущей папке.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Содержит список категорий для всех элементов беседы в почтовом ящике.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Содержит объединенные флаг состояния для элементов беседы в текущую папку.  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |Содержит объединенные флаг состояния всех элементов беседы в почтовом ящике.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Содержит значение, указывающее, имеет ли беседы по крайней мере один элемент в текущей папке вложения.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.  <br/> |
|[MessageCount](messagecount.md) <br/> |Содержит общее число элементов беседы в текущую папку.  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |Содержит общее число элементов беседы в почтовом ящике.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Содержит число элементов непрочитанных сообщений в папке.  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |Содержит все непрочитанные сообщения беседы элементов в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Содержит размер беседы, вычисляемых из размер всех элементов беседы в текущую папку.  <br/> |
|[GlobalSize](globalsize.md) <br/> |Содержит размер беседы, вычисляемых из размер всех элементов беседы в почтовом ящике.  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |Содержит список классов элементов, представляющий все классы элементов из элементов беседы в текущей папке.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Содержит список классов элементов, представляющий все классы элементов беседы элементов в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Содержит объединенные важности для всех элементов беседы в текущую папку.  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |Содержит объединенные важности для всех элементов беседы в почтовом ящике.  <br/> |
|[Что ItemID](itemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в текущую папку.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Conversations](conversations-ex15websvcsotherref.md) <br/> |Содержит массив диалогов, возвращаемого в ответе **FindConversation** .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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



[FindConversation Operation](findconversation-operation.md)
  
[Операция ApplyConversationAction](applyconversationaction-operation.md)


[Conversations in EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

