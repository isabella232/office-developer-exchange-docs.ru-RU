---
title: Properties (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: Элемент Properties содержит список одного или более свойств отслеживания.
ms.openlocfilehash: 8232b94effe3aae5b07be12bdaf1b5e85331938f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542983"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Properties (ArrayOfTrackingPropertiesType)

Элемент **Properties** содержит список одного или более свойств отслеживания. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Представляет имя и пару строк, используемых для создания свойств отчетов по отслеживанию сообщений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Указывает критерии для типов сообщений, которые необходимо найти.  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Содержит состояние и результат одного запроса [операции FindMessageTrackingReport.](findmessagetrackingreport-operation.md)  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запрос на операцию [GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного отчета по отслеживанию сообщений для указанного ID.  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Содержит результат одного запроса [операции GetMessageTrackingReport.](getmessagetrackingreport-operation.md)  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Содержит сведения для одного события для получателя.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Содержит один результат сообщения для [элемента FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md)  <br/> |
   
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

- [Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

