---
title: По запросу уведомления для событий, связанных с удаления почтового ящика веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Узнайте, какие почтового ящика событий при удалении элементов с помощью веб-служб Exchange в Exchange.
ms.openlocfilehash: b12d6a16cc539f36b6b4dcd7274529e9def3c247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761238"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>По запросу уведомления для событий, связанных с удаления почтового ящика веб-служб Exchange в Exchange

Узнайте, какие почтового ящика событий при удалении элементов с помощью веб-служб Exchange в Exchange.
  
После [удаления элементов и папок, из почтового ящика](deleting-items-by-using-ews-in-exchange.md), это вызывает события почтового ящика. Различными версиями Exchange возврата события другой почтовый ящик в соответствии с изменениями для элементов и папок в почтовом ящике. В следующей таблице указываются события почтовый ящик, для удаления возвращаются при использовании репликации по запросу уведомления для подписки на события почтового ящика. 
  
**Таблица 1: События удаления связанных почтовых ящиков для уведомления по запросу**

|**Тип удаления и операции веб-служб Exchange**|**Exchange 2010 уведомлений при указании идентификатора каждой папки**|**Exchange 2010 уведомлений при указании всех папок**|**Exchange Online и Exchange 2013 уведомлений при указании идентификатора каждой папки**|**Exchange Online и Exchange 2013 при указании всех папок**|
|:-----|:-----|:-----|:-----|:-----|
|С помощью [операции DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) обратимым удалением <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent папку родительского элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent папку родительского элемента.  <br/> |MovedEvent для элемента. Указывает, как идентификаторы старой и новой родительских папок. Перемещено в папку Удаленные элементы в корзине.  <br/> ModifiedEvent папку родительского элемента.  <br/> |DeletedEvent для элемента.  <br/> DeletedEvent для элемента из папки поиска по умолчанию AllItems.  <br/> ModifiedEvent папку родительского элемента.  <br/> |
|С помощью [операции DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) окончательного удаления <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent папку родительского элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent папку родительского элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent папку родительского элемента.  <br/> |DeletedEvent для элемента.  <br/> DeletedEvent для элемента из папки поиска по умолчанию AllItems.  <br/> ModifiedEvent папку родительского элемента.  <br/> |
|Перемещение папки «Удаленные» с помощью [операции DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent для элемента. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старую папку родительского элемента.  <br/> ModifiedEvent для новой родительской папки элемента, являющийся папки "Удаленные".  <br/> |MovedEvent для элемента. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старую папку родительского элемента.  <br/> ModifiedEvent для новой родительской папки элемента, являющийся папки "Удаленные".  <br/> |MovedEvent для элемента. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старую папку родительского элемента.  <br/> ModifiedEvent для новой родительской папки элемента, являющийся папки "Удаленные".  <br/> |DeletedEvent из папки поиска по умолчанию AllItems.  <br/> CreatedEvent для элемента в папке AllItems.  <br/> ModifiedEvent для элемента исходной родительской папки.  <br/> ModifiedEvent для папки «Удаленные».  <br/> |
|Обратимым удалением с помощью [операции DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |
|Окончательного удаления с помощью [операции DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки.  <br/> |
|Перемещение папки «Удаленные» с помощью [операции DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent для папки. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старый родительской папки.  <br/> ModifiedEvent новые родительской папки, который является папки "Удаленные".  <br/> |MovedEvent для папки. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старый родительской папки.  <br/> ModifiedEvent новые родительской папки, который является папки "Удаленные".  <br/> |MovedEvent для папки. Это свойство определяет идентификаторы обоих старой и новой родительских папок.  <br/> ModifiedEvent старый родительской папки.  <br/> ModifiedEvent новые родительской папки, который является папки "Удаленные".  <br/> |ModifiedEvent старый родительской папки.  <br/> ModifiedEvent для новой родительской папки являющийся папки "Удаленные".  <br/> |
   
## <a name="see-also"></a>См. также


- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

