---
title: SetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d61de0f3-24e0-434a-946a-c53d393b7d04
description: Элемент SetHoldOnMailboxesResponseMessage указывает сообщение ответа на запрос SetHoldOnMailboxes.
ms.openlocfilehash: 9fbfde90f2a3b9fc90e602fd3bd90289e1041f39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545988"
---
# <a name="setholdonmailboxesresponsemessage"></a>SetHoldOnMailboxesResponseMessage

Элемент **SetHoldOnMailboxesResponseMessage** указывает сообщение ответа на запрос **SetHoldOnMailboxes.** 
  
```XML
<SetHoldOnMailboxesResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponseMessage>
```

 **SetHoldOnMailboxesResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [ОписательныйLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [MailboxHoldResult](mailboxholdresult.md)
  
### <a name="parent-elements"></a>Родительские элементы

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

