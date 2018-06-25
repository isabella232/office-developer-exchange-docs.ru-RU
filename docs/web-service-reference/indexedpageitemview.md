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
# <a name="indexedpageitemview"></a><span data-ttu-id="38018-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="38018-103">IndexedPageItemView</span></span>

<span data-ttu-id="38018-104">Элемент **IndexedPageItemView** описывает как выгружаемый беседы или элемент возвращается информация для [операции FindItem](finditem-operation.md) или [FindConversation операции](findconversation-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="38018-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="38018-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="38018-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38018-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38018-106">Attributes and elements</span></span>

<span data-ttu-id="38018-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="38018-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38018-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38018-108">Attributes</span></span>

|<span data-ttu-id="38018-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="38018-109">**Attribute**</span></span>|<span data-ttu-id="38018-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38018-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38018-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="38018-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="38018-112">Описывает максимальное число элементов или бесед, чтобы вернуться в ответе.</span><span class="sxs-lookup"><span data-stu-id="38018-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="38018-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="38018-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="38018-114">**Смещение**</span><span class="sxs-lookup"><span data-stu-id="38018-114">**Offset**</span></span> <br/> |<span data-ttu-id="38018-115">Описание смещения от **Базисная точка**.</span><span class="sxs-lookup"><span data-stu-id="38018-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="38018-116">Если **Базисная точка** равна начала, смещение является положительным.</span><span class="sxs-lookup"><span data-stu-id="38018-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="38018-117">Если **Базисная точка** равна End, смещение обрабатывается как если бы он был отрицательным.</span><span class="sxs-lookup"><span data-stu-id="38018-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="38018-118">Этот элемент определяет или беседы будет в первую очередь доставки в ответе.</span><span class="sxs-lookup"><span data-stu-id="38018-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="38018-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="38018-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="38018-120">**Базисная точка**</span><span class="sxs-lookup"><span data-stu-id="38018-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="38018-121">Описывает ли страница элементов или бесед начинается с самого начала или окончания набора элементов или бесед, найденных с помощью условия поиска.</span><span class="sxs-lookup"><span data-stu-id="38018-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="38018-122">При поиске с конца всегда ищет в обратном направлении.</span><span class="sxs-lookup"><span data-stu-id="38018-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="38018-123">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="38018-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="38018-124">Атрибут Базисная точка</span><span class="sxs-lookup"><span data-stu-id="38018-124">BasePoint Attribute</span></span>

|<span data-ttu-id="38018-125">**Значение**</span><span class="sxs-lookup"><span data-stu-id="38018-125">**Value**</span></span>|<span data-ttu-id="38018-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38018-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38018-127">Начало</span><span class="sxs-lookup"><span data-stu-id="38018-127">Beginning</span></span>  <br/> |<span data-ttu-id="38018-128">Постраничное представление начинается с начала обнаруженного набора беседы или элемента.</span><span class="sxs-lookup"><span data-stu-id="38018-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="38018-129">End</span><span class="sxs-lookup"><span data-stu-id="38018-129">End</span></span>  <br/> |<span data-ttu-id="38018-130">Постраничное представление начинается в конце обнаруженного set беседы или элемента.</span><span class="sxs-lookup"><span data-stu-id="38018-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38018-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38018-131">Child elements</span></span>

<span data-ttu-id="38018-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="38018-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38018-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38018-133">Parent elements</span></span>

|<span data-ttu-id="38018-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38018-134">**Element**</span></span>|<span data-ttu-id="38018-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38018-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38018-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="38018-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="38018-137">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="38018-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="38018-138">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="38018-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="38018-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="38018-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="38018-140">Определяет запрос на поиск бесед в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="38018-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38018-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="38018-141">Remarks</span></span>

<span data-ttu-id="38018-142">Поиск с конца включает в себя перемещение происхождения, определяемую средством смещение.</span><span class="sxs-lookup"><span data-stu-id="38018-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="38018-143">Кроме того указатель возвращается назад на число запрошенных записей.</span><span class="sxs-lookup"><span data-stu-id="38018-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="38018-144">Например если существует 100 записей и смещение равно 25 с конца, поиск начинается с 75.</span><span class="sxs-lookup"><span data-stu-id="38018-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="38018-145">Если будет возвращено 10 записей, указатель мыши перемещается назад дополнительные 10 записывает 65 и возвращает записи 65 через 75.</span><span class="sxs-lookup"><span data-stu-id="38018-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="38018-146">Следующий индекс — 64.</span><span class="sxs-lookup"><span data-stu-id="38018-146">The next index is 64.</span></span> <span data-ttu-id="38018-147">Далее смещение с конца страницы равно 100 минус 64, которое равно 36.</span><span class="sxs-lookup"><span data-stu-id="38018-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="38018-148">36 — это значение следующего смещения от конца для получения следующей страницы индексированных.</span><span class="sxs-lookup"><span data-stu-id="38018-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="38018-149">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="38018-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="38018-150">Пример</span><span class="sxs-lookup"><span data-stu-id="38018-150">Example</span></span>

<span data-ttu-id="38018-151">В следующем примере показано [FindItem операции](finditem-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="38018-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="38018-152">Каждый элемент возвращается вместе с его идентификатор и темы.</span><span class="sxs-lookup"><span data-stu-id="38018-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="38018-153">Не более шести элементы будут возвращены в ответ, как указано в атрибуте **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="38018-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="38018-154">Элементы, перечислены в восходящем порядке, сгруппированные по важности.</span><span class="sxs-lookup"><span data-stu-id="38018-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="38018-155">Элементы в группе объединенные по теме.</span><span class="sxs-lookup"><span data-stu-id="38018-155">Items in a group are aggregated by subject.</span></span> 
  
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

## <a name="element-information"></a><span data-ttu-id="38018-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38018-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38018-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38018-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38018-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38018-158">Schema Name</span></span>  <br/> |<span data-ttu-id="38018-159">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="38018-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38018-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38018-160">Validation File</span></span>  <br/> |<span data-ttu-id="38018-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38018-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38018-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38018-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="38018-163">False</span><span class="sxs-lookup"><span data-stu-id="38018-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38018-164">См. также</span><span class="sxs-lookup"><span data-stu-id="38018-164">See also</span></span>



[<span data-ttu-id="38018-165">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="38018-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="38018-166">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="38018-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="38018-167">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="38018-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

