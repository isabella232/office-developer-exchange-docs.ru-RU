---
title: маилбоксскопе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: Элемент Маилбоксскопе указывает, следует ли выполнять поиск или получение для беседы в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834293"
---
# <a name="mailboxscope"></a>маилбоксскопе

Элемент **маилбоксскопе** указывает, следует ли выполнять поиск или получение для беседы в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**маилбокссеарчлокатионтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[FindConversation](findconversation.md) | Беседа с FindConversation[GetConversationItems](getconversationitems.md) | [(конверсатионтипе)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **маилбоксскопе** является областью для поиска или получение элементов в беседе в основных почтовых ящиках, архивных почтовых ящиках или как в основном, так и в архивных почтовых ящиках. Текстовое значение **PrimaryOnly** указывает область, предназначенную для основного почтового ящика пользователя. Текстовое значение **ArchiveOnly** указывает область, предназначенную для архивного почтового ящика пользователя. Текстовое значение **ALL** указывает область, которая предназначена как для основного почтового ящика, так и для архивного почтового ящика. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

