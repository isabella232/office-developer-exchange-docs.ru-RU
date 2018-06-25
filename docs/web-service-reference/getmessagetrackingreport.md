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
description: Элемент GetMessageTrackingReport содержит запрос на операцию GetMessageTrackingReport, чтобы получить полный сообщение отслеживания отчетов для указанного идентификатора.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762854"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

Элемент **GetMessageTrackingReport** содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора. 
  
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

 **GetMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Область (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Указывает, где выполняется поиск. Этот элемент обязательный.  <br/> |
|[Шаблон_отчета](reporttemplate.md) <br/> |Указывает тип отслеживания отчетов для извлечения. Этот элемент обязательный.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Указывает адрес получателя для использования с отчетом по указанным отслеживания. Этот элемент является необязательным.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Задает строку удостоверение, полученное от **FindMessageTrackingReport** операции. Этот элемент обязательный.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Указывает, что пользователь, выполняющий задачи имеет привилегированной роли. Этот элемент является необязательным.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Задает сведения о времени и производительности, который будет использоваться для немедленной отчет об отслеживании. Этот элемент является необязательным.  <br/> |
|[Свойства (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Задает список одного или нескольких свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

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



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

