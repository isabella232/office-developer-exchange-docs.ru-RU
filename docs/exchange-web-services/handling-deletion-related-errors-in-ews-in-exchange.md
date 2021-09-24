---
title: Обработка ошибок, связанных с удалением в EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Узнайте, как обрабатывать ошибки, связанные с удалением, в приложениях, которые вы разрабатываете с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: d82901a2ebc8577258e191cbd014db93cc40d099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513257"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с удалением в EWS в Exchange

Узнайте, как обрабатывать ошибки, связанные с удалением, в приложениях, которые вы разрабатываете с помощью управляемого API EWS или EWS в Exchange.
  
Если приложение удаляет [элементы и](deleting-items-by-using-ews-in-exchange.md)папки, возможно, вам придется обрабатывать ошибки, связанные с удалением. Вы можете обрабатывать эти ошибки во время работы или во время разработки приложения EWS.
  
**Таблица 1. Ошибки, связанные с удалением, и их обработка**

|**Ошибка**|**Возникает при попытке...**|**Обработать его...**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Удалите экземпляр повторяющейся задачи, и свойство **AffectedTaskOccurrence** не установлено.  <br/> |Настройка **свойства AffectedTaskOccurrence** и повторное удаление.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Обновим элемент календаря, расположенный в папке "Удаленные элементы", когда обновление приведет к отправке приглашения на собрание участникам.  <br/> |Отмена обновления или перемещение элемента календаря обратно в папку Календарь по умолчанию и обновление элемента календаря.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Ссылка на удаленный случай повторяющейся встречи.  <br/> |Удаление ссылки на удаленный случай.  <br/> |
|ErrorCannotDeleteObject  <br/> |Удаление элемента, который нельзя удалить.  <br/> |Отказ от попыток удаления элемента.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Удалите возникновение нерелигирующей задачи или удалите последнее возникновение повторяющейся задачи.  <br/> |Удаление нерелигирующей задачи или отказ от попыток удаления последнего возникновения повторяющейся задачи.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Удаление отличительной папки.  <br/> |Указание, что папки по умолчанию нельзя удалить.  <br/> |
|ErrorItemNotFound  <br/> |Доступ к постоянно удаленному элементу.  <br/> |Удаление ссылок на элемент при его удалении из магазина. Если элемент восстановлен, убедитесь, что вы восстанавливаете необходимые ссылки на клиента.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Удалите элемент календаря, не указав, следует ли отослать отмены собраний.  <br/> |Указание того, что отмена собрания должна быть отправлена или не должна быть отправлена.  <br/> |
   
## <a name="see-also"></a>См. также


- [Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Извлеките уведомления для событий почтового ящика, связанных с удалением EWS, в Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

