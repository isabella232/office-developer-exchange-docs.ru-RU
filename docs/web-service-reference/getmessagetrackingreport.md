---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: Элемент GetMessageTrackingReport содержит запрос операции GetMessageTrackingReport, чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762854"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

Элемент **GetMessageTrackingReport** содержит запрос [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора. 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 **жетмессажетраккингрепортрекуесттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Область действия (Нонемптистрингтипе)](scope-nonemptystringtype.md) <br/> |Указывает, где выполнять поиск. Этот элемент обязательный.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Указывает тип отчета отслеживания, который требуется получить. Этот элемент обязательный.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Указывает адрес получателя, который будет использоваться с указанным отчетом об отслеживании. Этот элемент является необязательным.  <br/> |
|[мессажетраккингрепортид](messagetrackingreportid.md) <br/> |Задает строку удостоверения, полученную из операции **FindMessageTrackingReport** . Этот элемент обязательный.  <br/> |
|[ретурнкуеуивентс](returnqueueevents.md) <br/> |Указывает, что пользователь, выполняющий задачу, имеет привилегированную роль. Этот элемент является необязательным.  <br/> |
|[диагностикслевел](diagnosticslevel.md) <br/> |Задает сведения о времени и производительности, которые будут использоваться для формирования отчета об отслеживании. Этот элемент является необязательным.  <br/> |
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Задает список из одного или нескольких свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

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



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

