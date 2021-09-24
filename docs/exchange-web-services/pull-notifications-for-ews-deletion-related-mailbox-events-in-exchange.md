---
title: Извлеките уведомления для событий почтового ящика, связанных с удалением EWS, в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Узнайте, какие события почтовых ящиков поднимаются при удалении элементов с помощью EWS в Exchange.
ms.openlocfilehash: fa04d49f02cfec621f00a9b51b121cff22ca393b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510416"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Извлеките уведомления для событий почтового ящика, связанных с удалением EWS, в Exchange

Узнайте, какие события почтовых ящиков поднимаются при удалении элементов с помощью EWS в Exchange.
  
При [удалении элементов](deleting-items-by-using-ews-in-exchange.md)и папок из почтового ящика запускается событие почтового ящика. Различные версии Exchange возвращают различные события почтовых ящиков в ответ на изменения элементов и папок в почтовом ящике. В следующей таблице определяются события почтовых ящиков, возвращаемые для удаления при использовании уведомлений о тяге для подписки на события почтовых ящиков. 
  
**Таблица 1. События почтовых ящиков, связанные с удалением, для уведомлений о вытягивке**

|**Тип удаления и операция EWS**|**Exchange 2010 г. при указании каждого идентификатора папки**|**Exchange 2010 г. при указании всех папок**|**Exchange Online и Exchange 2013 г. при указании каждого идентификатора папки**|**Exchange Online и Exchange 2013 г. при указании всех папок**|
|:-----|:-----|:-----|:-----|:-----|
|Мягкое удаление с помощью [операции DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |MovedEvent для элемента. Это указывает как старые, так и новые идентификаторы родительских папок. Элемент перемещается в папку Deletions в контейнере.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |DeletedEvent для элемента.  <br/> DeletedEvent для элемента из папки поиска по умолчанию AllItems.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |
|Жесткое удаление с помощью [операции DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |DeletedEvent для элемента.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |DeletedEvent для элемента.  <br/> DeletedEvent для элемента из папки поиска по умолчанию AllItems.  <br/> ModifiedEvent для родительской папки элемента.  <br/> |
|Перемещение в папку "Удаленные элементы" с помощью [операции DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent для элемента. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки элемента.  <br/> ModifiedEvent для новой родительской папки элемента, которая является папкой Удаленные элементы.  <br/> |MovedEvent для элемента. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки элемента.  <br/> ModifiedEvent для новой родительской папки элемента, которая является папкой Удаленные элементы.  <br/> |MovedEvent для элемента. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки элемента.  <br/> ModifiedEvent для новой родительской папки элемента, которая является папкой Удаленные элементы.  <br/> |DeletedEvent из папки поиска по умолчанию AllItems.  <br/> CreatedEvent для элемента в папке AllItems.  <br/> ModifiedEvent для исходной родительской папки элемента.  <br/> ModifiedEvent для папки Удаленные элементы.  <br/> |
|Мягкое удаление с помощью [операции DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |
|Жесткое удаление с помощью [операции DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |DeletedEvent для папки.  <br/> ModifiedEvent для родительской папки папки папки.  <br/> |
|Перемещение в папку "Удаленные элементы" с помощью [операции DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent для папки. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки.  <br/> ModifiedEvent для новой родительской папки "Удаленные элементы".  <br/> |MovedEvent для папки. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки.  <br/> ModifiedEvent для новой родительской папки "Удаленные элементы".  <br/> |MovedEvent для папки. Это указывает как старые, так и новые идентификаторы родительских папок.  <br/> ModifiedEvent для старой родительской папки.  <br/> ModifiedEvent для новой родительской папки "Удаленные элементы".  <br/> |ModifiedEvent для старой родительской папки.  <br/> ModifiedEvent для новой родительской папки "Удаленные элементы".  <br/> |
   
## <a name="see-also"></a>См. также


- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

