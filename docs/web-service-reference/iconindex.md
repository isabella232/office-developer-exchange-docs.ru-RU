---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: Элемент IconIndex определяет индекс значка для элемента или беседы.
ms.openlocfilehash: f0c024eeedcbda9aa5ad8afdea09a68f2499798e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541163"
---
# <a name="iconindex"></a>IconIndex

Элемент **IconIndex** определяет индекс значка для элемента или беседы. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Беседа (ConversationType)](conversation-conversationtype.md)  |  [Item](item.md)  |  [Контакт](contact.md)  |  [DistributionList](distributionlist.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Задача](task.md)
  
## <a name="text-value"></a>Текстовое значение

В следующей таблице представлены возможные текстовые значения элемента **IconIndex.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|||
|По умолчанию  <br/> |Указывает значок по умолчанию.  <br/> |
|PostItem  <br/> |Указывает значок для элемента post.  <br/> |
|MailRead  <br/> |Указывает значок чтения почты.  <br/> |
|MailUnread  <br/> |Указывает нечитаемую иконку почты.  <br/> |
|MailReplied  <br/> |Указывает ответ на значок почты.  <br/> |
|MailForwarded  <br/> |Указывает значок пересылаемой почты.  <br/> |
|MailEncrypted  <br/> |Указывает значок зашифрованной почты.  <br/> |
|MailSmimeSigned  <br/> |Указывает значок электронной почты с подписью Secure/Multipurpose Internet Mail Extensions (S/MIME).  <br/> |
|MailEncryptedReplied  <br/> |Указывает зашифрованный ответ на значок почты.  <br/> |
|MailSmimeSignedReplied  <br/> |Указывает подписанный S/MIME ответ на значок почты.  <br/> |
|MailEncryptedForwarded  <br/> |Указывает зашифрованный значок пересылаемой почты.  <br/> |
|MailSmimeSignedForwarded  <br/> |Указывает значок электронной почты с подписью S/MIME.  <br/> |
|MailEncryptedRead  <br/> |Указывает зашифрованный значок почты чтения.  <br/> |
|MailSmimeSignedRead  <br/> |Указывает значок электронной почты с подписью S/MIME.  <br/> |
|MailIrm  <br/> |Указывает значок электронной почты с защитой прав на информацию (IRM).  <br/> |
|MailIrmForwarded  <br/> |Указывает значок электронной почты, защищенный защитой IRM.  <br/> |
|MailIrmReplied  <br/> |Указывает защищенный IRM ответ на значок почты.  <br/> |
|SmsSubmitted  <br/> |Указывает иконописную почту, отправленную для маршрутивки службы коротких сообщений (SMS).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Указывает значок маршрутивки SMS на внешнюю точку доставки.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Указывает значок маршрутивки SMS во внешнюю систему обмена сообщениями.  <br/> |
|SmsDelivered  <br/> |Указывает значок отправленной почты SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Указывает значок по умолчанию для контактов.  <br/> |
|AppointmentItem  <br/> |Указывает значок элемента назначения.  <br/> |
|AppointmentRecur  <br/> |Указывает повторяющийся значок встречи.  <br/> |
|AppointmentMeet  <br/> |Указывает значок собрания.  <br/> |
|AppointmentMeetRecur  <br/> |Указывает повторяющийся значок собрания.  <br/> |
|AppointmentMeetNY  <br/> |Указывает значок для предварительного ответа на собрание.  <br/> |
|AppointmentMeetYes  <br/> |Указывает значок принятия собрания.  <br/> |
|AppointmentMeetNo  <br/> |Указывает значок отклоненного собрания.  <br/> |
|AppointmentMeetMaybe  <br/> |Указывает значок для возможного ответа на собрание.  <br/> |
|AppointmentMeetCancel  <br/> |Указывает значок отмены собрания.  <br/> |
|AppointmentMeetInfo  <br/> |Указывает значок сведений о собрании.  <br/> |
|TaskItem  <br/> |Указывает значок элемента задачи.  <br/> |
|TaskRecur  <br/> |Указывает повторяющийся значок задачи.  <br/> |
|TaskOwned  <br/> |Указывает значок задачи, который принадлежит.  <br/> |
|TaskDelegated  <br/> |Указывает значок делегированная задача.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

