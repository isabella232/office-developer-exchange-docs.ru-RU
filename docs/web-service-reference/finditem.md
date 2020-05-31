---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: Элемент FindItem определяет запрос на поиск элементов в почтовом ящике.
ms.openlocfilehash: 6664cd91007f1d39db7e8d446e0135f47d5ab932
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353926"
---
# <a name="finditem"></a><span data-ttu-id="d12b9-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="d12b9-103">FindItem</span></span>

<span data-ttu-id="d12b9-104">Элемент **FindItem** определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d12b9-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


<span data-ttu-id="d12b9-105">**финдитемтипе**</span><span class="sxs-lookup"><span data-stu-id="d12b9-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d12b9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d12b9-106">Attributes and elements</span></span>

<span data-ttu-id="d12b9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d12b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d12b9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d12b9-108">Attributes</span></span>

|<span data-ttu-id="d12b9-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d12b9-109">**Attribute**</span></span>|<span data-ttu-id="d12b9-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d12b9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d12b9-111">**Обход**</span><span class="sxs-lookup"><span data-stu-id="d12b9-111">**Traversal**</span></span> <br/> |<span data-ttu-id="d12b9-112">Определяет, ищет ли поиск элементы в папках или корзинах папок.</span><span class="sxs-lookup"><span data-stu-id="d12b9-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="d12b9-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="d12b9-114">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="d12b9-114">Traversal attribute values</span></span>

|<span data-ttu-id="d12b9-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d12b9-115">**Value**</span></span>|<span data-ttu-id="d12b9-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d12b9-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d12b9-117">Поверхност</span><span class="sxs-lookup"><span data-stu-id="d12b9-117">Shallow</span></span>  <br/> |<span data-ttu-id="d12b9-118">Возвращает только удостоверения элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="d12b9-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d12b9-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="d12b9-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="d12b9-120">Возвращает только удостоверения элементов в корзине папки.</span><span class="sxs-lookup"><span data-stu-id="d12b9-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="d12b9-121">Обратите внимание на то, что обратимо удаленный обход с ограничением поиска приведет к возвращению нулевых элементов, даже если имеются элементы, которые удовлетворяют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="d12b9-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="d12b9-122">Соответствующую</span><span class="sxs-lookup"><span data-stu-id="d12b9-122">Associated</span></span>  <br/> |<span data-ttu-id="d12b9-123">Возвращает только удостоверения связанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="d12b9-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d12b9-124">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d12b9-124">Child elements</span></span>

|<span data-ttu-id="d12b9-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d12b9-125">**Element**</span></span>|<span data-ttu-id="d12b9-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d12b9-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d12b9-127">итемшапе</span><span class="sxs-lookup"><span data-stu-id="d12b9-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="d12b9-128">Определяет свойства и содержимое элемента, включаемые в ответ [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d12b9-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-129">индекседпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="d12b9-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="d12b9-130">Описывает, как возвращаются сведения о страничном элементе для запроса **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="d12b9-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="d12b9-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-132">фрактионалпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="d12b9-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="d12b9-133">Описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="d12b9-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="d12b9-134">Смещение страничного представления от начала набора найденных элементов описывается с помощью дробной части.</span><span class="sxs-lookup"><span data-stu-id="d12b9-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="d12b9-135">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="d12b9-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="d12b9-137">Предоставляет ограниченные интервалы времени для определения поиска элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="d12b9-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="d12b9-138">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-139">контактсвиев</span><span class="sxs-lookup"><span data-stu-id="d12b9-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="d12b9-140">Определяет Поиск элементов контактов на основе отображаемых имен в алфавитном порядке.</span><span class="sxs-lookup"><span data-stu-id="d12b9-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="d12b9-141">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="d12b9-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="d12b9-143">Задает произвольное группирование для запросов **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="d12b9-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="d12b9-144">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-145">дистингуишедграупби</span><span class="sxs-lookup"><span data-stu-id="d12b9-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="d12b9-146">Предоставляет стандартные группирования для запросов **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="d12b9-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="d12b9-147">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="d12b9-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="d12b9-149">Определяет ограничение или запрос, используемый для фильтрации элементов или папок в операциях **FindItem**/ **FindFolder** и папок поиска.</span><span class="sxs-lookup"><span data-stu-id="d12b9-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="d12b9-150">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="d12b9-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="d12b9-152">Определяет порядок сортировки элементов в запросе FindItem.</span><span class="sxs-lookup"><span data-stu-id="d12b9-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="d12b9-153">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d12b9-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-154">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="d12b9-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="d12b9-155">Определяет папки для поиска операций FindItem и FindFolder.</span><span class="sxs-lookup"><span data-stu-id="d12b9-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="d12b9-156">Строка запроса (Куеристрингтипе)</span><span class="sxs-lookup"><span data-stu-id="d12b9-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="d12b9-157">Содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).</span><span class="sxs-lookup"><span data-stu-id="d12b9-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d12b9-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d12b9-158">Parent elements</span></span>

<span data-ttu-id="d12b9-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="d12b9-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d12b9-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="d12b9-160">Remarks</span></span>

<span data-ttu-id="d12b9-161">В запрос **FindItem** можно включить только один из элементов [индекседпажеитемвиев](indexedpageitemview.md), [фрактионалпажеитемвиев](fractionalpageitemview.md), [CalendarView](calendarview.md)или [контактсвиев](contactsview.md) .</span><span class="sxs-lookup"><span data-stu-id="d12b9-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="d12b9-162">В запрос **FindItem** можно включить только один из элементов [GroupBy](groupby.md) или [дистингуишедграупби](distinguishedgroupby.md) .</span><span class="sxs-lookup"><span data-stu-id="d12b9-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="d12b9-163">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d12b9-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d12b9-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d12b9-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d12b9-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d12b9-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d12b9-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d12b9-166">Schema Name</span></span>  <br/> |<span data-ttu-id="d12b9-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d12b9-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d12b9-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d12b9-168">Validation File</span></span>  <br/> |<span data-ttu-id="d12b9-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d12b9-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d12b9-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d12b9-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="d12b9-171">False</span><span class="sxs-lookup"><span data-stu-id="d12b9-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d12b9-172">См. также</span><span class="sxs-lookup"><span data-stu-id="d12b9-172">See also</span></span>

- [<span data-ttu-id="d12b9-173">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="d12b9-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="d12b9-174">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="d12b9-174">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

