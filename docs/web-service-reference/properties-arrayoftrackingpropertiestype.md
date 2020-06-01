---
title: Свойства (Аррайофтраккингпропертиестипе)
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
description: Элемент Properties содержит список одного или нескольких свойств отслеживания.
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465634"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Свойства (Аррайофтраккингпропертиестипе)

Элемент **Properties** содержит список одного или нескольких свойств отслеживания. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**аррайофтраккингпропертиестипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[траккингпропертитипе](trackingpropertytype.md) <br/> |Представляет строку имени и значения, используемую для создания свойств отчетов об отслеживании сообщений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Задает условия для типов сообщений, которые требуется найти.  <br/> |
|[финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) <br/> |Содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.  <br/> |
|[жетмессажетраккингрепортреспонсе](getmessagetrackingreportresponse.md) <br/> |Содержит результат одного запроса [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) .  <br/> |
|[реЦипиенттраккинжевент](recipienttrackingevent.md) <br/> |Содержит сведения об отдельном событии получателя.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[мессажетраккингсеарчресулт](messagetrackingsearchresult.md) <br/> |Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

