---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: Элемент MailboxScope определяет ли поиска или выборки для беседы должны охватывать основной почтовый ящик, архивного почтового ящика или обеих основной и архивирование почтовых ящиков.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834293"
---
# <a name="mailboxscope"></a>MailboxScope

Элемент **MailboxScope** определяет ли поиска или выборки для беседы должны охватывать основной почтовый ящик, архивного почтового ящика или обеих основной и архивирование почтовых ящиков. 
  
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

[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [беседы (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **MailboxScope** — это область для поиска или получение элементов беседы в любом основной почтовых ящиках, в архив почтовых ящиков или основных и архивные почтовые ящики. Текстовое значение **PrimaryOnly** указывает область, предназначенный для основного почтового ящика для пользователя. Текстовое значение **ArchiveOnly** указывает область, предназначенное для архивного почтового ящика для пользователя. Текстовое значение **всех** указывает область, предназначенный для основного почтового ящика и архивного почтового ящика. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

