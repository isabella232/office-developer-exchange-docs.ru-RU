---
title: CreateItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: Операции CreateItem создает элементов в хранилище Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761897"
---
# <a name="createitem-operation"></a>CreateItem Operation

Операции CreateItem создает элементов в хранилище Exchange.
  
## <a name="using-the-createitem-operation"></a>С помощью операции CreateItem

Можно использовать операцию CreateItem для создания следующих:
  
- Элементы календаря
    
- Сообщения электронной почты
    
- Приглашения на собрания
    
- Задачи
    
- Контакты
    
Для получения дополнительных сведений см [операции CreateItem (элемента календаря)](createitem-operation-calendar-item.md), [операции CreateItem (сообщение электронной почты)](createitem-operation-email-message.md), [операции CreateItem (собрание)](createitem-operation-meeting-request.md), [операции CreateItem (задача)](createitem-operation-task.md)и [операции CreateItem (контактов) ](createitem-operation-contact.md).
  
Операции CreateItem поддерживает использование объекты ответа. Объекты ответа поддерживает приемки и отклонения собраний и обработки кнопки голосования, которые включены в стандартные электронные сообщения. В следующей таблице перечислены объекты ответа, которые обрабатываются в операции CreateItem.
  
|**Объект ответа**|**Действие**|
|:-----|:-----|
|AcceptItem  <br/> |Принятие приглашения на собрание.  <br/> |
|CancelCalendarItem  <br/> |Отмена собрания. Это отличается от удаления всех участников, так как он также удаляет для организатора собрания.  <br/> |
|DeclineItem  <br/> |Отклонение приглашения на собрание.  <br/> |
|ForwardItem  <br/> |Отправьте приглашения на собрание другому пользователю в виде приглашения на собрание.  <br/> |
|RemoveItem  <br/> |Удалите отмененные собрания из календаря.  <br/> |
|ReplyAllToItem  <br/> |Отправьте сообщение, содержащее текст исходного запроса на проведение собрания всем участникам собрания.  <br/> |
|ReplyToItem  <br/> |Отправьте сообщение, содержащее текст исходного запроса на проведение собрания отправителю приглашения на собрание.  <br/> |
|SendReadReceipt  <br/> |Отправьте уведомление отправителю приглашения на собрание.  <br/> |
|TentativelyAcceptItem  <br/> |Предварительное принятие приглашения на собрание.  <br/> |
   
Операции CreateItem также поддерживает дополнительных объектов. В следующей таблице перечислены дополнительные объекты, поддерживаемые операции CreateItem.
  
|**Объект собрания**|**Описание**|
|:-----|:-----|
|Сообщения о собрании  <br/> |Представляет сообщение собрания в хранилище Exchange. Это базовый объект для других объектов собрания.  <br/> |
|Приглашения на собрание  <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|Приглашения на собрание  <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|Отмена собрания  <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
   
## <a name="see-also"></a>См. также



[Операции CreateItem (элемента календаря)](createitem-operation-calendar-item.md)
  
[Операции CreateItem (контактов)](createitem-operation-contact.md)
  
[Операции CreateItem (сообщение электронной почты)](createitem-operation-email-message.md)
  
[Операции CreateItem (запрос на собрание)](createitem-operation-meeting-request.md)
  
[Операции CreateItem (задача)](createitem-operation-task.md)
  
 **CreateItemType**

