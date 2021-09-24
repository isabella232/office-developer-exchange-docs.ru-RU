---
title: Операция CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: Операция CreateItem создает элементы в Exchange магазине.
ms.openlocfilehash: 2aee80d883aa623b8074ecc523d1a45fa71962da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538403"
---
# <a name="createitem-operation"></a>Операция CreateItem

Операция CreateItem создает элементы в Exchange магазине.
  
## <a name="using-the-createitem-operation"></a>Использование операции CreateItem

Вы можете использовать операцию CreateItem для создания следующих действий:
  
- Элементы календаря
    
- Сообщения электронной почты
    
- приглашения на собрания;
    
- Задачи
    
- Контакты
    
Дополнительные сведения см. в статьях [CreateItem operation (элемент календаря),](createitem-operation-calendar-item.md) [CreateItem operation (сообщение](createitem-operation-email-message.md)электронной почты), [CreateItem operation (запрос собрания),](createitem-operation-meeting-request.md) [CreateItem operation (task)](createitem-operation-task.md)и [CreateItem operation (contact).](createitem-operation-contact.md)
  
Операция CreateItem поддерживает использование объектов отклика. Объекты отклика поддерживают принятие и отклонение собраний и обработку кнопок голосования, включенных в стандартное сообщение электронной почты. В следующей таблице перечислены объекты отклика, обрабатываются в операции CreateItem.
  
|**Объект response**|**Действие**|
|:-----|:-----|
|AcceptItem  <br/> |Примите запрос на собрание.  <br/> |
|CancelCalendarItem  <br/> |Отмена собрания. Это отличается от удаления всех участников, так как оно также удаляет собрание для организатора.  <br/> |
|DeclineItem  <br/> |Отклонение запроса на собрание.  <br/> |
|ForwardItem  <br/> |Отправьте запрос на собрание другому лицу в качестве запроса на собрание.  <br/> |
|RemoveItem  <br/> |Удаление отмененного собрания из календаря.  <br/> |
|ReplyAllToItem  <br/> |Отправьте всем участникам собрания сообщение, в которое входит текст исходного запроса собрания.  <br/> |
|ReplyToItem  <br/> |Отправьте отправительу запроса собрания сообщение, в которое включено тело исходного запроса собрания.  <br/> |
|SendReadReceipt  <br/> |Отправьте квитанцию о прочтителье отправителю запроса на собрание.  <br/> |
|TentativelyAcceptItem  <br/> |Предварительно принять запрос на собрание.  <br/> |
   
Операция CreateItem также поддерживает дополнительные объекты собраний. В следующей таблице перечислены дополнительные объекты, поддерживаемые операцией CreateItem.
  
|**Объект Meeting**|**Описание**|
|:-----|:-----|
|Сообщение о собрании  <br/> |Представляет сообщение собрания в Exchange магазине. Это базовый объект для других объектов собраний.  <br/> |
|Запрос на собрание  <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|Ответы на собрания  <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|Отмена собрания  <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateItem (элемент календаря)](createitem-operation-calendar-item.md)
  
[Операция CreateItem (контакт)](createitem-operation-contact.md)
  
[Операция CreateItem (электронное сообщение)](createitem-operation-email-message.md)
  
[Операция CreateItem (приглашение на собрание)](createitem-operation-meeting-request.md)
  
[Операция CreateItem (задача)](createitem-operation-task.md)
  
 **CreateItemType**

