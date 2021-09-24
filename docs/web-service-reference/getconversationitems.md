---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: Элемент GetConversationItems определяет запрос, чтобы получить набор элементов, связанных, находясь в одном разговоре.
ms.openlocfilehash: 0bd792553cbab0c03a6c2cd5bfdbc18dfeba4273
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538119"
---
# <a name="getconversationitems"></a>GetConversationItems

Элемент **GetConversationItems** определяет запрос, чтобы получить набор элементов, связанных, находясь в одном разговоре. 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 **GetConversationItemsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[ItemShape](itemshape.md)  |  [FoldersToIgnore](folderstoignore.md)  |  [MaxItemsToReturn](maxitemstoreturn.md)  |  [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)  |  [MailboxScope](mailboxscope.md)  |  [Беседы](conversations-ex15websvcsotherref.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

