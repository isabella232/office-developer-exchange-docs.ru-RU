---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: Элемент Икониндекс определяет индекс значка для элемента или беседы.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833848"
---
# <a name="iconindex"></a>IconIndex

Элемент **икониндекс** определяет индекс значка для элемента или беседы. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **икониндекстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Беседа (конверсатионтипе)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [дистрибутионлист](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md)календаритем | Task i[Item](postitem.md) | [Task](task.md)
  
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные текстовые значения для элемента **икониндекс** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|||
|По умолчанию  <br/> |Задает значок по умолчанию.  <br/> |
|PostItem  <br/> |Задает значок элемента POST.  <br/> |
|маилреад  <br/> |Указывает значок чтения почты.  <br/> |
|маилунреад  <br/> |Указывает значок непрочтенной почты.  <br/> |
|маилреплиед  <br/> |Указывает значок "ответ на сообщение".  <br/> |
|маилфорвардед  <br/> |Указывает значок переадресованной почты.  <br/> |
|маиленкриптед  <br/> |Указывает значок зашифрованной почты.  <br/> |
|маилсмимесигнед  <br/> |Указывает значок подписанного почтового расширения для безопасного или многоцелевого расширения почты в Интернете (S/MIME).  <br/> |
|маиленкриптедреплиед  <br/> |Указывает зашифрованный значок, на который отправлен ответ.  <br/> |
|маилсмимесигнедреплиед  <br/> |Указывает значок почтового ящика с подписанным сообщением S/MIME.  <br/> |
|маиленкриптедфорвардед  <br/> |Указывает значок зашифрованной переадресованной почты.  <br/> |
|маилсмимесигнедфорвардед  <br/> |Указывает значок переадресованного почтового ящика с подписью S/MIME.  <br/> |
|маиленкриптедреад  <br/> |Задает зашифрованный значок чтения почты.  <br/> |
|маилсмимесигнедреад  <br/> |Указывает подписанный значок чтения почты S/MIME.  <br/> |
|маилирм  <br/> |Указывает значок защищенной службы управления правами на доступ к данным (IRM).  <br/> |
|маилирмфорвардед  <br/> |Указывает значок переадресованной почты с защитой IRM.  <br/> |
|маилирмреплиед  <br/> |Указывает значок почты, защищенный с помощью службы управления правами на доступ к данным.  <br/> |
|смссубмиттед  <br/> |Указывает значок, отправленный для маршрутизации по протоколу коротких сообщений (SMS).  <br/> |
|смсраутедтоделиверипоинт  <br/> |Задает значок маршрутизации SMS для внешней точки доставки.  <br/> |
|смсраутедтоекстерналмессагингсистем  <br/> |Задает значок маршрутизации SMS для внешней системы обмена сообщениями.  <br/> |
|смсделиверед  <br/> |Указывает значок доставленной почты SMS.  <br/> |
|аутлукдефаултфорконтактс  <br/> |Задает значок по умолчанию для контактов.  <br/> |
|AppointmentItem  <br/> |Задает значок элемента встречи.  <br/> |
|аппоинтментрекур  <br/> |Задает значок повторяющейся встречи.  <br/> |
|аппоинтментмит  <br/> |Указывает значок собрания.  <br/> |
|аппоинтментмитрекур  <br/> |Задает значок повторяющегося собрания.  <br/> |
|аппоинтментмитни  <br/> |Задает значок ответа на приглашение на собрание.  <br/> |
|аппоинтментмитес  <br/> |Указывает значок принятия приглашения на собрание.  <br/> |
|аппоинтментмитно  <br/> |Указывает значок "собрание отклонено".  <br/> |
|аппоинтментмитмайбе  <br/> |Задает значок, который может отреагировать на собрание.  <br/> |
|аппоинтментмитканцел  <br/> |Указывает значок отмены собрания.  <br/> |
|аппоинтментмитинфо  <br/> |Указывает значок сведений о собрании.  <br/> |
|TaskItem  <br/> |Задает значок элемента задачи.  <br/> |
|таскрекур  <br/> |Задает значок повторяющейся задачи.  <br/> |
|тасковнед  <br/> |Указывает значок владельца задачи.  <br/> |
|таскделегатед  <br/> |Задает делегированный значок задачи.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

