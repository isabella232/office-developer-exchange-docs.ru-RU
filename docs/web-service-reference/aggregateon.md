---
title: аггрегатеон
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: Элемент Аггрегатеон представляет свойство, используемое для определения порядка сгруппированных элементов для группового результирующего набора FindItem.
ms.openlocfilehash: 04359c187ef11538d64f8f0d3ea2fe84bc3d048b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463568"
---
# <a name="aggregateon"></a>аггрегатеон

Элемент **аггрегатеон** представляет свойство, используемое для определения порядка сгруппированных элементов для группового результирующего набора FindItem. 
  
- [FindItem](finditem.md)  
- [GroupBy](groupby.md)
- [аггрегатеон](aggregateon.md)
  
```xml
<AggregateOn>
   <FieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <IndexedFieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <ExtendedFieldURI/>
</AggregateOn>
```
 
**аггрегатеонтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Aggregate** <br/> | Указывает максимальное или минимальное значение свойства, определяемого элементом [фиелдури](fielduri.md) , который используется для упорядочивания групп элементов.<br/><br/>Ниже перечислены возможные значения.  <br/><br/>— Минимум  <br/>— Максимум  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет отдельные элементы словаря.  <br/> |
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI, которые необходимо получить, задать или создать.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GroupBy](groupby.md) <br/> |Задает произвольное группирование для запросов FindItem.  <br/> Ниже приведено выражение XPath для этого элемента:`/FindItem/GroupBy` <br/> |
   
## <a name="remarks"></a>Примечания

[Операция FindItem](finditem-operation.md) может возвращать сгруппированные результаты. В сгруппированных результатах все элементы, имеющие одинаковое значение для данного свойства группирования, собираются вместе и представляются как дочерние элементы этой группы. Например, если вы группируете по отправителю, все сообщения электронной почты организуются в отдельные группы в зависимости от того, откуда они находятся: от отправителя A, отправитель б и т. д. Эти группы являются дочерними по отношению к группе отправителей. 
  
Каждая группа в группе отправителей содержит коллекцию элементов, например, фактические сообщения электронной почты, которые были получены от каждого отправителя. Элемент [SortOrder](sortorder.md) можно использовать для сортировки элементов в группе. Однако для сортировки групп на основе значений свойств элемента необходимо использовать агрегацию. 
  
При объединении порядок групп основан на определенном свойстве элементов в группе. При использовании статистической обработки для сортировки элементов в группе необходимо определить свойство репрезентативного типа для сортировки групп. С помощью элемента **аггрегатеон** можно указать свойство репрезентативя. 
  
Когда свойство-представитель идентифицируется, атрибут **Aggregate** используется для указания того, сортируются ли группы в соответствии с максимальным или минимальным значением свойства идентифицировано. Если для атрибута **Aggregate** задано значение Maximum, группы сортируются начиная с самого большого значения свойства **аггрегатеон** . Если для атрибута **Aggregate** задано значение Minimum, группы сортируются начиная с наименьшего значения свойства **аггрегатеон** . 
  
Например, если вы хотите выпустить групповой запрос FindItem, группировка по отправителю, но вы хотите упорядочить группы, чтобы группа с последним сообщением электронной почты появлялась сверху, можно выполнить группировку по отправителю и статистическое значение по дате и времени, полученному с помощью **статистического** атрибута максимума. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере показан сгруппированный запрос и ответ на запрос FindItem. В этом примере показан запрос на возврат элементов, сгруппированных по свойству **ConversationTopic** . Две группы, A и B, возвращаются в убывающем порядке на основе максимального значения свойства [DateTimeReceived](datetimereceived.md) . 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="message:ConversationTopic"/>
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AdditionalProperties>    
      </ItemShape>
      <IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="20" Offset="0"/>
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="message:ConversationTopic"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
<!-- EXAMPLE RESPONSE -->
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>B</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAH=" ChangeKey="CQAAABY" />
                    <t:DateTimeReceived>2006-09-14T23:59:18Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnAHR=" ChangeKey="CQAAAw" />
                    <t:DateTimeReceived>2006-09-15T00:00:24Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnA==" ChangeKey="CQAAJXT" />
                    <t:DateTimeReceived>2006-09-15T00:22:45Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>A</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAAA==" ChangeKey="CQCJNe" />
                    <t:DateTimeReceived>2006-09-14T23:56:12Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQWgAA==" ChangeKey="CQAACJV6" />
                    <t:DateTimeReceived>2006-09-14T23:57:33Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAAA==" ChangeKey="CQA6CJXw" />
                    <t:DateTimeReceived>2006-09-15T00:23:31Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Чтобы отсортировать элементы в группе, используйте элемент [SortOrder](sortorder.md) . 
  
> [!NOTE]
> Для сохранения читаемости были сокращены идентификаторы элементов и ключи изменения. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

