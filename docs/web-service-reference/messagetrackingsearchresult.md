---
title: MessageTrackingSearchResult
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
description: Элемент MessageTrackingSearchResult содержит результат одного сообщения для элемента FindMessageTrackingReportResponse.
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834460"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

Элемент **MessageTrackingSearchResult** содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) . 
  
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
|[Subject](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[Отправитель (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит адрес электронной почты отправителя сообщения.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Содержит контактные данные для утверждения отправителя сообщения электронной почты.  <br/> |
|[Получатели (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Содержит список адресов электронной почты, которые получены этого сообщения.  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |Содержит время, когда сообщение было отправлено.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Содержит внутренний идентификатор сообщения в базе данных транспорта.  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |Содержит имя сервера в лесу, которые ранее принимает сообщение.  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |Содержит имя сервера в лесу, сначала принято сообщение.  <br/> |
|[Свойства (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |Содержит список сообщений, которые соответствуют условиям поиска.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

