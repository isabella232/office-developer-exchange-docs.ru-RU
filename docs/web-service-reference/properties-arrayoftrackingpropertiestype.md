---
title: Свойства (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: Элемент Properties содержит список из одного или нескольких свойств отслеживания.
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Свойства (ArrayOfTrackingPropertiesType)

Элемент **Properties** содержит список из одного или нескольких свойств отслеживания. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Свойства (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
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
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Представляет имя и значение пары строк, который используется для создания свойств для отчеты об отслеживании сообщений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Задает условия типам сообщений для поиска.  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Содержит состояние и результат одного запроса [FindMessageTrackingReport операции](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Содержит результат single [GetMessageTrackingReport операции](getmessagetrackingreport-operation.md) запроса.  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Содержит сведения для одного события для получателя.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

