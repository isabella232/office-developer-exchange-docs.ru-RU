---
title: фрактионалпажеитемвиев
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
description: Элемент Фрактионалпажеитемвиев описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе FindItem.
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762650"
---
# <a name="fractionalpageitemview"></a>фрактионалпажеитемвиев

Элемент **фрактионалпажеитемвиев** описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе [FindItem](finditem.md) . 
  
[FindItem](finditem.md)
  
[фрактионалпажеитемвиев](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **фрактионалпажевиевтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**максентриесретурнед** <br/> |Определяет максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) . Этот атрибут является необязательным. Если этот атрибут не указан, вызов возвратит все доступные элементы.  <br/> |
|**Числител** <br/> |Представляет числитель дробного смещения от начала набора результатов. Этот атрибут является обязательным. Числитель должен быть равен или меньше знаменателя. Этот атрибут должен представлять целое значение, равное или больше 0.  <br/> Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.  <br/> |
|**Подробно** <br/> |Представляет знаменатель дробного смещения от начала общего числа элементов в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять целое значение больше единицы.  <br/> Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Примечания

Смещение страничного представления от начала набора найденных элементов описывается с помощью дробной части. Дробь, которая определяется атрибутами **числительного** и **знаменателя** , описывает, где начинается страница данных. Например, если **числитель** равен четырем и **знаменателю** равен 5, то страница возвращаемой информации начинается с записи, расположенной четырьмя-пятогоями способа в наборе результатов. 
  
Если дробная дробь имеет нулевое значение, значит начало набора результатов. Если дробь имеет значение 1, то отображается конец набора результатов.
  
> [!NOTE]
> Дробь представляет начальную точку страницы, а не количество результатов, возвращаемых в наборе результатов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере показан запрос [FindItem](finditem.md) . Запрос возвращает элементы из результатов поиска, которые начинаются после второй третьей части всех элементов в наборе результатов. 
  
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

Например, если результирующий набор содержит девять элементов, то Постраничное представление будет возвращать до 12 элементов, начиная с элемента, который находится в двух третьихх в наборе результатов. В этом случае страница начинается с седьмого элемента. На странице будут содержаться седьмые, восьмые и девятые элементы. Если для числителя задано значение 0, то представление страницы будет возвращать все элементы в наборе результатов, если оно меньше, чем значение атрибута **максентриесретурнед** . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

