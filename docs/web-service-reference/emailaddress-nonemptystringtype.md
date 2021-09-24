---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: Элемент EmailAddress определяет основной SMTP-адрес пользователя почтового ящика.
ms.openlocfilehash: 8740f6f7f67269de86aaa7383a7ad8f3cdf07a4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512998"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

Элемент **EmailAddress** определяет основной SMTP-адрес пользователя почтового ящика. 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Определяет, кому отправляется вызываемая.  <br/> |
|[Mailbox](mailbox.md) <br/> | Определяет полностью разрешенный адрес электронной почты.  <br/><br/>Ниже приводится несколько выражений XPath к этому элементу:<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Ниже приводится дополнительный родительский элемент элемента почтовых ящиков:<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Отправитель](sender.md) <br/>- [От](from.md) <br/>- [Организатор](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Разрешение](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Участник](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список комнат собраний по адресу электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение, представляю которое представляет smTP-адрес.
  
## <a name="remarks"></a>Заметки

Элемент **EmailAddress** может представлять SMTP или устаревшие Exchange (также известные как DN) адреса. Элемент **EmailAddress** — это единственный необходимый элемент [почтовых ящиков.](mailbox.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

