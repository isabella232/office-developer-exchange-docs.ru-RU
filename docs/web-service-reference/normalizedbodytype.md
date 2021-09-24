---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: Элемент NormalizedBodyType указывает, возвращается ли нормализуемое тело в текстовом или HTML-формате.
ms.openlocfilehash: 69ce440e30d921b052782af60057fff2d9e9d68f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537568"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

Элемент **NormalizedBodyType** указывает, возвращается ли нормализуемое тело в текстовом или HTML-формате. 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
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

Текстовое значение элемента **NormalizedBodyType** указывает на формат, в который возвращается нормализуемое тело. В таблице ниже перечислены возможные варианты последнего. 
  
****

|**Значение**|**Описание**|
|:-----|:-----|
|Лучший  <br/> |Ответ возвращает самый богатый доступный контент текста тела. Это полезно, если неизвестно, является ли контент текстовым или HTML.  <br/> Возвращенное тело будет текстовым, если сохраненное тело является простым текстом. В противном случае ответ возвращает HTML, если сохраненное тело находится в формате HTML или RTF.  <br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |Ответ возвращает нормализуемую часть тела в качестве HTML.  <br/> |
|Текст  <br/> |Ответ возвращает нормализованное тело в виде простого текста.  <br/> |
   
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

