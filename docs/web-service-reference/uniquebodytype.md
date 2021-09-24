---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: Элемент UniqueBodyType указывает, возвращается ли уникальный корпус в текстовом или HTML-формате.
ms.openlocfilehash: a0149e41da24646fdf38a465434bfad3557ece22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520271"
---
# <a name="uniquebodytype"></a>UniqueBodyType

Элемент **UniqueBodyType** указывает, возвращается ли уникальный корпус в текстовом или HTML-формате. 
  
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

Текстовое значение элемента **UniqueBodyType** указывает на формат, в который возвращается уникальное тело. В таблице ниже перечислены возможные варианты последнего. 
  
****

|**Значение**|**Описание**|
|:-----|:-----|
|Лучший  <br/> |Ответ возвращает самый богатый доступный контент текста тела. Это полезно, если неизвестно, является ли контент текстовым или HTML.  <br/> Возвращенное тело будет текстовым, если сохраненное тело является простым текстом. В противном случае ответ возвращает HTML, если сохраненное тело находится в формате HTML или RTF.  <br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |Ответ возвращает уникальный орган в качестве HTML.  <br/> |
|Текст  <br/> |Ответ возвращает уникальный текст в виде простого текста.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[ItemShape](itemshape.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

