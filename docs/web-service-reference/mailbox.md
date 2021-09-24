---
title: Mailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Элемент почтовых ящиков идентифицирует объект Active Directory с поддержкой почты.
ms.openlocfilehash: 8065c0472c3b847d538422aa77cd93f75d919a9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535005"
---
# <a name="mailbox"></a>Mailbox

Элемент **почтовых ящиков** идентифицирует объект Active Directory с поддержкой почты. 
  
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

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет простой адрес протокола передачи почты (SMTP) пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутику, используемую для почтового ящика. По умолчанию значение SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[ItemId](itemid.md) <br/> |Определяет идентификатор элемента контактного или частного списка рассылки для получателей из папки контактов пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Определяет запрос на расширение списка рассылки. <br/> <br/> Ниже приводится выражение XPath к этому элементу: ` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит массив получателей элемента.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые получат копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения слепой копии (BCC) электронной почты.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет массив адресов электронной почты, на которые должны быть отправлены ответы.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправитель элемента.  <br/> |
|[From](from.md) <br/> |Представляет адресата, от которого было отправлено сообщение.  <br/> |
|[Organizer](organizer.md) <br/> |Представляет организатор собрания.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Определяет папки Microsoft Exchange Server 2007 года.  <br/><br/>  Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Решение](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Содержит массив почтовых ящиков, содержащихся в списке рассылки.  <br/> |
|[Attendee](attendee.md) <br/> |Представляет участников и ресурсы для элемента календаря.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Определяет запрос на добавление управляемых папок в почтовый ящик.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Определяет запрос на добавление делегатов в почтовый ящик.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Определяет запрос для получения сведений о делегатах в почтовый ящик.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Определяет запрос на удаление делегатов из почтового ящика.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегатов в почтовом ящике.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Описывает делегата в сценарии доступа делегата.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Описывает основное в сценарии доступа к делегатам.  <br/> |
|[Элемент](member-ex15websvcsotherref.md) <br/> |Представляет члена списка рассылки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Элементы [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) и [ItemId](itemid.md) определяют почтовый ящик или список рассылки. 

Элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) определяет почтовый ящик или список рассылки по smTP-адресу. 

Элемент [ItemId](itemid.md) определяет почтовый ящик идентификатором элемента, который связан с определенным почтовым ящиком. 

Элемент [ItemId](itemid.md) нельзя использовать для отправки сообщения в список рассылки или контакта в папке общедоступных контактов. Ошибка будет выброшена, если она используется в операции CreateItem, UpdateItem или SendItem при попытке отправить сообщение в список рассылки или связаться в общедоступных папках контактов. Используйте операцию ExpandDL для получения smTP-адреса и отправки сообщения с помощью элемента [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) вместо [элемента ItemId.](itemid.md) 
  
Другой элемент— [почтовый ящик (Доступность)](mailbox-availability.md)— предоставляет сведения для операций доступности. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

