---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: Элемент FindMailboxStatisticsByKeywords определяет запрос для поиска по ключевым словам статистики почтового ящика.
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762575"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

Элемент **FindMailboxStatisticsByKeywords** определяет запрос для поиска по ключевым словам статистики почтового ящика. 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 **FindMailboxStatisticsByKeywordsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Почтовые ящики (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |Содержит массив почтовых ящиков, влияет на удержание.  <br/> |
|[Ключевые слова](keywords-ex15websvcsotherref.md) <br/> |Задает ключевые слова для поиска.  <br/> |
|[Language](language.md) <br/> |Содержит язык, используемый для поискового запроса.  <br/> |
|[Отправители](senders.md) <br/> |Указывает массив SMTP-адреса.  <br/> |
|[Получатели (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Указывает массив получателей сообщения.  <br/> |
|[FromDate](fromdate.md) <br/> |Дата отправки сообщения.  <br/> |
|[ToDate](todate.md) <br/> |Указывает дату, которое было получено сообщение.  <br/> |
|[MessageTypes](messagetypes.md) <br/> |Указывает массив сообщения для поиска.  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |Указывает, следует ли выполнять поиск в удаленных элементов.  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |Указывает, следует ли включать в поиск личного архива.  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |Указывает, следует ли включать элементы, которые не удается выполнить поиск.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

