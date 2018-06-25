---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: Элемент MailboxHoldStatus указывает состояние удержания почтового ящика.
ms.openlocfilehash: 6703c909d0a7b4e83e190807fc3202ecd4699e7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834288"
---
# <a name="mailboxholdstatus"></a>MailboxHoldStatus

Элемент **MailboxHoldStatus** указывает состояние удержания почтового ящика. 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

**MailboxHoldStatusType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Почтовый ящик (string)](mailbox-string.md) | [состояния (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)
  
### <a name="parent-elements"></a>Родительские элементы

[MailboxHoldStatuses](mailboxholdstatuses.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

