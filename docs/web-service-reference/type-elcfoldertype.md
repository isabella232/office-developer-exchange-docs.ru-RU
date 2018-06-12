---
title: Тип (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Элемент Type указывает тип папки, используемые в политику хранения.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840244"
---
# <a name="type-elcfoldertype"></a>Тип (ElcFolderType)

Элемент **Type** указывает тип папки, используемые в политику хранения. 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Тип** — тип папки, используемые в политику хранения. Текстовое значение может иметь одно из следующих значений, которые представляют тип папки по умолчанию: календарь, контакты, DeletedItems, Черновики, папки "Входящие", JunkEmail, журнала, заметки, Исходящие, папки "Отправленные", задач, все, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, личные, RecoverableItems или NonIpmRoot 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

