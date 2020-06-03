---
title: мессажетраккингсеарчресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: Элемент Мессажетраккингсеарчресулт содержит один результат сообщения для элемента Финдмессажетраккингрепортреспонсе.
ms.openlocfilehash: 27e70cd9e11b480ab6bbb9b28275f142da7c76ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466684"
---
# <a name="messagetrackingsearchresult"></a>мессажетраккингсеарчресулт

Элемент **мессажетраккингсеарчресулт** содержит один результат сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) . 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 **финдмессажетраккингсеарчресулттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[Отправитель (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит адрес отправителя сообщения электронной почты.  <br/> |
|[пурпортедсендер](purportedsender.md) <br/> |Содержит контактные данные отправителя предполагаемым сообщения электронной почты.  <br/> |
|[Получатели (АррайофреЦипиентстипе)](recipients-arrayofrecipientstype.md) <br/> |Содержит список адресов электронной почты, которые получили это сообщение.  <br/> |
|[субмиттедтиме](submittedtime.md) <br/> |Содержит время отправки сообщения.  <br/> |
|[мессажетраккингрепортид](messagetrackingreportid.md) <br/> |Содержит внутренний идентификатор, идентифицирующий сообщение в базе данных транспорта.  <br/> |
|[превиаушопсервер](previoushopserver.md) <br/> |Содержит имя сервера в лесу, в котором ранее было принято сообщение.  <br/> |
|[фирссопсервер](firsthopserver.md) <br/> |Содержит имя сервера в лесу, который первым принял сообщение.  <br/> |
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетраккингсеарчресултс](messagetrackingsearchresults.md) <br/> |Содержит список сообщений, которые отвечают условиям поиска.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

