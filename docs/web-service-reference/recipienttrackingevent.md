---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: Элемент RecipientTrackingEvent содержит сведения для одного события для получателя.
ms.openlocfilehash: 30d9cd4ca075fda9607b191f576cac1b7a529988
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525765"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

Элемент **RecipientTrackingEvent** содержит сведения для одного события для получателя. 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 **RecipientTrackingEventType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Date (MessageTracking)](date-messagetracking.md) <br/> |Этот элемент обязательный.  <br/> |
|[Получатель](recipient.md) <br/> |Этот элемент обязательный.  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |Этот элемент обязательный.  <br/> |
|[EventDescription](eventdescription.md) <br/> |Этот элемент обязательный.  <br/> |
|[EventData](eventdata.md) <br/> |Этот элемент является необязательным.  <br/> |
|[Server (MessageTracking)](server-messagetracking.md) <br/> |Этот элемент обязательный.  <br/> |
|[InternalId](internalid.md) <br/> |Этот элемент обязательный.  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |Этот элемент является необязательным.  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |Этот элемент является необязательным.  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |Этот элемент является необязательным.  <br/> |
|[RootAddress](rootaddress.md) <br/> |Этот элемент является необязательным.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Содержит список одного или более событий отслеживания для получателя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

