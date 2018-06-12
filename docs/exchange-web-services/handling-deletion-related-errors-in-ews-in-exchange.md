---
title: Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Узнайте, как обрабатывать ошибки, связанные с удаления в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 0dc16c3350bb75fb1e91650f0a0f0b7423727eeb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760945"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange

Узнайте, как обрабатывать ошибки, связанные с удаления в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Если ваше приложение [удаляет элементов и папок](deleting-items-by-using-ews-in-exchange.md), которые нужно обрабатывать ошибки, связанные с удаления. Может обрабатывать эти ошибки во время выполнения или при разработке приложения веб-служб Exchange.
  
**В таблице 1: Ошибки, связанные с удаления и порядок их обработки**

|**Error**|**Происходит при попытке...**|**Обработать его с...**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Удалите экземпляр повторяющейся задачи и **AffectedTaskOccurrence** свойство не задано.  <br/> |Установка свойства **AffectedTaskOccurrence** и повтор попытки удаления.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Обновите элемент календаря, расположенный в папки "Удаленные" после обновления приведет отправку собрания пригласить участников.  <br/> |Отмена обновления или перемещение элемента календаря обратно в папку по умолчанию календаря и обновление элемента календаря.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Ссылаться на удаленных вхождения повторяющейся встречи.  <br/> |Удаление ссылки на удаленных вхождение.  <br/> |
|ErrorCannotDeleteObject  <br/> |Удалите элемент, который не может быть удалена.  <br/> |Выход попытки удаления элемента.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Удалить вхождение неповторяющейся задачи или удалить последнюю копию повторяющейся задачи.  <br/> |Удаление неповторяющейся задачи или выход пытается удалить последнюю копию повторяющейся задачи.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Удаление различающееся папки.  <br/> |Указывает, что папок по умолчанию удалить невозможно.  <br/> |
|ErrorItemNotFound  <br/> |Доступ к без возможности восстановления удаленных элементов.  <br/> |Удаление ссылки на элемент, когда он удаляется из хранилища. Если восстанавливается элемента, убедитесь, что снова задать необходимые ссылки на клиенте.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Удаление элемента календаря без указания должна быть отправлена отмен собрания.  <br/> |Указание, что следует отмен собрания или не будут отправляться.  <br/> |
   
## <a name="see-also"></a>См. также


- [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [По запросу уведомления для событий, связанных с удаления почтового ящика веб-служб Exchange в Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

