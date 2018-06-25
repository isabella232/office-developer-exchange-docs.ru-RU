---
title: Смещение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: Элемент смещение описание смещения от BaseOffset. Вместе с BaseOffset элемент элемент смещение определяет, является ли время стандартное или летнее время.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834642"
---
# <a name="offset"></a>Смещение

Элемент **смещение** описание смещения от [BaseOffset](baseoffset.md). Вместе с **BaseOffset** элемент элемент **смещение** определяет, является ли время стандартное или летнее время. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Переход на летнее](daylight.md) <br/> |Представляет дату и время изменения времени с летнего времени на стандартное время.  <br/> |
|[Стандартный](standard.md) <br/> |Представляет дату и время изменения времени с летнего времени на стандартное время.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет смещение в формате UTC.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

