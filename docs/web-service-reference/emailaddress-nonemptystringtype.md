---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: Элемент EmailAddress определяет основной SMTP-адрес пользователя почтового ящика.
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762281"
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
|[ActingAs](actingas.md) <br/> |Определяет, как отправляющего вызывающего абонента.  <br/> |
|[Mailbox](mailbox.md) <br/> | Определяет адрес электронной почты полностью разрешенной.  <br/><br/>Ниже приведены некоторые выражения XPath для этого элемента.<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Ниже приведены дополнительные родительские элементы элемента почтового ящика.<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Отправитель](sender.md) <br/>- [От](from.md) <br/>- [Организатор](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Решение](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Участник](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список конференц-залы, адрес электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее SMTP-адрес является обязательным.
  
## <a name="remarks"></a>Замечания

Элемент **EmailAddress** может представлять SMTP или прежних версий Exchange различающееся имя (DN) адресов. Элемент **EmailAddress** является единственным обязательным элементом [почтового ящика](mailbox.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

