---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: Элемент MessageTrackingReport содержит одно сообщение, которое возвращается в операции GetMessageTrackingReport.
ms.openlocfilehash: aa55bb9e4f81a4cc0586d7258720aefd743923fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539355"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

Элемент **MessageTrackingReport содержит** одно сообщение, которое возвращается в операции [GetMessageTrackingReport.](getmessagetrackingreport-operation.md)
  
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

 **MessageTrackingReportType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Содержит контактные данные отправитель сообщения электронной почты.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Содержит контактные данные предполагаемого отправившего сообщение электронной почты.  <br/> |
|[Тема](subject.md) <br/> |Содержит тему сообщения электронной почты.  <br/> |
|[SubmitTime](submittime.md) <br/> |Содержит время отправки сообщения электронной почты.  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |Содержит список получателей сообщения электронной почты.  <br/> |
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Содержит список одного или более событий отслеживания для получателей.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или более свойств отслеживания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Содержит результат одного запроса [операции GetMessageTrackingReport.](getmessagetrackingreport-operation.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

