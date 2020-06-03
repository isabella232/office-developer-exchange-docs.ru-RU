---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: Элемент SetHoldOnMailboxes содержит запрос SetHoldOnMailboxes.
ms.openlocfilehash: c96ff50cb1204d86abc66829e1c5da7124f407f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448354"
---
# <a name="setholdonmailboxes"></a>SetHoldOnMailboxes

Элемент **SetHoldOnMailboxes** содержит запрос **SetHoldOnMailboxes** . 
  
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

 **сесолдонмаилбоксестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Себя [(холдактионтипе)](actiontype-holdactiontype.md)  |  [Холдид](holdid.md)  |  [Query (запрос](query.md)  |  ) [Почтовые ящики (аррайофстрингстипе)](mailboxes-arrayofstringstype.md)  |  [Language (язык](language.md)  |  ) [Инклуденониндексаблеитемс](includenonindexableitems.md)  |  [Дедупликация](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

