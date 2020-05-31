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
ms.openlocfilehash: 7d226de908c4d5a474129e3e1f2344ec1318f538
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835413"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Холдактионтипе (](actiontype-holdactiontype.md) | [холдид](holdid.md) | ) | [почтовые ящики запросов (аррайофстрингстипе)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [инклуденониндексаблеитемс](includenonindexableitems.md) | [дедупликации](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md) [Query](query.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

