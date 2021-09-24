---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: Элемент IndexedPageItemView описывает возвращение сведений о разговоре или элементе страницы для операции FindItem или запроса на операцию FindConversation.
ms.openlocfilehash: bf46bdbd457c4f4fa47e6b575d3b797b74f58995
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541128"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

Элемент **IndexedPageItemView** описывает возвращение сведений о разговоре или элементе страницы для операции [FindItem](finditem-operation.md) или [запроса на операцию FindConversation.](findconversation-operation.md) 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное количество элементов или бесед, возвращаемого в ответ. Этот атрибут является необязательным.  <br/> |
|**Offset** <br/> |Описывает смещение из **BasePoint.** Если **BasePoint** равен Началу, смещение является положительным. Если **BasePoint** равен End, смещение обрабатывается так, как если бы оно было отрицательным. При этом определяется, какой элемент или беседа будут первыми доставлены в ответе. Этот атрибут является обязательным.  <br/> |
|**BasePoint** <br/> |Описывает, будет ли страница элементов или бесед начинаться с начала или конца набора элементов или бесед, найденных с помощью критериев поиска. Поиск с конца всегда выполняет поиск в обратном направлении. Этот атрибут является обязательным.  <br/> |
   
#### <a name="basepoint-attribute"></a>Атрибут BasePoint

|**Значение**|**Описание**|
|:-----|:-----|
|Начало  <br/> |Просмотр страницы начинается в начале найденного набора разговоров или элементов.  <br/> |
|End  <br/> |Просмотр страницы начинается в конце найденного набора беседы или элемента.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовом ящике.  <br/> |
   
## <a name="remarks"></a>Заметки

Поиск из конца включает перемещение в источник, идентифицированный смещением. Кроме того, указатель возвращается по количеству запрашиваемой записи. Например, если имеется 100 записей, а смещение — 25 с конца, поиск начинается с 75. Если возвращается 10 записей, указатель перемещается назад, дополнительные 10 записей — 65 и возвращает записи с 65 по 75. Следующий индекс — 64. Следующий смещение из конца страницы — 100 минус 64, что равно 36. 36 — это значение для следующего смещения из конца, чтобы получить следующую индексированную страницу.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показан запрос на операцию [FindItem.](finditem-operation.md) Каждый элемент возвращается с его ID и субъектом. В ответ возвращается не более шести элементов, как указано **атрибутом MaxEntriesReturned.** Элементы перечислены в порядке восходящей группы по значению. Элементы в группе агрегируются по субъекту. 
  
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
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[Операция FindConversation](findconversation-operation.md)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

