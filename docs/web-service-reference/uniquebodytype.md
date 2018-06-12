---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: Элемент UniqueBodyType указывает, возвращается ли уникальный текст в формате HTML или текст.
ms.openlocfilehash: c6eb4ec4e39a0c5355775a635db4c63efc666820
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840284"
---
# <a name="uniquebodytype"></a>UniqueBodyType

Элемент **UniqueBodyType** указывает, возвращается ли уникальный текст в формате HTML или текст. 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **UniqueBodyType** указывает, что формат уникальный body, возвращается в. В таблице ниже перечислены возможные варианты последнего. 
  
****

|**Значение**|**Описание**|
|:-----|:-----|
|Рекомендации  <br/> |В ответе будут возвращены содержательности доступное содержимое основного текста. Это полезно, если не известно, является ли содержимое текста или HTML.  <br/> Возвращаемое значение body будет текст основному сохраненных обычного текста. В противном случае ответ вернет HTML Если сохраненные текст в формате HTML или RTF.  <br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |В ответе возвращается уникальное body как HTML.  <br/> |
|Text  <br/> |В ответе возвращается уникальное body как обычный текст.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[ItemShape](itemshape.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

