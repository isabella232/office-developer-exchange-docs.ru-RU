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
description: Элемент CONVERSATION представляет одну беседу.
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458938"
---
# <a name="conversation-conversationtype"></a>Беседы (ConversationType)

Элемент **CONVERSATION** представляет одну беседу. 
  
[финдконверсатионреспонсе](findconversationresponse.md)
  
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

 **конверсатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет раздел "Беседа". Этот элемент доступен только для чтения.  <br/> |
|[уникуереЦипиентс](uniquerecipients.md) <br/> |Содержит список получателей беседы, собранные из определенной папки. Этот элемент доступен только для чтения.  <br/> |
|[глобалуникуереЦипиентс](globaluniquerecipients.md) <br/> |Содержит список получателей беседы, собранные по почтовому ящику. Этот элемент доступен только для чтения.  <br/> |
|[уникуеунреадсендерс](uniqueunreadsenders.md) <br/> |Содержит список всех пользователей, которые отправили сообщения, которые в настоящее время не прочитаны в текущей папке. Этот элемент доступен только для чтения.  <br/> |
|[глобалуникуеунреадсендерс](globaluniqueunreadsenders.md) <br/> |Содержит список всех пользователей, которые отправили сообщение, непрочтенное в этой беседе, во всех папках почтового ящика.  <br/> |
|[уникуесендерс](uniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в текущей папке. Этот элемент доступен только для чтения.  <br/> |
|[глобалуникуесендерс](globaluniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в почтовом ящике.  <br/> |
|[ластделиверитиме](lastdeliverytime.md) <br/> |Содержит время доставки сообщения, которое было последний раз получено в этой беседе в текущей папке.  <br/> |
|[глобалластделиверитиме](globallastdeliverytime.md) <br/> |Содержит время доставки сообщения, которое было последний раз получено в этой беседе, во всех папках почтового ящика.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, определяющих категории, которые применяются ко всем элементам бесед в текущей папке.  <br/> |
|[глобалкатегориес](globalcategories.md) <br/> |Содержит список категорий для всех элементов бесед в почтовом ящике.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Содержит сводный статус флага для элементов беседы в текущей папке.  <br/> |
|[глобалфлагстатус](globalflagstatus.md) <br/> |Содержит сводный статус флага для всех элементов бесед в почтовом ящике.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Содержит значение, указывающее, есть ли вложение по крайней мере для одного элемента беседы в текущей папке.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Содержит значение, указывающее, имеет ли хотя бы один элемент в почтовом ящике вложение.  <br/> |
|[MessageCount](messagecount.md) <br/> |Содержит общее число элементов беседы в текущей папке.  <br/> |
|[глобалмессажекаунт](globalmessagecount.md) <br/> |Содержит общее число элементов беседы в почтовом ящике.  <br/> |
|[унреадкаунт](unreadcount.md) <br/> |Содержит число непрочитанных элементов беседы в папке.  <br/> |
|[глобалунреадкаунт](globalunreadcount.md) <br/> |Содержит количество всех непрочтенных элементов беседы в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Содержит размер беседы, рассчитанный на основе размера всех элементов бесед в текущей папке.  <br/> |
|[глобалсизе](globalsize.md) <br/> |Содержит размер диалога, рассчитанный на основе размера всех элементов бесед в почтовом ящике.  <br/> |
|[Итемклассес (Аррайофитемкласстипе)](itemclasses-arrayofitemclasstype.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в текущей папке.  <br/> |
|[глобалитемклассес](globalitemclasses.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Содержит совокупную важность для всех элементов бесед в текущей папке.  <br/> |
|[глобалимпортанце](globalimportance.md) <br/> |Содержит совокупную важность для всех элементов бесед в почтовом ящике.  <br/> |
|[итемидс](itemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов бесед в текущей папке.  <br/> |
|[глобалитемидс](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы](conversations-ex15websvcsotherref.md) <br/> |Содержит массив бесед, возвращаемых в ответе **FindConversation** .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindConversation Operation](findconversation-operation.md)
  
[Операция ApplyConversationAction](applyconversationaction-operation.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

