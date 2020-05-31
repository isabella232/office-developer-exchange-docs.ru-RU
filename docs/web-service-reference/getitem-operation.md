---
title: Операция GetItem
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
description: Найдите сведения о операции GetItem EWS.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762834"
---
# <a name="getitem-operation"></a>Операция GetItem

Найдите сведения о операции **GetItem** EWS. 
  
Операция **GetItem** возвращает элементы из хранилища Exchange. 
  
## <a name="using-the-getitem-operation"></a>Использование операции GetItem

Операция **GetItem** возвращает множество свойств элемента. Свойства, возвращаемые в ответе **GetItem** , зависят от запрошенной фигуры, запрашивают дополнительные свойства и тип возвращаемого элемента. 
  
Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS). Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов [Message](message-ex15websvcsotherref.md) . Exchange не возвращает элемент базового [элемента](item.md) в ответах. 
  
Операция **GetItem** не возвращает вложения. Он возвращает метаданные о вложенном элементе или файле. Чтобы вернуть вложение, используйте [операцию GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>Заголовки SOAP для операции GetItem

Операция **GetItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|Header * * * *|****Element****|****Описание****|
|:-----|:-----|:-----|
|**датетимепреЦисион** <br/> |[датетимепреЦисион](datetimeprecision.md) <br/> |Задает разрешение значений данных и времени в ответах от сервера: в секундах или в миллисекундах.  <br/> |
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос.  <br/> |
|**тимезонеконтекст** <br/> |[тимезонеконтекст](timezonecontext.md) <br/> |Определяет часовой пояс, который будет использоваться для всех ответов сервера.  <br/> |
   
## <a name="in-this-section"></a>Содержание

[Операция GetItem (сообщение электронной почты)](getitem-operation-email-message.md)
  
[Операция GetItem (элемент календаря)](getitem-operation-calendar-item.md)
  
[Операция GetItem (задача)](getitem-operation-task.md)
  
[Операция GetItem (контакт)](getitem-operation-contact.md)
  
## <a name="see-also"></a>См. также



[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

