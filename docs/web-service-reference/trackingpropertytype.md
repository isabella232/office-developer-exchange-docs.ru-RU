---
title: траккингпропертитипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TrackingPropertyType
api_type:
- schema
ms.assetid: 1d0f219b-1063-4eaa-9d3b-da384a544f89
description: Элемент Траккингпропертитипе представляет собой комбинацию имени и значения строк, которая используется для создания свойств отчетов об отслеживании сообщений.
ms.openlocfilehash: 762c7d364382c3087277651cc01329e3c85df4e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840229"
---
# <a name="trackingpropertytype"></a>траккингпропертитипе

Элемент **траккингпропертитипе** представляет собой комбинацию имени и значения строк, которая используется для создания свойств отчетов об отслеживании сообщений. 
  
[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md)
  
[траккингпропертитипе](trackingpropertytype.md)
  
```xml
<TrackingPropertyType>
   <Name/>
   <Value/>
</TrackingPropertyType>
```

 **траккингпропертитипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (отслеживание сообщений)](name-message-tracking.md) <br/> |Определяет имя свойства отчета "Отслеживание сообщений".  <br/> |
|[Value (отслеживание сообщений)](value-message-tracking.md) <br/> |Определяет значение свойства отчета "Отслеживание сообщений". Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Свойства (Аррайофтраккингпропертиестипе)](properties-arrayoftrackingpropertiestype.md) <br/> |Содержит список одного или нескольких свойств отслеживания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

