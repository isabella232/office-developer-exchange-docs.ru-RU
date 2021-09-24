---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: Элемент MessageTrackingSearchResult содержит один результат сообщения для элемента FindMessageTrackingReportResponse.
ms.openlocfilehash: 2bd70461b2896d0204b163365d525f76d42bb213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523882"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

Элемент **MessageTrackingSearchResult** содержит один результат сообщения для элемента [FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md) 
  
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

 **FindMessageTrackingSearchResultType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит адрес отправитель сообщения электронной почты.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Содержит контактные данные предполагаемого отправившего сообщение электронной почты.  <br/> |
|[Recipients (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Содержит список адресов электронной почты, которые получили это сообщение.  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |Содержит время отправки сообщения.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Содержит внутренний идентификатор, который идентифицирует сообщение в транспортной базе данных.  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |Содержит имя сервера в лесу, который ранее принял сообщение.  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |Содержит имя сервера в лесу, который впервые принял сообщение.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или более свойств отслеживания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |Содержит список сообщений, которые соответствуют критериям поиска.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

