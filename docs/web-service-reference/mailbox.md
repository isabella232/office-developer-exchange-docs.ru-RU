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
description: Элемент почтового ящика идентифицирует почты объект Active Directory.
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834258"
---
# <a name="mailbox"></a>Почтовый ящик

Элемент **почтового ящика** идентифицирует почты объект Active Directory. 
  
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
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя почтового ящика пользователя. Этот элемент является необязательным.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутизации, используемый для почтового ящика. Значение по умолчанию — SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Определяет запрос на разверните список рассылки. <br/> <br/> Ниже приведен выражение XPath для этого элемента.` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит массив получателей элемента.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копии сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет массив адресов электронной почты, на которые будут отправляться ответы.  <br/> |
|[Отправитель](sender.md) <br/> |Идентифицирует отправителя элемента.  <br/> |
|[From](from.md) <br/> |Представляет получателя, у которого было отправлено сообщение.  <br/> |
|[Организатор](organizer.md) <br/> |Представляет организатора собрания.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Идентифицирует папок Microsoft Exchange Server 2007 по умолчанию.  <br/><br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Решение](resolution.md) <br/> |Содержит одного объекта разрешения.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Содержит массив почтовых ящиков, которые содержатся в списке рассылки.  <br/> |
|[Attendee](attendee.md) <br/> |Представляет участников и ресурсов для элемента календаря.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Определяет запрос на добавление управляемых папок почтового ящика.  <br/> |
|[Метод AddDelegate](adddelegate.md) <br/> |Определяет запрос на Добавление делегатов к почтовому ящику.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Определяет запрос на получение сведений о делегатов к почтовому ящику.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Определяет запрос для удаления делегатов из почтового ящика.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегаты в почтовом ящике.  <br/> |
|[Получил](receivedby.md) <br/> |Описывает делегат в сценарии доступа делегата.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Описывает участника в сценарии доступа делегата.  <br/> |
|[Элемент](member-ex15websvcsotherref.md) <br/> |Представляет элемент в список рассылки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Элементы [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) и [ItemId](itemid.md) определение списка рассылки или почтового ящика. 

Элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) определяет почтовый ящик или список рассылки по SMTP-адрес. 

Элемент [ItemId](itemid.md) идентифицирует почтового ящика, идентификатор элемента, который связан с определенного почтового ящика. 

Элемент [ItemId](itemid.md) не может использоваться для отправки сообщения в список рассылки и контактов в папке контактов общедоступной. Ошибка возникает при использовании в ходе операции CreateItem, UpdateItem или SendItem при попытке отправить сообщение в список рассылки или контактов в общей папке контактов. Используйте операцию ExpandDL для получения SMTP-адрес и отправьте сообщение с помощью элемента [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) вместо [ItemId](itemid.md) элемент. 
  
Другого элемента [почтового ящика (доступность)](mailbox-availability.md), сведения о доступности операций. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

