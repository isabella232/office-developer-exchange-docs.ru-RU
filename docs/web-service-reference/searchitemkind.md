---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: Элемент SearchItemKind указывает тип элементов, которые ищутся для операции FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 93803d181f32d88c30ab0fa9a72bb92f22907dde
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510857"
---
# <a name="searchitemkind"></a>SearchItemKind

Элемент **SearchItemKind** указывает тип элементов, которые ищутся для операции **FindMailboxStatisticsByKeyword.** 
  
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

Текстовое значение элемента **SearchItemKind** — это тип элемента, который будет искать ключевые слова. Следующий список содержит текстовые значения, которые можно использовать в **элементе SearchItemKind.** 
  
- **Email** — указывает, что сообщения электронной почты находятся в поиске ключевых слов. 
    
- **Собрания** . Указывает, что для собраний ищутся ключевые слова. 
    
- **Задачи** . Указывает, что задачи ищут ключевые слова. 
    
- **Примечания** . Указывает, что записи ищутся для ключевых слов. 
    
- **Документы** — указывает на поиск документов по ключевым словам. 
    
- **Журналы** — указывает, что в журналах ищутся ключевые слова. 
    
- **Контакты** — указывает на поиск контактов по ключевым словам. 
    
- **Im** — указывает, что мгновенные сообщения ищут ключевые слова. 
    
- **Голосовая почта** — указывает на поиск голосовой почты по ключевым словам. 
    
- **Факсы** — указывает, что факсы ищут ключевые слова. 
    
- **Сообщения** . Указывает, что в сообщениях ищутся ключевые слова. 
    
- **Rssfeeds** — указывает, что RSS-каналы ищут ключевые слова. 
    
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

