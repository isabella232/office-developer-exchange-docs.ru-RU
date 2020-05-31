---
title: деливеристатус
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
description: Элемент Деливеристатус указывает состояние сообщения.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762064"
---
# <a name="deliverystatus"></a>деливеристатус

Элемент **деливеристатус** указывает состояние сообщения. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **мессажетраккингделиверистатустипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[реЦипиенттраккинжевент](recipienttrackingevent.md) <br/> |Содержит сведения об отдельном событии получателя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные текстовые значения для элемента **деливеристатус** . 
  
**Значения элементов Деливеристатус**

|**Значение**|**Описание**|
|:-----|:-----|
|Безуспешных  <br/> |Указывает, что сообщение не было доставлено.  <br/> |
|Pending  <br/> |Указывает, что сообщение ожидает утверждения модератором.  <br/> |
|Отобран  <br/> |Указывает, что сообщение было доставлено всем указанным получателям.  <br/> |
|Скопирован  <br/> |Указывает, что сообщение было передано на сервер за пределами области поиска.  <br/> |
|Чтение  <br/> |Указывает, что сообщение было доставлено и Прочитано получателями.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **деливеристатус** имел тип **Мессажетраккингделиверистатустипе** в Exchange Server 2010. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

