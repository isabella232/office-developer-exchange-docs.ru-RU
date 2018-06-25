---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: Элемент FractionalPageItemView описывается, где начала страничного представления и максимальное число элементов, возвращаемых в запросе FindItem.
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762650"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

Элемент **FractionalPageItemView** описывается, где начала страничного представления и максимальное число элементов, возвращаемых в запросе [FindItem](finditem.md) . 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Определяет максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) . Этот атрибут является необязательным. Если этот атрибут не указан, вызов вернет все доступные элементы.  <br/> |
|**Числитель** <br/> |Представляет числитель дробная смещения от начала набора результатов. Этот атрибут является обязательным. Числитель должно быть равно или меньше, чем делителя. Этот атрибут должен представлять целочисленное значение, которое равно или больше нуля.  <br/> Дополнительные сведения см.  <br/> |
|**Делителя** <br/> |Представляет делителя дробная смещением от начала общее число элементов в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять целое число, которое больше одного.  <br/> Дополнительные сведения см.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Замечания

Смещение страничного представления от начала набора элементов, обнаруженные описывается функцией. Дроби, которая определяется **числитель** и **делителя** атрибуты, описание которых начинается страницы сведений. К примеру Если **числитель** равно четыре и **делителя** равно пять, страница возвращенных данных начинается запись находится четыре пятых длины способ в наборе результатов. 
  
Если дроби равно нулю, это означает начала набора результатов. Если дроби оценивается как одно, это означает конец набора результатов.
  
> [!NOTE]
> Дроби представляет начальную точку страницы, будут возвращены не число результатов в наборе результатов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере показано [FindItem](finditem.md) запроса. Запрос возвращает элементы из результатов поиска, запустите после второй третья очередь элементы в наборе результатов. 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

Например если результирующий набор содержит девяти элементов, постраничное представление возвращает до 12 элементов, начиная с элемента обнаруженного две трети способ в наборе результатов. В этом случае страница начинается в седьмой элемента. Страница будет содержать седьмой восьмой и девятого элементов. Если числитель нулевое значение, просмотр страницы вернет все элементы в результирующем наборе, до тех пор, пока число меньше, чем атрибут **MaxEntriesReturned** . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindItem Operation](finditem-operation.md)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

