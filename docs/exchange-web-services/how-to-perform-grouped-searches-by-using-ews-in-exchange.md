---
title: Выполнение группового поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Узнайте, как выполнять группировку поисков в управляемом API EWS или приложении EWS, предназначенном для Exchange.
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527931"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a>Выполнение группового поиска с помощью EWS в Exchange

Узнайте, как выполнять группировку поисков в управляемом API EWS или приложении EWS, предназначенном для Exchange.
  
Сгруппированные поиски удобны в том, что они дают вам возможность контролировать организацию результатов поиска. Упорядоченные результаты поиска могут облегчить приложению обработку результатов или отобразить их конечному пользователю в управляемом виде.
  
Группирование заключается в размещении всех элементов в наборе результатов с одинаковым значением определенного поля в группе. Например, вы можете группировать результаты по отправителю, и все элементы из одного лица будут находиться в отдельной группе, а элементы в каждой группе будут отсортированы в соответствии с порядком, указанным в представлении. Сами группы сортируются по статистическому значению, основанному на выбранном поле.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для организации результатов поиска**

|**Задача**|**В управляемом API EWS используйте...**|**В EWS используйте...**|
|:-----|:-----|:-----|
|Упорядочение элементов с одинаковым значением в определенном свойстве в результатах по группам  <br/> |[Группирование. GroupOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |Элемент [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) в качестве дочернего элемента для элемента [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)  <br/> |
|Сортировка элементов в каждой группе по значению в определенном свойстве  <br/> |[Итемвиев. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |Элемент [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx)  <br/> |
|Сортировка групп  <br/> |[GROUPING. Аггрегатеон](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [GROUPING. Аггрегатетипе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [GROUPING. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |Элемент **фиелдури** в качестве дочернего элемента для элемента [аггрегатеон](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)<br/><br/> **Статистический** атрибут для элемента **аггрегатеон**<br/><br/>Атрибут **Order** для элемента **GroupBy**  <br/> |
   
Давайте попробуем пошаговое выполнение.
  
## <a name="group-results-by-a-specific-property"></a>Группировка результатов по определенному свойству
<a name="bk_GroupResults"> </a>

Первый шаг по использованию группирования — выбор свойства или атрибута элементов в хранилище Exchange для группировки по. Управляемый API EWS предоставляет эти свойства классам в соответствующих классах, а EWS представляет их в виде элементов XML. Вы можете выбрать любое свойство, включая настраиваемые или расширенные свойства, но при этом полезно знать, как группируются элементы в зависимости от значения свойства, которое вы выбрали. 

Все элементы, имеющие одинаковое значение в свойстве, выбранном для группировки, будут сгруппированы вместе. Это может показаться очевидным, но это очень важная информация. Обратите внимание на то, что происходит при группировке по свойству даты и времени, например [Item. DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или элемент [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) в EWS. Цель может быть упорядочена по группам, при этом каждая группа содержит элементы из одного дня. Тем не менее, группирование просматривает все значение, которое включает время. 

Конечный результат заключается в том, что элементы будут сгруппированы, так что одновременно получаемые элементы перемещаются в свои группы. Скорее всего, результаты будут отсортированы в большом количестве групп с небольшим количеством элементов в каждой группе. 
  
Чтобы получить набор результатов с небольшим количеством групп и большим количеством элементов в каждой группе, выберите свойство, которое может иметь меньшее количество значений, например [EmailMessage. from](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) или [Item. Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) в управляемом API EWS или [из](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) [категорий](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) в EWS. На следующем рисунке показан список сообщений электронной почты, которые отображаются в папке "Входящие". 
  
**Рис. 1. Сообщения в папке "Входящие"**

![Пример списка сообщений в папке "Входящие".](media/Ex15_GroupedSearch_MsgList.png)
  
Если сгруппировать элементы на рис. 1 по свойству **EmailMessage. from** , то результатом будет две группы, одна для сообщений, отправленных с "счастливых брутто", а другой для сообщений, отправляемых Ольга Даниелс. 
  
**Рис. 2. Сообщения, разделенные на группы на основе свойства From**

![Изображение, на котором показаны сообщения, рассортированные по двум спискам согласно свойству "От".](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a>Сортировка элементов в группах
<a name="bk_SortItems"> </a>

Вы можете управлять сортировкой элементов в каждой группе с помощью свойства [итемвиев. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или элемента [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) в EWS. Один и тот же порядок применяется к каждой группе. Например, если Вы отсортируете элементы на рис. 1 по свойству **Item. DateTimeReceived** , в убывающем порядке, самый последний полученный из них элемент будет первым в группе вероятнее всего, а последний, полученный из Ольга Даниелс, будет первым в группе Ольга Даниелс. С легкостью, группы на рисунке 2 уже отсортированы таким образом. 
  
## <a name="sort-the-groups"></a>Сортировка групп
<a name="bk_SortGroups"> </a>

Теперь, когда ваши группы сопоставлены, последним шагом будет сортировка самих групп. Так как сами группы не имеют определенных значений, процесс группирования должен назначить значение сортировки каждой группе. Это выполняется путем объединения значений определенного свойства в каждой группе, заданного свойством [Group. аггрегатеон](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS, или элементом [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) в качестве дочернего элемента для элемента [аггрегатеон](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) в EWS. Свойство [Group. аггрегатетипе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS (или атрибут **Aggregate** для элемента **аггрегатеон** в EWS) указывает, какое значение из элементов в каждой группе назначается значению сортировки для группы — либо наибольшее значение, либо наименьшее значение. Наконец, порядок сортировки (по убыванию или по возрастанию) задается свойством [Group. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или атрибутом **Order** для элемента [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) в веб-службах EWS. 
  
Например, если группы, показанные на рисунке 2, отсортированы по статистической обработке свойства **Item. DateTimeReceived** с наименьшим значением и сортировка по убыванию, элементы возвращаются в порядке, приведенном на рисунке 3. 
  
**Рис. 3. Сгруппированные результаты поиска с группами, отсортированными по свойству DateTimeReceived**

![Изображение, на котором показан отсортированный список сообщений, сгруппированный по свойству "От", где группы отсортированы по наименьшим времени и дате получения.](media/Ex15_GroupedSearch_Results.png)
  
В следующих разделах показано, как можно забирать группирование и сортировку в коде.
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a>Пример: выполнение группового поиска с помощью управляемого API EWS
<a name="bk_GroupSearchEWSMA"> </a>

Следующие методы управляемого API EWS могут использовать группировку:
  
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
В следующем примере используется метод **ExchangeService. FindItems** ; Тем не менее те же правила и концепции применяются к методу **Folder. FindItems** . В этом примере определен метод под названием **граупитемсбифром** . В качестве параметров в качестве параметров используется объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и объект [веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) . Он запрашивает первые 50 элементов в папке, сгруппированные по свойству **EmailMessage. from** , отсортированному по свойству **Item. DateTimeReceived** в убывающем порядке. Сами группы сортируются по наименьшему значению свойства **Item. DateTimeReceived** в их элементах в порядке убывания. 
  
В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a>Пример: выполнение группового поиска с помощью EWS
<a name="bk_GroupSearchEWS"> </a>

В следующем примере запроса показан запрос [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для первых 50 элементов в папке, сгруппированных по элементу **from** и отсортированный по элементу **DateTimeReceived** в убывающем порядке. Сами группы сортируются по наименьшему значению элемента **DateTimeReceived** в их элементах в убывающем порядке. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Сервер возвращает следующий ответ.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a>Различия версий
<a name="bk_VersionDiffs"> </a>

Версии Exchange, начиная с основной версии 15 и заканчивая сборкой 15.0.775.38, возвращают элементы **группы** (типа **граупедитемстипе**) вместо элементов [граупедитемс](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) в ответе SOAP. Если вы используете управляемый API EWS, это приведет к тому, что коллекция [граупедфиндитемсресултс. итемграупс](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) будет содержать 0 объектов. Если вы используете EWS, элементы **Group** должны обрабатываться как элементы **граупедитемс** . 
  
Версии Exchange, начиная с основной версии 15, возвращают дополнительные элементы **Group** или **граупедитемс** с атрибутом **xsi: nil** со значением **true** в ответе SOAP. Если вы используете управляемый API EWS, эти дополнительные элементы приведут к созданию [сервицексмлдесериализатионексцептион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) . Если вы используете EWS, эти дополнительные элементы следует игнорировать. 
  
## <a name="see-also"></a>См. также

- [Поиск и веб-службах Exchange](search-and-ews-in-exchange.md)    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [Класс GROUPING](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

