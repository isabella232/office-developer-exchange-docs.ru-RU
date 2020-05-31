---
title: нормализедбодитипе
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: Элемент Нормализедбодитипе указывает, возвращается ли нормализованный текст в текстовом формате или HTML-формате.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834554"
---
# <a name="normalizedbodytype"></a>нормализедбодитипе

Элемент **нормализедбодитипе** указывает, возвращается ли нормализованный текст в текстовом формате или HTML-формате. 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 **бодитипереспонсетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[итемшапе](itemshape.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **нормализедбодитипе** указывает формат, в котором возвращается нормализованный текст. В таблице ниже перечислены возможные варианты последнего. 
  
****

|**Значение**|**Описание**|
|:-----|:-----|
|Лучший  <br/> |Ответ будет возвращать наиболее широко доступное содержимое основного текста. Это полезно, если он неизвестен, является ли контент текстовым или HTML-кодом.  <br/> Возвращаемый текст будет содержать текст, если сохраненный текст является обычным текстом. В противном случае ответ вернет HTML, если сохраненный текст имеет формат HTML или RTF.  <br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |Ответ вернет нормализованный текст в формате HTML.  <br/> |
|Текст  <br/> |Ответ вернет нормализованный текст в виде обычного текста.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[итемшапе](itemshape.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

