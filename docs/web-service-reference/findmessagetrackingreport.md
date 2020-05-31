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
description: Элемент FindMessageTrackingReport указывает условия для типов сообщений, которые требуется найти.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762584"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

Элемент **FindMessageTrackingReport** указывает условия для типов сообщений, которые требуется найти. 
  
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

 **финдмессажетраккингрепортрекуесттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Область действия (Нонемптистрингтипе)](scope-nonemptystringtype.md) <br/> |Указывает, насколько обширным должен быть отчет об отслеживании сообщений.  <br/> |
|[Domain (отслеживание сообщений)](domain-message-tracking.md) <br/> |Содержит имя домена, в котором выполняется отслеживание сообщений.  <br/> |
|[Отправитель (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит контактные данные отправителя сообщения электронной почты.  <br/> |
|[пурпортедсендер](purportedsender.md) <br/> |Содержит контактные данные отправителя предполагаемым сообщения электронной почты.  <br/> |
|[Получатель](recipient.md) <br/> |Содержит адрес электронной почты получателя сообщения.  <br/> |
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Содержит дату и время начала поиска.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Содержит дату и время окончания поиска.  <br/> |
|[MessageId](messageid.md) <br/> |Содержит идентификатор сообщения для поиска.  <br/> |
|[федератедделиверимаилбокс](federateddeliverymailbox.md) <br/> |Содержит имя почтового ящика, в котором было отправлено сообщение, переданное в другом месте.  <br/> |
|[диагностикслевел](diagnosticslevel.md) <br/> |Представляет уровень детализации для диагностических отчетов.  <br/> |
|[серверхинт](serverhint.md) <br/> |Представляет отправную точку для отслеживания сообщения на удаленном сайте или в лесу.  <br/> |
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

