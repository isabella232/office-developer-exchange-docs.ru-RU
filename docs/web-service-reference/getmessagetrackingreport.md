---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: Элемент GetMessageTrackingReport содержит запрос на операцию GetMessageTrackingReport для получения полного отчета о отслеживании сообщений для указанного ID.
ms.openlocfilehash: cdf4e2c0f17c7d723dc56f30c445bfd527f891a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516981"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

Элемент **GetMessageTrackingReport** содержит запрос на операцию [GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного отчета о отслеживании сообщений для указанного ID. 
  
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
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Указывает, где выполнять поиск. Этот элемент обязательный.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Указывает тип отчета отслеживания для получения. Этот элемент обязательный.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Указывает адрес получателя для использования в указанном отчете отслеживания. Этот элемент является необязательным.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Указывает строку удостоверений, полученную в ходе операции **FindMessageTrackingReport.** Этот элемент обязательный.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Указывает, что лицо, которое работает с этой задачей, имеет привилегированную роль. Этот элемент является необязательным.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Указывает сведения о времени и производительности, которые будут использоваться для получения отчета отслеживания. Этот элемент является необязательным.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Указывает список одного или более свойств отслеживания. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

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



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

