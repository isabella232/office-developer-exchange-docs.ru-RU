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
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833919"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="32ff6-103">индекседпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="32ff6-103">IndexedPageItemView</span></span>

<span data-ttu-id="32ff6-104">Элемент **индекседпажеитемвиев** описывает, как возвращаются страничные беседы или сведения об элементе для [операции FindItem](finditem-operation.md) или запроса [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="32ff6-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="32ff6-105">**индекседпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="32ff6-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32ff6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="32ff6-106">Attributes and elements</span></span>

<span data-ttu-id="32ff6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="32ff6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32ff6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="32ff6-108">Attributes</span></span>

|<span data-ttu-id="32ff6-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="32ff6-109">**Attribute**</span></span>|<span data-ttu-id="32ff6-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32ff6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32ff6-111">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="32ff6-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="32ff6-112">Описывает максимальное число элементов или бесед, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="32ff6-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="32ff6-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="32ff6-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="32ff6-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="32ff6-114">**Offset**</span></span> <br/> |<span data-ttu-id="32ff6-115">Описывает смещение от **басепоинт**.</span><span class="sxs-lookup"><span data-stu-id="32ff6-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="32ff6-116">Если **басепоинт** равно "начало", смещение является положительным.</span><span class="sxs-lookup"><span data-stu-id="32ff6-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="32ff6-117">Если **басепоинт** равен end, то смещение обрабатывается так, как если бы оно было отрицательным.</span><span class="sxs-lookup"><span data-stu-id="32ff6-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="32ff6-118">Это позволяет определить, какой элемент или беседа будет первым доставлен в ответе.</span><span class="sxs-lookup"><span data-stu-id="32ff6-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="32ff6-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="32ff6-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="32ff6-120">**басепоинт**</span><span class="sxs-lookup"><span data-stu-id="32ff6-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="32ff6-121">Указывает, будет ли страница элементов или бесед начинается с начала или с конца набора элементов или бесед, найденных с помощью условий поиска.</span><span class="sxs-lookup"><span data-stu-id="32ff6-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="32ff6-122">Поиск от End всегда выполняет поиск в обратном направлении.</span><span class="sxs-lookup"><span data-stu-id="32ff6-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="32ff6-123">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="32ff6-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="32ff6-124">Атрибут Басепоинт</span><span class="sxs-lookup"><span data-stu-id="32ff6-124">BasePoint Attribute</span></span>

|<span data-ttu-id="32ff6-125">**Значение**</span><span class="sxs-lookup"><span data-stu-id="32ff6-125">**Value**</span></span>|<span data-ttu-id="32ff6-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32ff6-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32ff6-127">Слайд</span><span class="sxs-lookup"><span data-stu-id="32ff6-127">Beginning</span></span>  <br/> |<span data-ttu-id="32ff6-128">Постраничное представление начинается с начала найденного диалога или набора элементов.</span><span class="sxs-lookup"><span data-stu-id="32ff6-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="32ff6-129">Конец</span><span class="sxs-lookup"><span data-stu-id="32ff6-129">End</span></span>  <br/> |<span data-ttu-id="32ff6-130">Постраничное представление начинается в конце найденного диалога или набора элементов.</span><span class="sxs-lookup"><span data-stu-id="32ff6-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="32ff6-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="32ff6-131">Child elements</span></span>

<span data-ttu-id="32ff6-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="32ff6-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32ff6-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="32ff6-133">Parent elements</span></span>

|<span data-ttu-id="32ff6-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="32ff6-134">**Element**</span></span>|<span data-ttu-id="32ff6-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32ff6-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32ff6-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="32ff6-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="32ff6-137">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="32ff6-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="32ff6-138">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="32ff6-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="32ff6-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="32ff6-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="32ff6-140">Определяет запрос на поиск бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="32ff6-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="32ff6-141">Примечания</span><span class="sxs-lookup"><span data-stu-id="32ff6-141">Remarks</span></span>

<span data-ttu-id="32ff6-142">Поиск с конца включает перемещение к началу, определяемому смещением.</span><span class="sxs-lookup"><span data-stu-id="32ff6-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="32ff6-143">Кроме того, указатель перемещается обратно на число запрошенных записей.</span><span class="sxs-lookup"><span data-stu-id="32ff6-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="32ff6-144">Например, если имеется 100 записей, а смещение — 25 из конца, поиск начинается с 75.</span><span class="sxs-lookup"><span data-stu-id="32ff6-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="32ff6-145">Если возвращено 10 записей, указатель перемещается обратно в обратное 10 записей в 65 и возвращает записи от 65 до 75.</span><span class="sxs-lookup"><span data-stu-id="32ff6-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="32ff6-146">Следующий индекс — 64.</span><span class="sxs-lookup"><span data-stu-id="32ff6-146">The next index is 64.</span></span> <span data-ttu-id="32ff6-147">Следующее смещение от конца для страницы составляет 100 минус 64, что равно 36.</span><span class="sxs-lookup"><span data-stu-id="32ff6-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="32ff6-148">36 это значение для следующего смещения, начиная с конца, для получения следующей индексированной страницы.</span><span class="sxs-lookup"><span data-stu-id="32ff6-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="32ff6-149">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="32ff6-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="32ff6-150">Пример</span><span class="sxs-lookup"><span data-stu-id="32ff6-150">Example</span></span>

<span data-ttu-id="32ff6-151">В приведенном ниже примере показан запрос [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="32ff6-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="32ff6-152">Каждый элемент возвращается с ИДЕНТИФИКАТОРом и темой.</span><span class="sxs-lookup"><span data-stu-id="32ff6-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="32ff6-153">В отклике возвращается не более шести элементов, как указано в атрибуте **максентриесретурнед** .</span><span class="sxs-lookup"><span data-stu-id="32ff6-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="32ff6-154">Элементы перечислены в порядке возрастания, сгруппированные по важности.</span><span class="sxs-lookup"><span data-stu-id="32ff6-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="32ff6-155">Элементы в группе объединяются по темам.</span><span class="sxs-lookup"><span data-stu-id="32ff6-155">Items in a group are aggregated by subject.</span></span> 
  
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

## <a name="element-information"></a><span data-ttu-id="32ff6-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="32ff6-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32ff6-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="32ff6-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32ff6-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="32ff6-158">Schema Name</span></span>  <br/> |<span data-ttu-id="32ff6-159">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="32ff6-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32ff6-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="32ff6-160">Validation File</span></span>  <br/> |<span data-ttu-id="32ff6-161">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="32ff6-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32ff6-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="32ff6-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="32ff6-163">False</span><span class="sxs-lookup"><span data-stu-id="32ff6-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32ff6-164">См. также</span><span class="sxs-lookup"><span data-stu-id="32ff6-164">See also</span></span>



[<span data-ttu-id="32ff6-165">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="32ff6-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="32ff6-166">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="32ff6-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="32ff6-167">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="32ff6-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

