---
title: Обработка ошибок, связанных с делегирования в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Узнайте, как обрабатывать ошибки, связанные с делегирования в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 3851709888e3a1087df02eea5d4d58888ad168e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760948"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с делегирования в веб-служб Exchange в Exchange

Узнайте, как обрабатывать ошибки, связанные с делегирования в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Если приложение использует делегирование или добавляет или удаляет делегатов, может потребоваться обрабатывать ошибки, связанные с делегирования. Может обрабатывать эти ошибки во время выполнения или при разработке приложения веб-служб Exchange. Эти ошибки определяются перечисление управляемый API EWS [ServiceError](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) и веб-служб Exchange [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) элемент. 
  
## <a name="delegation-related-errors"></a>Ошибки, связанные с делегирования

|**Error**|**Происходит при попытке...**|**Обработать его с...**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Выполнение операции в почтовый ящик, папки или элемента, не имеют доступа к.  <br/> |Обновление разрешений делегата, чтобы они могли получить доступ к папке или элемента путем вызова метода управляемый API EWS [UpdateDelegates](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) или операции [UpdateDelegate](http://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) EWS и затем Повтор запроса.  <br/> |
|ErrorAccessDenied  <br/> |Изменение элементов, у вас необходимые разрешения для изменения.  <br/> |Обновление делегированных разрешений путем вызова метода управляемый API EWS **UpdateDelegate** или операции **UpdateDelegate** EWS и затем Повтор запроса.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |При попытке добавить владельца почтового ящика в качестве делегата своего почтового ящика.  <br/> |[Добавление другого пользователя в качестве делегата](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md), не владельца почтового ящика.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Добавьте делегата, когда делегат уже существует.  <br/> |Так как делегат уже существует для владельца почтового ящика не выполняет никаких действий. Или, если вы пытаетесь изменить разрешения для существующего делегата, а затем с помощью метода **UpdateDelegates** или **UpdateDelegate** операции.  <br/> |
|ErrorNotDelegate  <br/> |Изменение делегированных разрешений для пользователя, который не имеет Делегирование разрешений для почтового ящика.  <br/> |[Добавление пользователя в качестве делегата](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для почтового ящика, прежде чем обновить или удалить их разрешения.  <br/> |
|ErrorDelegateNoUser  <br/> |Изменение делегированных разрешений для пользователя, который не находится в доменной службы Active Directory (AD DS).  <br/> |Создание пользователя в Доменных службах Active Directory или исправление делегат сведения в запросе.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Используйте делегат для подписки на уведомления от имени владельца почтового ящика.  <br/> |Подписка на уведомления в качестве владельца почтового ящика.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Для выполнения запроса из делегата, который имеет другой сервер версии, чем основной сервер почтовых ящиков.  <br/> |С помощью делегата или добавления делегата, почтовый ящик которого имеется та же версия сервера в качестве владельца почтового ящика.  <br/> |
|ErrorMissingEmailAddress  <br/> |Для выполнения запроса, делегат учетной записью, которая не имеет почтового ящика.  <br/> |Добавление почтового ящика представителя учетной записи.  <br/> |
   
## <a name="see-also"></a>См. также


- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

