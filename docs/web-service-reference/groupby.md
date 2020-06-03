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
description: Элемент GroupBy указывает произвольную группировку для запросов FindItem.
ms.openlocfilehash: 0d681e5376e4dd71921cc97f270211e49179db85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530101"
---
# <a name="groupby"></a><span data-ttu-id="51f78-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="51f78-103">GroupBy</span></span>

<span data-ttu-id="51f78-104">Элемент **GroupBy** указывает произвольную группировку для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="51f78-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="51f78-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="51f78-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="51f78-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="51f78-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

<span data-ttu-id="51f78-107">**граупбитипе**</span><span class="sxs-lookup"><span data-stu-id="51f78-107">**GroupByType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="51f78-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="51f78-108">Attributes and elements</span></span>

<span data-ttu-id="51f78-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="51f78-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51f78-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="51f78-110">Attributes</span></span>

|<span data-ttu-id="51f78-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="51f78-111">**Attribute**</span></span>|<span data-ttu-id="51f78-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f78-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51f78-113">**Order**</span><span class="sxs-lookup"><span data-stu-id="51f78-113">**Order**</span></span> <br/> | <span data-ttu-id="51f78-114">Определяет порядок групп в массиве сгруппированных элементов, который возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="51f78-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="51f78-115">Этот атрибут относится к типу Сортдиректионтипе.</span><span class="sxs-lookup"><span data-stu-id="51f78-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="51f78-116">Значения атрибутов Order</span><span class="sxs-lookup"><span data-stu-id="51f78-116">Order attribute values</span></span>

|<span data-ttu-id="51f78-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="51f78-117">**Value**</span></span>|<span data-ttu-id="51f78-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f78-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51f78-119">По возрастанию</span><span class="sxs-lookup"><span data-stu-id="51f78-119">Ascending</span></span>  <br/> |<span data-ttu-id="51f78-120">Группы упорядочиваются в порядке возрастания.</span><span class="sxs-lookup"><span data-stu-id="51f78-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="51f78-121">Убыванию</span><span class="sxs-lookup"><span data-stu-id="51f78-121">Descending</span></span>  <br/> |<span data-ttu-id="51f78-122">Группы упорядочиваются по убыванию.</span><span class="sxs-lookup"><span data-stu-id="51f78-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="51f78-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="51f78-123">Child elements</span></span>

|<span data-ttu-id="51f78-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51f78-124">**Element**</span></span>|<span data-ttu-id="51f78-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f78-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51f78-126">фиелдури</span><span class="sxs-lookup"><span data-stu-id="51f78-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="51f78-127">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="51f78-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="51f78-128">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="51f78-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="51f78-129">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="51f78-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="51f78-130">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="51f78-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="51f78-131">Определяет расширенные свойства MAPI, которые необходимо получить, задать или создать.</span><span class="sxs-lookup"><span data-stu-id="51f78-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="51f78-132">аггрегатеон</span><span class="sxs-lookup"><span data-stu-id="51f78-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="51f78-133">Представляет поле, используемое для определения порядка групп в отклике.</span><span class="sxs-lookup"><span data-stu-id="51f78-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51f78-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="51f78-134">Parent elements</span></span>

|<span data-ttu-id="51f78-135">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51f78-135">**Element**</span></span>|<span data-ttu-id="51f78-136">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51f78-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51f78-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="51f78-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="51f78-138">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="51f78-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="51f78-139">Ниже приведено выражение XPath для этого элемента:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="51f78-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51f78-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="51f78-140">Remarks</span></span>

<span data-ttu-id="51f78-141">Ответ FindItem будет содержать коллекцию групп.</span><span class="sxs-lookup"><span data-stu-id="51f78-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="51f78-142">Каждая группа будет содержать все элементы с соответствующими значениями свойства **GroupBy** .</span><span class="sxs-lookup"><span data-stu-id="51f78-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="51f78-143">Свойство, которое определяет группирование, определяется в элементе [фиелдури](fielduri.md), [индекседфиелдури](indexedfielduri.md)или [екстендедфиелдури](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="51f78-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="51f78-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="51f78-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51f78-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="51f78-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51f78-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="51f78-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="51f78-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="51f78-147">Schema Name</span></span>  <br/> |<span data-ttu-id="51f78-148">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="51f78-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="51f78-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="51f78-149">Validation File</span></span>  <br/> |<span data-ttu-id="51f78-150">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="51f78-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51f78-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="51f78-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="51f78-152">False</span><span class="sxs-lookup"><span data-stu-id="51f78-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51f78-153">См. также</span><span class="sxs-lookup"><span data-stu-id="51f78-153">See also</span></span>

- [<span data-ttu-id="51f78-154">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="51f78-154">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="51f78-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="51f78-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="51f78-156">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="51f78-156">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

