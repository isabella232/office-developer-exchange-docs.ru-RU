---
title: индекседпажеитемвиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: Элемент Индекседпажеитемвиев описывает, как возвращаются страничные беседы или сведения об элементе для операции FindItem или запроса операции FindConversation.
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456915"
---
# <a name="indexedpageitemview"></a>индекседпажеитемвиев

Элемент **индекседпажеитемвиев** описывает, как возвращаются страничные беседы или сведения об элементе для [операции FindItem](finditem-operation.md) или запроса [операции FindConversation](findconversation-operation.md) . 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **индекседпажевиевтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**максентриесретурнед** <br/> |Описывает максимальное число элементов или бесед, возвращаемых в ответе. Этот атрибут является необязательным.  <br/> |
|**Offset** <br/> |Описывает смещение от **басепоинт**. Если **басепоинт** равно "начало", смещение является положительным. Если **басепоинт** равен end, то смещение обрабатывается так, как если бы оно было отрицательным. Это позволяет определить, какой элемент или беседа будет первым доставлен в ответе. Этот атрибут является обязательным.  <br/> |
|**басепоинт** <br/> |Указывает, будет ли страница элементов или бесед начинается с начала или с конца набора элементов или бесед, найденных с помощью условий поиска. Поиск от End всегда выполняет поиск в обратном направлении. Этот атрибут является обязательным.  <br/> |
   
#### <a name="basepoint-attribute"></a>Атрибут Басепоинт

|**Значение**|**Описание**|
|:-----|:-----|
|Слайд  <br/> |Постраничное представление начинается с начала найденного диалога или набора элементов.  <br/> |
|Конец  <br/> |Постраничное представление начинается в конце найденного диалога или набора элементов.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовом ящике.  <br/> |
   
## <a name="remarks"></a>Примечания

Поиск с конца включает перемещение к началу, определяемому смещением. Кроме того, указатель перемещается обратно на число запрошенных записей. Например, если имеется 100 записей, а смещение — 25 из конца, поиск начинается с 75. Если возвращено 10 записей, указатель перемещается обратно в обратное 10 записей в 65 и возвращает записи от 65 до 75. Следующий индекс — 64. Следующее смещение от конца для страницы составляет 100 минус 64, что равно 36. 36 это значение для следующего смещения, начиная с конца, для получения следующей индексированной страницы.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В приведенном ниже примере показан запрос [операции FindItem](finditem-operation.md) . Каждый элемент возвращается с ИДЕНТИФИКАТОРом и темой. В отклике возвращается не более шести элементов, как указано в атрибуте **максентриесретурнед** . Элементы перечислены в порядке возрастания, сгруппированные по важности. Элементы в группе объединяются по темам. 
  
```XML
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
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
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

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[Операция FindConversation](findconversation-operation.md)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

