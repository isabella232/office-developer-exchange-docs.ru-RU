---
title: Обработка ошибок, связанных с делегированиями в EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Узнайте, как обрабатывать ошибки, связанные с делегированиями, в приложениях, которые разрабатываются с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 17e4e7898f5cbed7a6dc524a84db6ba4080eab88
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512298"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с делегированиями в EWS в Exchange

Узнайте, как обрабатывать ошибки, связанные с делегированиями, в приложениях, которые разрабатываются с помощью управляемого API EWS или EWS в Exchange.
  
Если ваше приложение использует делегирования или добавляет или удаляет делегатов, возможно, вам придется обрабатывать ошибки, связанные с делегирования. Вы можете обрабатывать эти ошибки во время работы или во время разработки приложения EWS. Эти ошибки определяются переумежением EWS Managed API [ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) и элементом EWS [ResponseCode.](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
  
## <a name="delegation-related-errors"></a>Ошибки, связанные с делегированиями

|**Ошибка**|**Возникает при попытке...**|**Обработать его...**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Выполните операцию на почтовом ящике, папке или элементе, к который у вас нет доступа.  <br/> |Обновление разрешений делегата для доступа к папке или элементу путем вызова метода управляемого API [UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) EWS или операции [UpdateDelegate](https://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) EWS, а затем повторного запроса.  <br/> |
|ErrorAccessDenied  <br/> |Измените элемент, который не имеет достаточных привилегий для изменения.  <br/> |Обновление разрешений делегатов путем вызова метода управляемого API **UpdateDelegate** EWS или операции **UpdateDelegate** EWS, а затем повторного запроса.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Попытка добавить владельца почтового ящика в качестве делегата в собственный почтовый ящик.  <br/> |[Добавление другого пользователя в качестве делегата,](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)а не владельца почтового ящика.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Добавьте делегата, когда делегат уже существует.  <br/> |Ничего не делать, так как делегат уже существует для владельца почтового ящика. Или, если вы пытаетесь изменить разрешения существующего делегата, используйте метод **UpdateDelegates** или **операцию UpdateDelegate.**  <br/> |
|ErrorNotDelegate  <br/> |Изменение разрешений делегирования для пользователя, у которого нет разрешений делегирования для почтового ящика.  <br/> |[Добавление пользователя в качестве делегата](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для почтового ящика перед попыткой обновить или удалить разрешения.  <br/> |
|ErrorDelegateNoUser  <br/> |Изменение разрешений делегирования для пользователя, который не находится в службе домена Active Directory (AD DS).  <br/> |Создание пользователя в AD DS или исправление сведений делегата в запросе.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Используйте делегата для подписки на уведомления от имени владельца почтового ящика.  <br/> |Подписка на уведомления в качестве владельца почтового ящика.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Сделайте запрос от делегата, который имеет другую версию сервера, чем сервер почтовых ящиков директора.  <br/> |Использование делегата или добавление делегата, почтовый ящик которого имеет ту же версию сервера, что и владелец почтового ящика.  <br/> |
|ErrorMissingEmailAddress  <br/> |Сделайте запрос с помощью учетной записи делегата, у нее нет почтового ящика.  <br/> |Добавление почтового ящика в учетную запись делегата.  <br/> |
   
## <a name="see-also"></a>См. также


- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

