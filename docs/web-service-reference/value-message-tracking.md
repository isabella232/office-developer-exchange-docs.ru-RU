---
title: Value (отслеживание сообщений)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: Элемент Value представляет свойство для отчета по отслеживанию сообщений.
ms.openlocfilehash: c8aa4f3cc41e76b633ee1b244371de2f5410c944
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513964"
---
# <a name="value-message-tracking"></a>Value (отслеживание сообщений)

Элемент **Value** представляет свойство для отчета по отслеживанию сообщений. 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Представляет имя и пару строк, используемых для создания свойств отчетов по отслеживанию сообщений.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение необязательно.
  
## <a name="remarks"></a>Заметки

Этот элемент может возникать как минимум один раз в [элементе TrackingPropertyType.](trackingpropertytype.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

