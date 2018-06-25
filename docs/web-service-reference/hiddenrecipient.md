---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: Элемент HiddenRecipient указывает, что получатель был добавлен политикой организации, должны быть скрыты от непривилегированным пользователям.
ms.openlocfilehash: 73b2e3e39c675cf3e2bc56105b1e76009d4a2451
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833810"
---
# <a name="hiddenrecipient"></a>HiddenRecipient

Элемент **HiddenRecipient** указывает, что получатель был добавлен политикой организации, должны быть скрыты от непривилегированным пользователям. 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 **Boolean**
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

Этот элемент может быть значение **true** или **false**. Значение **true** указывает, что пользователь был добавлен политикой организации; значение **false** указывает, что пользователь не был добавлен политикой организации. 
  
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



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

