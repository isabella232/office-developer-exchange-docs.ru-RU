---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: Элемент GroupBy задает произвольную группировки для запросов FindItem.
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833753"
---
# <a name="groupby"></a><span data-ttu-id="e7c5c-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="e7c5c-103">GroupBy</span></span>

<span data-ttu-id="e7c5c-104">Элемент **GroupBy** задает произвольную группировки для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="e7c5c-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="e7c5c-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="e7c5c-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="e7c5c-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

 <span data-ttu-id="e7c5c-107">**GroupByType**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-107">**GroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7c5c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7c5c-108">Attributes and elements</span></span>

<span data-ttu-id="e7c5c-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7c5c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7c5c-110">Attributes</span></span>

|<span data-ttu-id="e7c5c-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-111">**Attribute**</span></span>|<span data-ttu-id="e7c5c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7c5c-113">**Порядок**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-113">**Order**</span></span> <br/> | <span data-ttu-id="e7c5c-114">Определяет порядок групп в массиве сгруппированных элементов, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="e7c5c-115">Этот атрибут имеет тип SortDirectionType.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="e7c5c-116">Значения атрибутов заказа</span><span class="sxs-lookup"><span data-stu-id="e7c5c-116">Order attribute values</span></span>

|<span data-ttu-id="e7c5c-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-117">**Value**</span></span>|<span data-ttu-id="e7c5c-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7c5c-119">По возрастанию</span><span class="sxs-lookup"><span data-stu-id="e7c5c-119">Ascending</span></span>  <br/> |<span data-ttu-id="e7c5c-120">Группы упорядочены в порядке возрастания.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="e7c5c-121">Descending</span><span class="sxs-lookup"><span data-stu-id="e7c5c-121">Descending</span></span>  <br/> |<span data-ttu-id="e7c5c-122">Группы упорядочены по убыванию.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e7c5c-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7c5c-123">Child elements</span></span>

|<span data-ttu-id="e7c5c-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-124">**Element**</span></span>|<span data-ttu-id="e7c5c-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7c5c-126">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e7c5c-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="e7c5c-127">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="e7c5c-128">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e7c5c-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="e7c5c-129">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="e7c5c-130">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e7c5c-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e7c5c-131">Задает расширенные свойства MAPI для получения, установки или создать.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="e7c5c-132">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="e7c5c-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="e7c5c-133">Представляет поле, которое используется для определения порядка групп в ответе.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7c5c-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7c5c-134">Parent elements</span></span>

|<span data-ttu-id="e7c5c-135">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-135">**Element**</span></span>|<span data-ttu-id="e7c5c-136">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7c5c-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7c5c-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="e7c5c-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="e7c5c-138">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="e7c5c-139">Ниже приведен выражение XPath для этого элемента.`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="e7c5c-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7c5c-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="e7c5c-140">Remarks</span></span>

<span data-ttu-id="e7c5c-141">Ответ FindItem будет содержать коллекцию групп.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="e7c5c-142">Каждой группе будет содержать все элементы, которым пришлось совпадающие значения для свойства **GroupBy** .</span><span class="sxs-lookup"><span data-stu-id="e7c5c-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="e7c5c-143">Свойство, которое определяет группирование идентифицируется в элементе [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="e7c5c-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="e7c5c-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e7c5c-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7c5c-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7c5c-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7c5c-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7c5c-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7c5c-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7c5c-147">Schema Name</span></span>  <br/> |<span data-ttu-id="e7c5c-148">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e7c5c-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7c5c-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7c5c-149">Validation File</span></span>  <br/> |<span data-ttu-id="e7c5c-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e7c5c-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7c5c-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7c5c-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7c5c-152">False</span><span class="sxs-lookup"><span data-stu-id="e7c5c-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7c5c-153">См. также</span><span class="sxs-lookup"><span data-stu-id="e7c5c-153">See also</span></span>

- [<span data-ttu-id="e7c5c-154">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="e7c5c-154">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="e7c5c-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e7c5c-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="e7c5c-156">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="e7c5c-156">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

