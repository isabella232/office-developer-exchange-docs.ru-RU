---
title: MailboxStatisticsSearchResult
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 73499df7-3d50-4e39-895d-6e15dd8b2777
description: Элемент MailboxStatisticsSearchResult содержит результаты поиска по ключевым словам.
ms.openlocfilehash: 5b40622cf15596d7ab8a7fa09c9a1998092c3ee7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834302"
---
# <a name="mailboxstatisticssearchresult"></a>MailboxStatisticsSearchResult

Элемент **MailboxStatisticsSearchResult** содержит результаты поиска по ключевым словам. 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

**MailboxStatisticsSearchResultType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[UserMailbox](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)
  
### <a name="parent-elements"></a>Родительские элементы

[FindMailboxStatisticsByKeywordsResponseMessage](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

