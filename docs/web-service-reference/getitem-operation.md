---
title: GetItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Найдите сведения о веб-служб Exchange GetItem операции.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762834"
---
# <a name="getitem-operation"></a>GetItem Operation

Найдите сведения о операции **GetItem** веб-служб Exchange. 
  
Операции **GetItem** получает элементы из хранилища Exchange. 
  
## <a name="using-the-getitem-operation"></a>С помощью операции GetItem

Операции **GetItem** Возвращает множество свойств элемента. Свойства, возвращаемые в ответ **GetItem** различаться в зависимости от запрошенного фигуры возвращать запрошенный дополнительных свойств и типа элемента. 
  
Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange (EWS). Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы [сообщения](message-ex15websvcsotherref.md) . Exchange не возвращает [базовый элемент](item.md) в ответы. 
  
Операции **GetItem** не возвращает вложения. Возвращает метаданные о вложенного элемента или файла. Чтобы вернуть вложение, с помощью [операции GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>Заголовки SOAP операции GetItem

Операции **GetItem** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|Заголовок ***|****Element****|****Описание****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Указывает разрешение значения времени и данных в ответов с сервера, в секундах или в миллисекундах.  <br/> |
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов с сервера.  <br/> |
   
## <a name="in-this-section"></a>В этом разделе

[Операции GetItem (сообщение электронной почты)](getitem-operation-email-message.md)
  
[Операции GetItem (элемента календаря)](getitem-operation-calendar-item.md)
  
[Операции GetItem (задача)](getitem-operation-task.md)
  
[Операции GetItem (контактов)](getitem-operation-contact.md)
  
## <a name="see-also"></a>См. также



[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

