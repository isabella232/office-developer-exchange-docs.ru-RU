---
title: Операция CreateItem
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
description: Операция CreateItem создает элементы в хранилище Exchange.
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458868"
---
# <a name="createitem-operation"></a>Операция CreateItem

Операция CreateItem создает элементы в хранилище Exchange.
  
## <a name="using-the-createitem-operation"></a>Использование операции CreateItem

С помощью операции CreateItem можно создать следующее:
  
- Элементы календаря
    
- Сообщения электронной почты
    
- Приглашения на собрания
    
- Задачи
    
- Контакты
    
Для получения дополнительных сведений см. [Операция CreateItem (элемент календаря)](createitem-operation-calendar-item.md), [Операция CreateItem (сообщение электронной почты)](createitem-operation-email-message.md), [Операция CreateItem (приглашение на собрание)](createitem-operation-meeting-request.md), [Операция CreateItem (Task)](createitem-operation-task.md)и [Операция CreateItem (Contact)](createitem-operation-contact.md).
  
Операция CreateItem поддерживает использование объектов Response. Объекты Response поддерживают принятие и отклонение собраний и обработку кнопок голосования, включенных в стандартное электронное сообщение. В следующей таблице перечислены объекты ответа, которые обрабатываются в операции CreateItem.
  
|**Объект Response**|**Действие**|
|:-----|:-----|
|акцептитем  <br/> |Принятие приглашения на собрание.  <br/> |
|канцелкалендаритем  <br/> |Отмена собрания. Это отличается от удаления всех участников, так как он также удаляет собрание для организатора.  <br/> |
|деклинеитем  <br/> |Отклонение приглашения на собрание.  <br/> |
|форвардитем  <br/> |Отправка приглашения на собрание другому человеку в качестве приглашения на собрание.  <br/> |
|RemoveItem  <br/> |Удаление отмененного собрания из календаря.  <br/> |
|репляллтоитем  <br/> |Отправьте сообщение, содержащее текст исходного приглашения на собрание всем участникам собрания.  <br/> |
|реплитоитем  <br/> |Отправьте сообщение, содержащее текст исходного приглашения на собрание отправителю приглашения на собрание.  <br/> |
|сендреадрецеипт  <br/> |Отправка уведомления о прочтении отправителю приглашения на собрание.  <br/> |
|тентативелякцептитем  <br/> |Принятие приглашения на собрание под вопросом.  <br/> |
   
Операция CreateItem также поддерживает дополнительные объекты Meeting. В следующей таблице перечислены дополнительные объекты, поддерживаемые операцией CreateItem.
  
|**Объект Meeting**|**Описание**|
|:-----|:-----|
|Сообщение о собрании  <br/> |Представляет сообщение о собрании в хранилище Exchange. Это базовый объект для других объектов Meeting.  <br/> |
|Приглашение на собрание  <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|Ответ на приглашение на собрание  <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|Отмена собрания  <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateItem (элемент календаря)](createitem-operation-calendar-item.md)
  
[Операция CreateItem (Contact)](createitem-operation-contact.md)
  
[Операция CreateItem (сообщение электронной почты)](createitem-operation-email-message.md)
  
[Операция CreateItem (приглашение на собрание)](createitem-operation-meeting-request.md)
  
[Операция CreateItem (задача)](createitem-operation-task.md)
  
 **креатеитемтипе**

