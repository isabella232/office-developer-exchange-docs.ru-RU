---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: Элемент ConvertHtmlCodePageToUTF8 указывает, преобразуется ли html-тело элемента в UTF8.
ms.openlocfilehash: e43de22b6d8050c14eb18d0fdd5a72f463335189
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545575"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

Элемент **ConvertHtmlCodePageToUTF8 указывает,** преобразуется ли html-тело элемента в UTF8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Определяет набор свойств, возвращаемого в ответ.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текста, **истинное** для элемента **ConvertHtmlCodePageToUTF8,** указывает на то, что htmL-тело преобразуется в UTF8. Ложное **текстовое** значение указывает на то, что htmL-тело не преобразуется в UTF8. 
  
## <a name="remarks"></a>Заметки

Значение true **по** умолчанию используется, если элемент **ConvertHtmlCodePageToUTF8** не указан в запросе. 
  
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

