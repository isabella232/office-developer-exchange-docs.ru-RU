---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: Элемент FractionalPageFolderView описывается, где начала страничного представления и максимальное число папок, возвращаемых в запросе FindFolder.
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762647"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

Элемент **FractionalPageFolderView** описывается, где начала страничного представления и максимальное число папок, возвращаемых в запросе [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Определяет максимальное число результатов, возвращаемых в ответе [FindFolder](findfolder.md) . Этот атрибут является необязательным.  <br/> |
|**Числитель** <br/> |Представляет числитель дробная смещения от начала набора результатов. Этот атрибут является обязательным. Числитель должно быть равно или меньше, чем делителя. Этот атрибут должен представлять целочисленное значение, которое равно или больше нуля. Дополнительные сведения см.  <br/> |
|**Делителя** <br/> |Представляет делителя дробная смещением от начала общее число папок в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять целое число, которое больше одного. Дополнительные сведения см.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос для определения папок в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Замечания

Смещение страничного представления от начала набора папок, обнаруженного описывается функцией. Дроби, которая определяется **числитель** и **делителя** атрибуты, описание которых начинается страницы сведений. К примеру Если **числитель** равно четыре и **делителя** равно пять, страница возвращенных данных начинается запись находится четыре пятых длины способ в наборе результатов. 
  
Если дроби равно нулю, это означает начала набора результатов. Если дроби оценивается как одно, это означает конец набора результатов.
  
> [!NOTE]
> Дроби представляет начальную точку страницы, будут возвращены не число результатов в наборе результатов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindFolder Operation](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

