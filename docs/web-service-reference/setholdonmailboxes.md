---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: Элемент SetHoldOnMailboxes содержит запрос SetHoldOnMailboxes.
ms.openlocfilehash: 82ebbbdce04a5b70eae790a899ca089e38aa76d9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516377"
---
# <a name="setholdonmailboxes"></a>SetHoldOnMailboxes

Элемент **SetHoldOnMailboxes содержит** запрос **SetHoldOnMailboxes.** 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 **SetHoldOnMailboxesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[ActionType (HoldActionType)](actiontype-holdactiontype.md)  |  [HoldId](holdid.md)  |  [Запрос](query.md)  |  [Почтовые ящики (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  |  [Язык](language.md)  |  [IncludeNonIndexableItems](includenonindexableitems.md)  |  [Deduplication](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
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
   

