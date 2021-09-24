---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: Элемент MailboxScope определяет, должен ли поиск или извлечение для беседы охватывать основной почтовый ящик, архивный почтовый ящик или основной и архивный почтовый ящик.
ms.openlocfilehash: 705c72ae2aefbb16599f392eb712d080668490b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522882"
---
# <a name="mailboxscope"></a>MailboxScope

Элемент **MailboxScope** определяет, должен ли поиск или извлечение для беседы охватывать основной почтовый ящик, архивный почтовый ящик или основной и архивный почтовый ящик. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[FindConversation](findconversation.md)  |  [GetConversationItems](getconversationitems.md)  |  [Беседа (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **MailboxScope** — это область поиска или получения элементов в беседе между основными почтовыми ящиками, архивными почтовыми ящиками или первичными и архивными почтовыми ящиками. Текстовое значение **PrimaryOnly указывает** область, которая ориентирована на основной почтовый ящик для пользователя. Текстовое значение **ArchiveOnly указывает** область, которая нацелена на почтовый ящик архива для пользователя. Текстовое значение **All** указывает область, которая ориентирована как на основной почтовый ящик, так и на архивный почтовый ящик. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

