---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: Элемент IconIndex определяет индекс значка для элемента или беседы.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833848"
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

[Беседы (ConversationType)](conversation-conversationtype.md) | [элемента](item.md) | [контакт](contact.md) | [DistributionList](distributionlist.md) | [сообщение](message-ex15websvcsotherref.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач ](task.md)
  
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **IconIndex** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|||
|Значение по умолчанию  <br/> |Указывает значок по умолчанию.  <br/> |
|PostItem  <br/> |Указывает значок для элемента записи.  <br/> |
|MailRead  <br/> |Указывает, что значок чтения почты.  <br/> |
|MailUnread  <br/> |Указывает значок непрочитанных сообщений.  <br/> |
|MailReplied  <br/> |Задает пересылаемых значок Почта.  <br/> |
|MailForwarded  <br/> |Указывает значок пересылки почты.  <br/> |
|MailEncrypted  <br/> |Указывает значок зашифрованных сообщений.  <br/> |
|MailSmimeSigned  <br/> |Указывает значок подписью безопасные многоцелевые расширения почтового стандарта Интернета (S/MIME).  <br/> |
|MailEncryptedReplied  <br/> |Указывает, что зашифрованные ответ значок Почта.  <br/> |
|MailSmimeSignedReplied  <br/> |Указывает, что S/MIME подписанные пересылаемых значок Почта.  <br/> |
|MailEncryptedForwarded  <br/> |Указывает значок зашифрованных переадресованных сообщений.  <br/> |
|MailSmimeSignedForwarded  <br/> |Указывает, подписью S/MIME пересылку значок Почта.  <br/> |
|MailEncryptedRead  <br/> |Указывает значок зашифрованные чтения почты.  <br/> |
|MailSmimeSignedRead  <br/> |Указывает, подписью S/MIME чтение значок Почта.  <br/> |
|MailIrm  <br/> |Указывает значок Почта защищенного управления правами.  <br/> |
|MailIrmForwarded  <br/> |Указывает, защищенных службой IRM пересылку значок Почта.  <br/> |
|MailIrmReplied  <br/> |Указывает, что IRM-защитой дан ответ значок Почта.  <br/> |
|SmsSubmitted  <br/> |Указывает значок почты, отправленные на маршрутизации службы коротких сообщений (SMS).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Указывает значок для SMS маршрутизации к точке внешних доставки.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Указывает значок для маршрутизации SMS для внешней системы обмена сообщениями.  <br/> |
|SmsDelivered  <br/> |Указывает значок доставлено почты SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Указывает значок по умолчанию для контактов.  <br/> |
|AppointmentItem  <br/> |Указывает значок элемента встречи.  <br/> |
|AppointmentRecur  <br/> |Указывает значок повторяющейся встречи.  <br/> |
|AppointmentMeet  <br/> |Указывает значок собрания.  <br/> |
|AppointmentMeetRecur  <br/> |Указывает значок повторяющихся собраний.  <br/> |
|AppointmentMeetNY  <br/> |Указывает значок под вопросом ответа на приглашение на собрание.  <br/> |
|AppointmentMeetYes  <br/> |Указывает собрания значок приемки.  <br/> |
|AppointmentMeetNo  <br/> |Указывает значок отклоненные собрания.  <br/> |
|AppointmentMeetMaybe  <br/> |Указывает значок может быть ответа на приглашение на собрание.  <br/> |
|AppointmentMeetCancel  <br/> |Указывает значок Отменить собрание.  <br/> |
|AppointmentMeetInfo  <br/> |Указывает собрания значок информации.  <br/> |
|TaskItem  <br/> |Указывает значок элемента задачи.  <br/> |
|TaskRecur  <br/> |Указывает значок повторяющейся задачи.  <br/> |
|TaskOwned  <br/> |Определяет задачу, владельцем которого значок.  <br/> |
|TaskDelegated  <br/> |Указывает значок делегированные задачи.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

