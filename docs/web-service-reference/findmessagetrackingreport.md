---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: Элемент FindMessageTrackingReport указывает критерии для типов сообщений, которые необходимо найти.
ms.openlocfilehash: ec2ab16c6649d85edd86b9438e00ea7cfb9841ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513691"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

Элемент **FindMessageTrackingReport** указывает критерии для типов сообщений, которые необходимо найти. 
  
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
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Представляет, насколько обширным должен быть отчет о отслеживании сообщений.  <br/> |
|[Domain (отслеживание сообщений)](domain-message-tracking.md) <br/> |Содержит имя домена, в котором выполняется отслеживание сообщений.  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит контактные данные отправитель сообщения электронной почты.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Содержит контактные данные предполагаемого отправившего сообщение электронной почты.  <br/> |
|[Получатель](recipient.md) <br/> |Содержит адрес электронной почты получателя сообщения.  <br/> |
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Содержит дату и время начала поиска.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Содержит дату и время окончания поиска.  <br/> |
|[MessageId](messageid.md) <br/> |Содержит идентификатор сообщения для поиска.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Содержит имя почтового ящика, куда было отправлено локальное сообщение.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Представляет уровень детализации диагностических отчетов.  <br/> |
|[ServerHint](serverhint.md) <br/> |Представляет отправную точку для отслеживания сообщения на удаленном сайте или лесу.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или более свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

