---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: Элемент FindMessageTrackingReport указывает критерии для типов сообщений для поиска.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762584"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

Элемент **FindMessageTrackingReport** указывает критерии для типов сообщений для поиска. 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 **FindMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Область (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Представляет, как широкое должны быть отчета отслеживания сообщений.  <br/> |
|[Домен (отслеживания сообщений)](domain-message-tracking.md) <br/> |Содержит имя домена, в котором выполняется отслеживания сообщений.  <br/> |
|[Отправитель (EmailAddressType)](sender-emailaddresstype.md) <br/> |Контактные сведения для отправителя сообщения электронной почты.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Содержит контактные данные для утверждения отправителя сообщения электронной почты.  <br/> |
|[Recipient](recipient.md) <br/> |Содержит адрес электронной почты получателя сообщения.  <br/> |
|[Subject](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Содержит начальную дату и время для поиска.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Содержит конечную дату и время для поиска.  <br/> |
|[Код сообщения](messageid.md) <br/> |Содержит идентификатор сообщения для поиска.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Содержит имя почтового ящика, где нескольких локальных сообщение было отправлено.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Представляет уровень детализации для диагностических отчетов.  <br/> |
|[ServerHint](serverhint.md) <br/> |Представляет собой отправную точку для отслеживания сообщений в удаленной сети или в лесу.  <br/> |
|[Свойства (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

