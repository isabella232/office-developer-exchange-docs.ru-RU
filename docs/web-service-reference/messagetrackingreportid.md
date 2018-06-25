---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: Элемент MessageTrackingReportId представляет сообщение, его идентификатор сообщения, организации, где сообщение об ошибке, сервер, на котором было отправлено сообщение и внутренний идентификатор, который уникальным образом определяет сообщение.
ms.openlocfilehash: 8e0d85b203b8a34acedb5f6b9fe46359d5e0b97c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834456"
---
# <a name="messagetrackingreportid"></a>MessageTrackingReportId

Элемент **MessageTrackingReportId** представляет сообщение, его идентификатор сообщения, организации, где сообщение об ошибке, сервер, на котором было отправлено сообщение и внутренний идентификатор, который уникальным образом определяет сообщение. 
  
```XML
<MessageTrackingReportId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее строку является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

