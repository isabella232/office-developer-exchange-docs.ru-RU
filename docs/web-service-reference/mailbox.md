---
title: Почтовый ящик
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Элемент Mailbox определяет объект Active Directory с включенной поддержкой почты.
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468203"
---
# <a name="mailbox"></a>Почтовый ящик

Элемент **Mailbox** определяет объект Active Directory с включенной поддержкой почты. 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md) <br/> |Определяет SMTP-адрес пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутизацию, используемую для почтового ящика. По умолчанию используется протокол SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Идентификатор](itemid.md) <br/> |Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Определяет запрос на развертывание списка рассылки. <br/> <br/> Ниже приведено выражение XPath для этого элемента:` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит массив получателей элемента.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет массив адресов электронной почты, в которые должны отправляться ответы.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправителя элемента.  <br/> |
|[From](from.md) <br/> |Представляет адрес получателя, от которого было отправлено сообщение.  <br/> |
|[Organizer](organizer.md) <br/> |Представляет организатор собрания.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> | Определяет стандартные папки Microsoft Exchange Server 2007.  <br/><br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Resolution](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
|[длекспансион](dlexpansion.md) <br/> |Содержит массив почтовых ящиков, содержащихся в списке рассылки.  <br/> |
|[Участник](attendee.md) <br/> |Представляет участников и ресурсы для элемента календаря.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Определяет запрос на добавление управляемых папок в почтовый ящик.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Определяет запрос на добавление делегатов в почтовый ящик.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Определяет запрос на получение сведений о делегатах для почтового ящика.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Определяет запрос на удаление делегатов из почтового ящика.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегатов в почтовом ящике.  <br/> |
|[рецеиведби](receivedby.md) <br/> |Описывает делегат в сценарии доступа делегата.  <br/> |
|[рецеиведрепресентинг](receivedrepresenting.md) <br/> |Описывает участника в сценарии доступа делегата.  <br/> |
|[Элемент](member-ex15websvcsotherref.md) <br/> |Представляет члена списка рассылки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Элементы [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) и [ItemId](itemid.md) идентифицируют почтовый ящик или список рассылки. 

Элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) определяет почтовый ящик или список рассылки по SMTP-адресу. 

Элемент [ItemId](itemid.md) идентифицирует почтовый ящик по идентификатору элемента, связанному с определенным почтовым ящиком. 

Элемент [ItemId](itemid.md) нельзя использовать для отправки сообщения в список рассылки или контакт в общедоступной папке "Контакты". Если при попытке отправить сообщение в список рассылки или контакт в общедоступной папке Contacts, будет выдаваться сообщение об ошибке, если оно используется в операции CreateItem, UpdateItem или SendItem. Используйте операцию ExpandDL для получения SMTP-адреса, а затем отправьте сообщение с помощью элемента [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) , а не элемента [ItemId](itemid.md) . 
  
Другой элемент, [Mailbox (Availability)](mailbox-availability.md), предоставляет сведения об операциях обеспечения доступности. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

