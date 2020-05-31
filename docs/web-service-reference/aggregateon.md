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
ms.openlocfilehash: fe14de23e6a4c90d826200cae927427acfccc3c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761363"
---
# <a name="aggregateon"></a><span data-ttu-id="6470f-103">аггрегатеон</span><span class="sxs-lookup"><span data-stu-id="6470f-103">AggregateOn</span></span>

<span data-ttu-id="6470f-104">Элемент **аггрегатеон** представляет свойство, используемое для определения порядка сгруппированных элементов для группового результирующего набора FindItem.</span><span class="sxs-lookup"><span data-stu-id="6470f-104">The **AggregateOn** element represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span> 
  
- [<span data-ttu-id="6470f-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="6470f-105">FindItem</span></span>](finditem.md)  
- [<span data-ttu-id="6470f-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="6470f-106">GroupBy</span></span>](groupby.md)
- [<span data-ttu-id="6470f-107">аггрегатеон</span><span class="sxs-lookup"><span data-stu-id="6470f-107">AggregateOn</span></span>](aggregateon.md)
  
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
 
<span data-ttu-id="6470f-108">**аггрегатеонтипе**</span><span class="sxs-lookup"><span data-stu-id="6470f-108">**AggregateOnType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6470f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6470f-109">Attributes and elements</span></span>

<span data-ttu-id="6470f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6470f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6470f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6470f-111">Attributes</span></span>

|<span data-ttu-id="6470f-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6470f-112">**Attribute**</span></span>|<span data-ttu-id="6470f-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6470f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6470f-114">**Aggregate**</span><span class="sxs-lookup"><span data-stu-id="6470f-114">**Aggregate**</span></span> <br/> | <span data-ttu-id="6470f-115">Указывает максимальное или минимальное значение свойства, определяемого элементом [фиелдури](fielduri.md) , который используется для упорядочивания групп элементов.</span><span class="sxs-lookup"><span data-stu-id="6470f-115">Indicates the maximum or minimum value of the property identified by the [FieldURI](fielduri.md) element that is used for ordering the groups of items.</span></span><br/><br/><span data-ttu-id="6470f-116">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="6470f-116">The following are the possible values:</span></span>  <br/><br/><span data-ttu-id="6470f-117">— Минимум</span><span class="sxs-lookup"><span data-stu-id="6470f-117">- Minimum</span></span>  <br/><span data-ttu-id="6470f-118">— Максимум</span><span class="sxs-lookup"><span data-stu-id="6470f-118">- Maximum</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6470f-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6470f-119">Child elements</span></span>

|<span data-ttu-id="6470f-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6470f-120">**Element**</span></span>|<span data-ttu-id="6470f-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6470f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6470f-122">фиелдури</span><span class="sxs-lookup"><span data-stu-id="6470f-122">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="6470f-123">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="6470f-123">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="6470f-124">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="6470f-124">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="6470f-125">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="6470f-125">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="6470f-126">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="6470f-126">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="6470f-127">Определяет расширенные свойства MAPI, которые необходимо получить, задать или создать.</span><span class="sxs-lookup"><span data-stu-id="6470f-127">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6470f-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6470f-128">Parent elements</span></span>

|<span data-ttu-id="6470f-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6470f-129">**Element**</span></span>|<span data-ttu-id="6470f-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6470f-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6470f-131">GroupBy</span><span class="sxs-lookup"><span data-stu-id="6470f-131">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="6470f-132">Задает произвольное группирование для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="6470f-132">Specifies arbitrary groupings for FindItem queries.</span></span>  <br/> <span data-ttu-id="6470f-133">Ниже приведено выражение XPath для этого элемента:`/FindItem/GroupBy`</span><span class="sxs-lookup"><span data-stu-id="6470f-133">The following is the XPath expression to this element:  `/FindItem/GroupBy`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6470f-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="6470f-134">Remarks</span></span>

<span data-ttu-id="6470f-135">[Операция FindItem](finditem-operation.md) может возвращать сгруппированные результаты.</span><span class="sxs-lookup"><span data-stu-id="6470f-135">The [FindItem operation](finditem-operation.md) can return grouped results.</span></span> <span data-ttu-id="6470f-136">В сгруппированных результатах все элементы, имеющие одинаковое значение для данного свойства группирования, собираются вместе и представляются как дочерние элементы этой группы.</span><span class="sxs-lookup"><span data-stu-id="6470f-136">Within grouped results, all items that have the same value for a given grouping property are gathered together and presented as children of that group.</span></span> <span data-ttu-id="6470f-137">Например, если вы группируете по отправителю, все сообщения электронной почты организуются в отдельные группы в зависимости от того, откуда они находятся: от отправителя A, отправитель б и т. д.</span><span class="sxs-lookup"><span data-stu-id="6470f-137">For example, if you group by sender, all e-mails are organized into separate groups based on whether they are from sender A, sender B, and so on.</span></span> <span data-ttu-id="6470f-138">Эти группы являются дочерними по отношению к группе отправителей.</span><span class="sxs-lookup"><span data-stu-id="6470f-138">These groups are children of the sender group.</span></span> 
  
<span data-ttu-id="6470f-139">Каждая группа в группе отправителей содержит коллекцию элементов, например, фактические сообщения электронной почты, которые были получены от каждого отправителя.</span><span class="sxs-lookup"><span data-stu-id="6470f-139">Each of the groups within the sender group contains a collection of items, such as the actual e-mails that came from each sender.</span></span> <span data-ttu-id="6470f-140">Элемент [SortOrder](sortorder.md) можно использовать для сортировки элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="6470f-140">You can use the [SortOrder](sortorder.md) element to sort the items within a group.</span></span> <span data-ttu-id="6470f-141">Однако для сортировки групп на основе значений свойств элемента необходимо использовать агрегацию.</span><span class="sxs-lookup"><span data-stu-id="6470f-141">To sort the groups based on an item's property values, however, you must use aggregation.</span></span> 
  
<span data-ttu-id="6470f-142">При объединении порядок групп основан на определенном свойстве элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="6470f-142">With aggregation, the order of groups is based on a specific property of the items within the group.</span></span> <span data-ttu-id="6470f-143">При использовании статистической обработки для сортировки элементов в группе необходимо определить свойство репрезентативного типа для сортировки групп.</span><span class="sxs-lookup"><span data-stu-id="6470f-143">When you use aggregation to sort items within a group, you must identify a representative property by which to sort the groups.</span></span> <span data-ttu-id="6470f-144">С помощью элемента **аггрегатеон** можно указать свойство репрезентативя.</span><span class="sxs-lookup"><span data-stu-id="6470f-144">You can use the **AggregateOn** element to specify the representative property.</span></span> 
  
<span data-ttu-id="6470f-145">Когда свойство-представитель идентифицируется, атрибут **Aggregate** используется для указания того, сортируются ли группы в соответствии с максимальным или минимальным значением свойства идентифицировано.</span><span class="sxs-lookup"><span data-stu-id="6470f-145">When a representative property is identified, the **Aggregate** attribute is used to indicate whether the groups are sorted according to the maximum or the minimum value of the identified property.</span></span> <span data-ttu-id="6470f-146">Если для атрибута **Aggregate** задано значение Maximum, группы сортируются начиная с самого большого значения свойства **аггрегатеон** .</span><span class="sxs-lookup"><span data-stu-id="6470f-146">If the **Aggregate** attribute is set to Maximum, the groups are sorted beginning with the largest value for the **AggregateOn** property.</span></span> <span data-ttu-id="6470f-147">Если для атрибута **Aggregate** задано значение Minimum, группы сортируются начиная с наименьшего значения свойства **аггрегатеон** .</span><span class="sxs-lookup"><span data-stu-id="6470f-147">If the **Aggregate** attribute is set to Minimum, the groups are sorted beginning with the smallest value for the **AggregateOn** property.</span></span> 
  
<span data-ttu-id="6470f-148">Например, если вы хотите выпустить групповой запрос FindItem, группировка по отправителю, но вы хотите упорядочить группы, чтобы группа с последним сообщением электронной почты появлялась сверху, можно выполнить группировку по отправителю и статистическое значение по дате и времени, полученному с помощью **статистического** атрибута максимума.</span><span class="sxs-lookup"><span data-stu-id="6470f-148">For example, if you want to issue a FindItem grouped query, grouping by sender, but you want to order the groups so that the group with the most recent e-mail message is on top, you can group by sender and aggregate on date/time received with an **Aggregate** attribute of Maximum.</span></span> 
  
<span data-ttu-id="6470f-149">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6470f-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6470f-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6470f-150">Example</span></span>

<span data-ttu-id="6470f-151">В приведенном ниже примере показан сгруппированный запрос и ответ на запрос FindItem.</span><span class="sxs-lookup"><span data-stu-id="6470f-151">The following example shows a grouped FindItem request and response.</span></span> <span data-ttu-id="6470f-152">В этом примере показан запрос на возврат элементов, сгруппированных по свойству **ConversationTopic** .</span><span class="sxs-lookup"><span data-stu-id="6470f-152">The example shows a request to return items grouped by the **ConversationTopic** property.</span></span> <span data-ttu-id="6470f-153">Две группы, A и B, возвращаются в убывающем порядке на основе максимального значения свойства [DateTimeReceived](datetimereceived.md) .</span><span class="sxs-lookup"><span data-stu-id="6470f-153">Two groups, A and B, are returned in descending order based on the maximum value of the [DateTimeReceived](datetimereceived.md) property.</span></span> 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="6470f-154">Чтобы отсортировать элементы в группе, используйте элемент [SortOrder](sortorder.md) .</span><span class="sxs-lookup"><span data-stu-id="6470f-154">To sort the items in a group, use the [SortOrder](sortorder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6470f-155">Для сохранения читаемости были сокращены идентификаторы элементов и ключи изменения.</span><span class="sxs-lookup"><span data-stu-id="6470f-155">The item identifiers and change keys have been shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6470f-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6470f-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6470f-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6470f-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6470f-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6470f-158">Schema Name</span></span>  <br/> |<span data-ttu-id="6470f-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6470f-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="6470f-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6470f-160">Validation File</span></span>  <br/> |<span data-ttu-id="6470f-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6470f-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6470f-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6470f-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="6470f-163">False</span><span class="sxs-lookup"><span data-stu-id="6470f-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6470f-164">См. также</span><span class="sxs-lookup"><span data-stu-id="6470f-164">See also</span></span>

- [<span data-ttu-id="6470f-165">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="6470f-165">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="6470f-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6470f-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6470f-167">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="6470f-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

