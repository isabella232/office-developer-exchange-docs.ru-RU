---
title: реЦипиенттраккинжевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: Элемент РеЦипиенттраккинжевент содержит сведения об отдельном событии получателя.
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465487"
---
# <a name="recipienttrackingevent"></a>реЦипиенттраккинжевент

Элемент **реЦипиенттраккинжевент** содержит сведения об отдельном событии получателя. 
  
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

 **реЦипиенттраккинжевенттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Дата (MessageTracking)](date-messagetracking.md) <br/> |Этот элемент обязательный.  <br/> |
|[Получатель](recipient.md) <br/> |Этот элемент обязательный.  <br/> |
|[деливеристатус](deliverystatus.md) <br/> |Этот элемент обязательный.  <br/> |
|[евентдескриптион](eventdescription.md) <br/> |Этот элемент обязательный.  <br/> |
|[EventData](eventdata.md) <br/> |Этот элемент является необязательным.  <br/> |
|[Сервер (MessageTracking)](server-messagetracking.md) <br/> |Этот элемент обязательный.  <br/> |
|[интерналид](internalid.md) <br/> |Этот элемент обязательный.  <br/> |
|[бккреЦипиент](bccrecipient.md) <br/> |Этот элемент является необязательным.  <br/> |
|[хидденреЦипиент](hiddenrecipient.md) <br/> |Этот элемент является необязательным.  <br/> |
|[уникуепасид](uniquepathid.md) <br/> |Этот элемент является необязательным.  <br/> |
|[рутаддресс](rootaddress.md) <br/> |Этот элемент является необязательным.  <br/> |
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[реЦипиенттраккинжевентс](recipienttrackingevents.md) <br/> |Содержит список одного или нескольких событий отслеживания для получателя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

