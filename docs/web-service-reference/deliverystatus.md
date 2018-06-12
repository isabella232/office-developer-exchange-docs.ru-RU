---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: Элемент DeliveryStatus указывает состояние сообщения.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762064"
---
# <a name="deliverystatus"></a>DeliveryStatus

Элемент **DeliveryStatus** указывает состояние сообщения. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Содержит сведения для одного события для получателя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения для элемента **DeliveryStatus** . 
  
**Значения элементов DeliveryStatus**

|**Значение**|**Описание**|
|:-----|:-----|
|Неуспешный  <br/> |Указывает, что сообщение не было доставлено.  <br/> |
|Ожидание  <br/> |Указывает, что сообщение ожидает утверждения из модератор.  <br/> |
|Доставлено  <br/> |Указывает, что сообщение было доставлено всем указанным получателям.  <br/> |
|Перенесены  <br/> |Указывает, что сообщение перенесено на сервер вне области поиска.  <br/> |
|Чтение  <br/> |Указывает, что сообщение было доставлено и читают получателей.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **DeliveryStatus** был типа **MessageTrackingDeliveryStatusType** в Exchange Server 2010. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

