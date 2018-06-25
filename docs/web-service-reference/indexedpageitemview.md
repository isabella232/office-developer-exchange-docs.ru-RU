---
title: IndexedPageItemView
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
description: Элемент IndexedPageItemView описывает как выгружаемый беседы или элемент возвращается информация для операции FindItem или FindConversation операции запроса.
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833919"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

Элемент **IndexedPageItemView** описывает как выгружаемый беседы или элемент возвращается информация для [операции FindItem](finditem-operation.md) или [FindConversation операции](findconversation-operation.md) запроса. 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное число элементов или бесед, чтобы вернуться в ответе. Этот атрибут является необязательным.  <br/> |
|**Смещение** <br/> |Описание смещения от **Базисная точка**. Если **Базисная точка** равна начала, смещение является положительным. Если **Базисная точка** равна End, смещение обрабатывается как если бы он был отрицательным. Этот элемент определяет или беседы будет в первую очередь доставки в ответе. Этот атрибут является обязательным.  <br/> |
|**Базисная точка** <br/> |Описывает ли страница элементов или бесед начинается с самого начала или окончания набора элементов или бесед, найденных с помощью условия поиска. При поиске с конца всегда ищет в обратном направлении. Этот атрибут является обязательным.  <br/> |
   
#### <a name="basepoint-attribute"></a>Атрибут Базисная точка

|**Значение**|**Описание**|
|:-----|:-----|
|Начало  <br/> |Постраничное представление начинается с начала обнаруженного набора беседы или элемента.  <br/> |
|End  <br/> |Постраничное представление начинается в конце обнаруженного set беседы или элемента.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовый ящик.  <br/> |
   
## <a name="remarks"></a>Замечания

Поиск с конца включает в себя перемещение происхождения, определяемую средством смещение. Кроме того указатель возвращается назад на число запрошенных записей. Например если существует 100 записей и смещение равно 25 с конца, поиск начинается с 75. Если будет возвращено 10 записей, указатель мыши перемещается назад дополнительные 10 записывает 65 и возвращает записи 65 через 75. Следующий индекс — 64. Далее смещение с конца страницы равно 100 минус 64, которое равно 36. 36 — это значение следующего смещения от конца для получения следующей страницы индексированных.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показано [FindItem операции](finditem-operation.md) запроса. Каждый элемент возвращается вместе с его идентификатор и темы. Не более шести элементы будут возвращены в ответ, как указано в атрибуте **MaxEntriesReturned** . Элементы, перечислены в восходящем порядке, сгруппированные по важности. Элементы в группе объединенные по теме. 
  
```XML
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindItem Operation](finditem-operation.md)
  
[FindConversation Operation](findconversation-operation.md)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

