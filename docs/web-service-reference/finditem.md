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
description: Элемент FindItem определяет запрос для поиска элементов в почтовом ящике.
ms.openlocfilehash: 9831b034be7deb0cf6e756bb585bdbe34b370afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762577"
---
# <a name="finditem"></a><span data-ttu-id="77b9a-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="77b9a-103">FindItem</span></span>

<span data-ttu-id="77b9a-104">Элемент **FindItem** определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="77b9a-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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

 <span data-ttu-id="77b9a-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="77b9a-105">**FindItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77b9a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77b9a-106">Attributes and elements</span></span>

<span data-ttu-id="77b9a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="77b9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77b9a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77b9a-108">Attributes</span></span>

|<span data-ttu-id="77b9a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="77b9a-109">**Attribute**</span></span>|<span data-ttu-id="77b9a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77b9a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77b9a-111">**Обход**</span><span class="sxs-lookup"><span data-stu-id="77b9a-111">**Traversal**</span></span> <br/> |<span data-ttu-id="77b9a-112">Определяет, будет ли поиск элементов в папках или папки корзины.</span><span class="sxs-lookup"><span data-stu-id="77b9a-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="77b9a-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="77b9a-114">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="77b9a-114">Traversal attribute values</span></span>

|<span data-ttu-id="77b9a-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="77b9a-115">**Value**</span></span>|<span data-ttu-id="77b9a-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77b9a-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77b9a-117">Неполная</span><span class="sxs-lookup"><span data-stu-id="77b9a-117">Shallow</span></span>  <br/> |<span data-ttu-id="77b9a-118">Возвращает только идентификаторы элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="77b9a-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="77b9a-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="77b9a-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="77b9a-120">Возвращает только идентификаторы элементов, находящихся в папке корзины.</span><span class="sxs-lookup"><span data-stu-id="77b9a-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="77b9a-121">Обратите внимание, что удаленные обхода, в сочетании с ограничения поиска приведет к нулю, найденном даже в том случае, если существуют элементы, соответствующие условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="77b9a-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="77b9a-122">Связанные</span><span class="sxs-lookup"><span data-stu-id="77b9a-122">Associated</span></span>  <br/> |<span data-ttu-id="77b9a-123">Возвращает только идентификаторы связанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="77b9a-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="77b9a-124">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77b9a-124">Child elements</span></span>

|<span data-ttu-id="77b9a-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77b9a-125">**Element**</span></span>|<span data-ttu-id="77b9a-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77b9a-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77b9a-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="77b9a-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="77b9a-128">Определяет свойства элемента и содержимого для включения в [операции FindItem](finditem-operation.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="77b9a-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="77b9a-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="77b9a-130">Описывает, как выгружаемый элемента сведения возвращаются для запроса **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="77b9a-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="77b9a-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="77b9a-133">Описывает, где начала страничного представления и максимальное число элементов, возвращаемых в запросе **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="77b9a-134">Смещение страничного представления от начала набора найденных элементов описывается функцией.</span><span class="sxs-lookup"><span data-stu-id="77b9a-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="77b9a-135">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-136">Представления календаря</span><span class="sxs-lookup"><span data-stu-id="77b9a-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="77b9a-137">Содержит время охватывать ограничения для определения критериев поиска для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="77b9a-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="77b9a-138">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="77b9a-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="77b9a-140">Определяет поиска на основе алфавитном отображения имен контактов.</span><span class="sxs-lookup"><span data-stu-id="77b9a-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="77b9a-141">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="77b9a-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="77b9a-143">Указывает произвольное группирование для запросов **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="77b9a-144">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="77b9a-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="77b9a-146">Содержит стандартные группы для запросов **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="77b9a-147">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-148">Ограничения</span><span class="sxs-lookup"><span data-stu-id="77b9a-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="77b9a-149">Задает ограничение или запрос, используемый для фильтрации элементов или папок в **FindItem**/ **FindFolder** и папки операций поиска.</span><span class="sxs-lookup"><span data-stu-id="77b9a-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="77b9a-150">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="77b9a-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="77b9a-152">Определяет способ сортировки в запросе FindItem элементов.</span><span class="sxs-lookup"><span data-stu-id="77b9a-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="77b9a-153">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="77b9a-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="77b9a-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="77b9a-155">Идентифицирует папок для поиска для операций FindItem и FindFolder.</span><span class="sxs-lookup"><span data-stu-id="77b9a-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="77b9a-156">Строка запроса (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="77b9a-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="77b9a-157">Содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).</span><span class="sxs-lookup"><span data-stu-id="77b9a-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77b9a-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77b9a-158">Parent elements</span></span>

<span data-ttu-id="77b9a-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="77b9a-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77b9a-160">Замечания</span><span class="sxs-lookup"><span data-stu-id="77b9a-160">Remarks</span></span>

<span data-ttu-id="77b9a-161">Только один из [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [представления календаря](calendarview.md)или элементы [ContactsView](contactsview.md) может быть включен в запросе **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="77b9a-162">Только один из элементов [GroupBy](groupby.md) или [DistinguishedGroupBy](distinguishedgroupby.md) может быть включен в запросе **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="77b9a-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="77b9a-163">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b9a-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77b9a-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77b9a-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77b9a-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77b9a-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77b9a-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77b9a-166">Schema Name</span></span>  <br/> |<span data-ttu-id="77b9a-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="77b9a-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77b9a-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77b9a-168">Validation File</span></span>  <br/> |<span data-ttu-id="77b9a-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77b9a-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77b9a-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77b9a-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="77b9a-171">False</span><span class="sxs-lookup"><span data-stu-id="77b9a-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77b9a-172">См. также</span><span class="sxs-lookup"><span data-stu-id="77b9a-172">See also</span></span>



[<span data-ttu-id="77b9a-173">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="77b9a-173">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="77b9a-174">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="77b9a-174">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

