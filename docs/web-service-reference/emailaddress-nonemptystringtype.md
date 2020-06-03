---
title: EmailAddress (Нонемптистрингтипе)
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
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463134"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (Нонемптистрингтипе)

Элемент **EmailAddress** определяет основной SMTP-адрес пользователя почтового ящика. 
  
```XML
<EmailAddress/>
```

 **нонемптистрингтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[актингас](actingas.md) <br/> |Указывает, кому отправляется вызывающий абонент.  <br/> |
|[Mailbox](mailbox.md) <br/> | Определяет полностью разрешенный адрес электронной почты.  <br/><br/>Ниже приведено несколько выражений XPath для этого элемента:<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Ниже приведены дополнительные родительские элементы элемента Mailbox:<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Организатор](sender.md) <br/>- [От](from.md) <br/>- [Коллекции](organizer.md) <br/>- [дистингуишедфолдерид](distinguishedfolderid.md) <br/>- [Решение](resolution.md) <br/>- [длекспансион](dlexpansion.md) <br/>- [Участника](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список комнат для собраний по адресу электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение, представляющее SMTP-адрес.
  
## <a name="remarks"></a>Примечания

Элемент **EmailAddress** может представлять SMTP-адреса или адреса прежнего различающегося имени Exchange (также известные как DN). Элементом **EmailAddress** является единственный обязательный элемент [почтового ящика](mailbox.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

