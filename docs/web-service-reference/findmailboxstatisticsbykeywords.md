---
title: финдмаилбоксстатистиксбикэйвордс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: Элемент Финдмаилбоксстатистиксбикэйвордс указывает запрос на поиск статистики почтовых ящиков по ключевому слову.
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462530"
---
# <a name="findmailboxstatisticsbykeywords"></a>финдмаилбоксстатистиксбикэйвордс

Элемент **финдмаилбоксстатистиксбикэйвордс** указывает запрос на поиск статистики почтовых ящиков по ключевому слову. 
  
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

 **финдмаилбоксстатистиксбикэйвордстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Почтовые ящики (Аррайофусермаилбоксестипе)](mailboxes-arrayofusermailboxestype.md) <br/> |Содержит массив почтовых ящиков, на которые влияет удержание.  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |Задает ключевые слова для поиска.  <br/> |
|[Language](language.md) <br/> |Содержит язык, используемый для поискового запроса.  <br/> |
|[Отправители](senders.md) <br/> |Указывает массив SMTP-адресов.  <br/> |
|[Получатели (Аррайофсмтпаддресстипе)](recipients-arrayofsmtpaddresstype.md) <br/> |Указывает массив получателей сообщения.  <br/> |
|[фромдате](fromdate.md) <br/> |Указывает дату отправки сообщения.  <br/> |
|[тодате](todate.md) <br/> |Указывает дату получения сообщения.  <br/> |
|[мессажетипес](messagetypes.md) <br/> |Указывает массив сообщений для поиска.  <br/> |
|[сеарчдумпстер](searchdumpster.md) <br/> |Указывает, следует ли выполнять поиск в удаленных элементах.  <br/> |
|[инклудеперсоналарчиве](includepersonalarchive.md) <br/> |Указывает, следует ли включать в поиск личный архив.  <br/> |
|[инклудеунсеарчаблеитемс](includeunsearchableitems.md) <br/> |Указывает, следует ли включать элементы, поиск которых невозможен.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

