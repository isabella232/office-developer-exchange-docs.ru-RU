---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: Элемент MessageTrackingReportId представляет сообщение по идентификатору сообщения, организации, в которой было найдено сообщение, серверу, на котором было отправлено сообщение, и внутреннему идентификатору, который однозначно идентифицирует сообщение.
ms.openlocfilehash: 8ed8ddcfe20c9008a208035f2b101fb5241f432d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518262"
---
# <a name="messagetrackingreportid"></a>MessageTrackingReportId

Элемент **MessageTrackingReportId** представляет сообщение по идентификатору сообщения, организации, в которой было найдено сообщение, серверу, на котором было отправлено сообщение, и внутреннему идентификатору, который однозначно идентифицирует сообщение. 
  
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
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запрос на операцию [GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного отчета по отслеживанию сообщений для указанного ID.  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Содержит один результат сообщения для [элемента FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет строку.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

