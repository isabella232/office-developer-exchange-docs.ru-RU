---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: Элемент SearchItemKind указывает тип элементов, которые осуществляется поиск FindMailboxStatisticsByKeyword операции.
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835298"
---
# <a name="searchitemkind"></a>SearchItemKind

Элемент **SearchItemKind** указывает тип элементов, которые осуществляется поиск **FindMailboxStatisticsByKeyword** операции. 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SearchItemKind** — это тип элемента, который выполняется поиск по ключевым словам. Следующий список содержит текстовые значения, которые могут использоваться в элементе **SearchItemKind** . 
  
- **Электронной почты** — указывает, что поиск сообщений электронной почты, выполняется ключевые слова. 
    
- **Собрания** — указывает, что собраний выполняется поиск по ключевым словам. 
    
- **Задачи** — указывает, что задачи выполняется поиск по ключевым словам. 
    
- **Примечания** — указывает, что notes выполняется поиск по ключевым словам. 
    
- **Документы** - указывает, что поиск документов, выполняется ключевые слова. 
    
- **Журналы** — указывает, что журналы выполняется поиск по ключевым словам. 
    
- **Контакты** — указывает, что контакты выполняется поиск по ключевым словам. 
    
- **Обмен мгновенными сообщениями** — указывает, что мгновенных сообщений выполняется поиск по ключевым словам. 
    
- **Голосовая почта** — указывает, что сообщения голосовой почты выполняется поиск по ключевым словам. 
    
- **Факсы** - указывает, что факсы выполняется поиск по ключевым словам. 
    
- **Публикации, посвященные** - указывает, что публикации выполняется поиск по ключевым словам. 
    
- **Rssfeeds** — указывает, что RSS-каналы выполняется поиск по ключевым словам. 
    
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
   

