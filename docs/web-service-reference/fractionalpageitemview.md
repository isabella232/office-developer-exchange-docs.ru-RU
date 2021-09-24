---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: Элемент FractionalPageItemView описывает, где начинается просмотр страницы и максимальное количество элементов, возвращаемых в запросе FindItem.
ms.openlocfilehash: 0d948bad0ba24c4a105be32daa645d1864cb4f3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530248"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

Элемент **FractionalPageItemView** описывает, где начинается просмотр страницы и максимальное количество элементов, возвращаемых в [запросе FindItem.](finditem.md) 
  
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
|**MaxEntriesReturned** <br/> |Определяет максимальное количество результатов, возвращаемых в [ответе FindItem.](finditem.md) Этот атрибут является необязательным. Если этот атрибут не указан, вызов возвращает все доступные элементы.  <br/> |
|**Числитель** <br/> |Представляет числитель дробного смещения с начала набора результатов. Этот атрибут является обязательным. Числитель должен быть равен или меньше, чем знаменатель. Этот атрибут должен представлять неотъемлемое значение, равное нулю или больше нуля.  <br/> Дополнительные сведения см. в разделе Примечание в этой теме.  <br/> |
|**Знаменатель** <br/> |Представляет знаменатель дробного смещения с начала общего числа элементов в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять неотъемлемое значение, которое больше одного.  <br/> Дополнительные сведения см. в разделе Примечание в этой теме.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Заметки

Смещение представления страницы с начала набора найденных элементов описывается фракцией. Фракция, определяемая атрибутами **Numerator** и **Denominator,** описывает, где начинается страница информации. Например, если **Numerator** равен  четырем, а Знаменатель — пяти, страница возвращаемой информации начинается с записи, расположенной на четыре пятых пути к набору результатов. 
  
Если фракция оценивается до нуля, это указывает на начало набора результатов. Если фракция оценивается до одной, это указывает конец набора результатов.
  
> [!NOTE]
> Фракция представляет точки начала страницы, а не количество результатов в наборе результатов, которые будут возвращены. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере показан [запрос FindItem.](finditem.md) Запрос возвращает элементы из результатов поиска, которые начинаются после второй трети всех элементов в наборе результатов. 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Например, если набор результатов содержит девять элементов, просмотр страницы возвращает до 12 элементов, начиная с элемента, найденного в двух третей пути к набору результатов. В этом случае страница начинается с седьмого элемента. Страница будет содержать седьмой, восьмой и девятый элементы. Если значение числитора установлено до нуля, представление страницы возвращает все элементы в наборе результатов до тех пор, пока число меньше атрибута **MaxEntriesReturned.** 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

