---
title: сеарчмаилбоксесресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: Элемент Сеарчмаилбоксесресулт содержит результат запроса SearchMailboxes.
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466705"
---
# <a name="searchmailboxesresult"></a>сеарчмаилбоксесресулт

Элемент **сеарчмаилбоксесресулт** содержит результат запроса **SearchMailboxes** . 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 **сеарчмаилбоксесресулттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Сеарчкуериес](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Размер (длинный)](size-long.md)  |  [Пажеитемкаунт](pageitemcount.md)  |  [Пажеитемсизе](pageitemsize.md)  |  [Кэйвордстатс](keywordstats.md)  |  [Элементы (аррайофсеарчпревиевитемстипе)](items-arrayofsearchpreviewitemstype.md)  |  [Фаиледмаилбоксес](failedmailboxes.md)  |  [Уточнения](refiners.md)  |  [Маилбоксстатс](mailboxstats.md)
  
### <a name="parent-elements"></a>Родительские элементы

[сеарчмаилбоксесреспонсемессаже](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

