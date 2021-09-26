---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: Элемент FindMailboxStatisticsByKeywords указывает запрос на поиск статистики почтовых ящиков по ключевому слову.
ms.openlocfilehash: 3f84b0c3bb2a4a0a2a164b9e9120c3505073417e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546506"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

Элемент **FindMailboxStatisticsByKeywords** указывает запрос на поиск статистики почтовых ящиков по ключевому слову. 
  
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
|[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |Содержит массив почтовых ящиков, затронутых удержанием.  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |Указывает ключевые слова для поиска.  <br/> |
|[Language](language.md) <br/> |Содержит язык, используемый для запроса поиска.  <br/> |
|[Отправители](senders.md) <br/> |Указывает массив SMTP-адресов.  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Указывает массив получателей сообщения.  <br/> |
|[FromDate](fromdate.md) <br/> |Указывает дату, в которую было отправлено сообщение.  <br/> |
|[ToDate](todate.md) <br/> |Указывает дату, когда было получено сообщение.  <br/> |
|[MessageTypes](messagetypes.md) <br/> |Указывает массив сообщений для поиска.  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |Указывает, следует ли искать в удаленных элементов.  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |Указывает, следует ли включать личный архив в поиск.  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |Указывает, следует ли включать элементы, которые нельзя искать.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

