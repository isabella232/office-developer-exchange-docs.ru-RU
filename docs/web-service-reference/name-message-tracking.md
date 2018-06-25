---
title: Имя (отслеживания сообщений)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: Элемент Name представляет имя свойства для отслеживания отчетов сообщений.
ms.openlocfilehash: c905df03842de47b2bcbd62897aa9a8cf464cc6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834501"
---
# <a name="name-message-tracking"></a>Имя (отслеживания сообщений)

Элемент **Name** представляет имя свойства для отслеживания отчетов сообщений. 
  
```xml
<Name/>
```

**Строка**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Представляет имя и значение пары строк, который используется для создания свойств для отчеты об отслеживании сообщений.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Этот элемент может возникнуть только один раз в элементе [TrackingPropertyType](trackingpropertytype.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

