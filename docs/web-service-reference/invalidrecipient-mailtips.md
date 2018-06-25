---
title: InvalidRecipient (подсказки)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: Элемент InvalidRecipient указывает, является ли Недопустимый получатель.
ms.openlocfilehash: addb86ece2be3091ac55a52ee2f16f5c5f72ae41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833958"
---
# <a name="invalidrecipient-mailtips"></a>InvalidRecipient (подсказки)

Элемент **InvalidRecipient** указывает, является ли Недопустимый получатель. 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
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
|[Почтовые подсказки](mailtips.md) <br/> |Представляет значения для различных типов почтовые подсказки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение этого элемента равно **true** , если получатель является недопустимым. Значение равно **false** , если получатель не является недопустимым. 
  
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

