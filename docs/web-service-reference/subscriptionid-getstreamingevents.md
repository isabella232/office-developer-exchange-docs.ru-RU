---
title: SubscriptionId (GetStreamingEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f86c178-2311-4844-82db-c2a0e469d116
description: Элемент SubscriptionId представляет идентификатор для потоковой передачи подписки.
ms.openlocfilehash: eb451e611c4922fa3b9cff7edec54dfb8260f5f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840106"
---
# <a name="subscriptionid-getstreamingevents"></a>SubscriptionId (GetStreamingEvents)

Элемент **SubscriptionId** представляет идентификатор для потоковой передачи подписки. 
  
```XML
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |Представляет операцию, используемый клиентами для потоковой передачи уведомления запросов от сервера.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение является идентификатором GUID.
  
## <a name="remarks"></a>Замечания

Идентификатор GUID, представляющий идентификатор подписки формируется на сервере клиентского доступа при создании подписки.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetStreamingEvents](getstreamingevents-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

