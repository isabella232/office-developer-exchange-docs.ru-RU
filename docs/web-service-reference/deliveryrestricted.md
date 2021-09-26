---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: Элемент DeliveryRestricted указывает, будут ли ограничения на доставку препятствовать сообщению отправительного сообщения до получателя.
ms.openlocfilehash: 1df5254a284989a8ffc02a8c650eaf69b2214583
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545365"
---
# <a name="deliveryrestricted"></a>DeliveryRestricted

Элемент **DeliveryRestricted** указывает, будут ли ограничения на доставку препятствовать сообщению отправительного сообщения до получателя. 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
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
|[Подсказки](mailtips.md) <br/> |Представляет значения для различных типов советов почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение этого  элемента верно, если ограничения на доставку не смогут довести сообщение отправитель до получателя. Значение является **ложным,** если ограничения на доставку не помешают сообщению отправительного сообщения достичь получателя. 
  
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

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

