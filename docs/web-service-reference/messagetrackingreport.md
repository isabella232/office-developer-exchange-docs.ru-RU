---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: Элемент MessageTrackingReport содержит одно сообщение, которое возвращается в операции GetMessageTrackingReport.
ms.openlocfilehash: fc3e56fbb1bee411fa31751f558f520874133076
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463218"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

Элемент **MessageTrackingReport** содержит одно сообщение, которое возвращается в [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md).
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 **мессажетраккингрепорттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Отправитель (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит контактные данные отправителя сообщения электронной почты.  <br/> |
|[пурпортедсендер](purportedsender.md) <br/> |Содержит контактные данные отправителя предполагаемым сообщения электронной почты.  <br/> |
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[субмиттиме](submittime.md) <br/> |Содержит время, в течение которого сообщение электронной почты было отправлено.  <br/> |
|[оригиналреЦипиентс](originalrecipients.md) <br/> |Содержит список получателей сообщения электронной почты.  <br/> |
|[реЦипиенттраккинжевентс](recipienttrackingevents.md) <br/> |Содержит список одного или нескольких событий отслеживания для получателей.  <br/> |
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетмессажетраккингрепортреспонсе](getmessagetrackingreportresponse.md) <br/> |Содержит результат одного запроса [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

