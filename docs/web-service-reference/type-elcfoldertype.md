---
title: Тип (Елкфолдертипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Элемент Type указывает тип папки, используемой в политике хранения.
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465109"
---
# <a name="type-elcfoldertype"></a>Тип (Елкфолдертипе)

Элемент **Type** указывает тип папки, используемой в политике хранения. 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **елкфолдертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Retentionpolicytag используется](retentionpolicytag.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Type** — это тип папки, используемый в политике хранения. Текстовое значение может быть одним из следующих значений, которые представляют тип папки по умолчанию: Calendar, Contacts, DeletedItems, Черновики, Inbox, Жункемаил, журнал, Notes, Inbox, SentItems, Tasks, ALL, Манажедкустомфолдер, Рсссубскриптионс, СинЦиссуес, ConversationHistory, Personal, RecoverableItems или Нонипмрут 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

