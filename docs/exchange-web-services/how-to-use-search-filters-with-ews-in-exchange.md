---
title: Использование фильтров поиска с EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Узнайте, как использовать фильтры поиска с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455837"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="54b19-103">Использование фильтров поиска с EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="54b19-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="54b19-104">Узнайте, как использовать фильтры поиска с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="54b19-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="54b19-105">Фильтры поиска — это основное средство для задания критериев поиска в управляемом API EWS или приложении EWS.</span><span class="sxs-lookup"><span data-stu-id="54b19-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="54b19-106">Рекомендуется использовать фильтры поиска, а не [строки запросов](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), для выполнения следующих действий:</span><span class="sxs-lookup"><span data-stu-id="54b19-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="54b19-107">Поиск по определенному свойству или набору свойств.</span><span class="sxs-lookup"><span data-stu-id="54b19-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="54b19-108">Поиск с использованием нескольких условий поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="54b19-109">Фильтры поиска — единственный вариант, если вы выполняете одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="54b19-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="54b19-110">Поиск настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="54b19-110">Searching custom properties.</span></span>  
- <span data-ttu-id="54b19-111">Выполняется поиск строки с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="54b19-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="54b19-112">Выполнение поиска по префиксу или точному совпадению строк.</span><span class="sxs-lookup"><span data-stu-id="54b19-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="54b19-113">Выполнение операций поиска по маске.</span><span class="sxs-lookup"><span data-stu-id="54b19-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="54b19-114">Поиск элементов с определенным набором свойств, независимо от значения.</span><span class="sxs-lookup"><span data-stu-id="54b19-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="54b19-115">Поиск папок.</span><span class="sxs-lookup"><span data-stu-id="54b19-115">Searching for folders.</span></span>
- <span data-ttu-id="54b19-116">Создание папок поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="54b19-117">Определение необходимого типа фильтра поиска</span><span class="sxs-lookup"><span data-stu-id="54b19-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="54b19-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-118"><a name="bk_SelectFilter"> </a></span></span>

<span data-ttu-id="54b19-119">Прежде чем приступать к созданию фильтра поиска, сначала определите необходимый тип фильтра.</span><span class="sxs-lookup"><span data-stu-id="54b19-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="54b19-120">Типы фильтров реализуются как классы потомков класса [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS, а также как дочерние элементы элемента [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в EWS.</span><span class="sxs-lookup"><span data-stu-id="54b19-120">The filter types are implemented as descendant classes of the [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="54b19-121">**Таблица 1. Типы фильтров поиска**</span><span class="sxs-lookup"><span data-stu-id="54b19-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="54b19-122">**Тип фильтра**</span><span class="sxs-lookup"><span data-stu-id="54b19-122">**Filter type**</span></span>|<span data-ttu-id="54b19-123">**Класс управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="54b19-123">**EWS Managed API class**</span></span>|<span data-ttu-id="54b19-124">**Элемент EWS**</span><span class="sxs-lookup"><span data-stu-id="54b19-124">**EWS element**</span></span>|<span data-ttu-id="54b19-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54b19-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="54b19-126">Содержит фильтр</span><span class="sxs-lookup"><span data-stu-id="54b19-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="54b19-127">контаинссубстринг</span><span class="sxs-lookup"><span data-stu-id="54b19-127">ContainsSubstring</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-128">Contains</span><span class="sxs-lookup"><span data-stu-id="54b19-128">Contains</span></span>](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-129">Лучший тип фильтра, используемый для сравнений строк.</span><span class="sxs-lookup"><span data-stu-id="54b19-129">The best filter type to use for string comparisons.</span></span> <span data-ttu-id="54b19-130">Он позволяет управлять чувствительностью к регистру, независимо от того, следует ли игнорировать пробелы и устанавливать режим включения.</span><span class="sxs-lookup"><span data-stu-id="54b19-130">It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="54b19-131">Фильтр масок</span><span class="sxs-lookup"><span data-stu-id="54b19-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="54b19-132">ексклудесбитмаск</span><span class="sxs-lookup"><span data-stu-id="54b19-132">ExcludesBitmask</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-133">Исключает</span><span class="sxs-lookup"><span data-stu-id="54b19-133">Excludes</span></span>](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-134">Позволяет выполнять поиск в целых свойствах в виде битовых масок и возвращать только результаты с битами, соответствующими заданной битовой маске.</span><span class="sxs-lookup"><span data-stu-id="54b19-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="54b19-135">Фильтр EXISTS</span><span class="sxs-lookup"><span data-stu-id="54b19-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="54b19-136">Exists</span><span class="sxs-lookup"><span data-stu-id="54b19-136">Exists</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-137">Exists</span><span class="sxs-lookup"><span data-stu-id="54b19-137">Exists</span></span>](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-138">Возвращает все элементы, у которых есть указанное свойство, независимо от значения.</span><span class="sxs-lookup"><span data-stu-id="54b19-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="54b19-139">Фильтр равенства</span><span class="sxs-lookup"><span data-stu-id="54b19-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="54b19-140">исекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-140">IsEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="54b19-141">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-141">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-142">исекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-142">IsEqualTo</span></span>](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="54b19-143">иснотекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-143">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-144">Сравнивает значение указанного свойства с указанным значением константы или значением другого свойства и возвращает все элементы, имеющие значение равно (в случае фильтра **исекуалто** ) или не равное значение (в случае фильтра **иснотекуалто** ).</span><span class="sxs-lookup"><span data-stu-id="54b19-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="54b19-145">Фильтр реляционного тестирования</span><span class="sxs-lookup"><span data-stu-id="54b19-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="54b19-146">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="54b19-146">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="54b19-147">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-147">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="54b19-148">ислесссан</span><span class="sxs-lookup"><span data-stu-id="54b19-148">IsLessThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="54b19-149">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-149">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-150">исгреатерсан</span><span class="sxs-lookup"><span data-stu-id="54b19-150">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="54b19-151">исгреатерсанорекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-151">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="54b19-152">ислесссан</span><span class="sxs-lookup"><span data-stu-id="54b19-152">IsLessThan</span></span>](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="54b19-153">ислесссанорекуалто</span><span class="sxs-lookup"><span data-stu-id="54b19-153">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-154">Возвращает все элементы, имеющие значение указанного свойства в соответствии с указанным значением константы или с другим свойством.</span><span class="sxs-lookup"><span data-stu-id="54b19-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="54b19-155">Например, фильтр **исгреатерсан** возвращает все элементы со значением, превышающим указанное значение в указанном свойстве.</span><span class="sxs-lookup"><span data-stu-id="54b19-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="54b19-156">Фильтр отрицания</span><span class="sxs-lookup"><span data-stu-id="54b19-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="54b19-157">Not</span><span class="sxs-lookup"><span data-stu-id="54b19-157">Not</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-158">Not</span><span class="sxs-lookup"><span data-stu-id="54b19-158">Not</span></span>](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-159">Инвертирует результат других фильтров.</span><span class="sxs-lookup"><span data-stu-id="54b19-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="54b19-160">Составной фильтр</span><span class="sxs-lookup"><span data-stu-id="54b19-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="54b19-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="54b19-161">SearchFilterCollection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="54b19-162">And</span><span class="sxs-lookup"><span data-stu-id="54b19-162">And</span></span>](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="54b19-163">Or</span><span class="sxs-lookup"><span data-stu-id="54b19-163">Or</span></span>](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="54b19-164">Объединяет несколько фильтров, позволяя использовать более сложные критерии поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="54b19-165">Содержит фильтр</span><span class="sxs-lookup"><span data-stu-id="54b19-165">Contains filter</span></span>

<span data-ttu-id="54b19-166">Фильтр содержит является лучшим выбором для поиска свойств строки.</span><span class="sxs-lookup"><span data-stu-id="54b19-166">A contains filter is the best choice for searching string properties.</span></span> <span data-ttu-id="54b19-167">С помощью фильтра CONTAINS можно управлять аспектами совпадений строк, например чувствительностью к регистру и продолжением обработки пробела, путем установки режима включения и сравнения.</span><span class="sxs-lookup"><span data-stu-id="54b19-167">With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-168">Содержит фильтр в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="54b19-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-169"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="54b19-170">Если вы используете управляемый API EWS, то задается режим включения с помощью свойства [контаинментмоде](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) класса [контаинссубстринг](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) , а режим сравнения задается с помощью свойства [компарисонмоде](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) класса **контаинссубстринг** .</span><span class="sxs-lookup"><span data-stu-id="54b19-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="54b19-171">В приведенном ниже примере показано, как создать фильтр поиска, который выполняет поиск в поле subject элементов для подстроки "заметки к собранию".</span><span class="sxs-lookup"><span data-stu-id="54b19-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="54b19-172">В этом примере игнорируется регистр, но не учитывается пробелы.</span><span class="sxs-lookup"><span data-stu-id="54b19-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="54b19-173">Содержит фильтр в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-173">Contains filter in EWS</span></span>
<span data-ttu-id="54b19-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-174"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="54b19-175">В EWS режим включения задается с помощью атрибута **контаинментмоде** в элементе [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) , а режим сравнения задается с помощью атрибута **контаинменткомпарисон** элемента **Contains** .</span><span class="sxs-lookup"><span data-stu-id="54b19-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="54b19-176">В приведенном ниже примере показано, как создать фильтр поиска для поиска в поле темы элементов для подстроки "заметки к собранию".</span><span class="sxs-lookup"><span data-stu-id="54b19-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="54b19-177">В этом примере игнорируется регистр, но не учитывается пробелы.</span><span class="sxs-lookup"><span data-stu-id="54b19-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="54b19-178">Фильтр масок</span><span class="sxs-lookup"><span data-stu-id="54b19-178">Bitmask filter</span></span>

<span data-ttu-id="54b19-179">Фильтр битовая маска позволяет выполнять поиск в целых свойствах в виде битовых масок и возвращать результаты, в которых определенные биты не задаются в значении указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="54b19-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-180">Фильтр масок битов в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-181">В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все элементы, имеющие значение в настраиваемом свойстве **итеминдекс** (которое определяется в [примере: Поиск элементов с помощью фильтра поиска и раздела УПРАВЛЯЕМого API EWS](#bk_ExampleEWSMA) в этой статье), для которых не задан второй бит (10 в двоичном формате).</span><span class="sxs-lookup"><span data-stu-id="54b19-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="54b19-182">Фильтр масок битов в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="54b19-183">В приведенном ниже примере показано, как использовать EWS для создания фильтра поиска, чтобы возвратить все элементы, имеющие значение в настраиваемом свойстве **итеминдекс** (которое определяется в [примере: Поиск элементов с помощью фильтра поиска и раздела УПРАВЛЯЕМого API EWS](#bk_ExampleEWSMA) в этой статье), для которых не задан второй бит (10 в двоичном формате).</span><span class="sxs-lookup"><span data-stu-id="54b19-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="54b19-184">Фильтр EXISTS</span><span class="sxs-lookup"><span data-stu-id="54b19-184">Exists filter</span></span>

<span data-ttu-id="54b19-185">Фильтр Exists позволяет искать элементы, для которых задано определенное свойство, независимо от значения.</span><span class="sxs-lookup"><span data-stu-id="54b19-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-186">Фильтр EXISTS в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-187">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых есть набор настраиваемых свойств **итеминдекс** .</span><span class="sxs-lookup"><span data-stu-id="54b19-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="54b19-188">Фильтр EXISTS в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-188">Exists filter in EWS</span></span>

<span data-ttu-id="54b19-189">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых есть набор настраиваемых свойств **итеминдекс** .</span><span class="sxs-lookup"><span data-stu-id="54b19-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="54b19-190">Фильтр равенства</span><span class="sxs-lookup"><span data-stu-id="54b19-190">Equality filter</span></span>

<span data-ttu-id="54b19-191">Фильтры равенства позволяют выполнять поиск всех элементов со значением указанного свойства, которые либо равны определенному значению, либо не равны определенному значению.</span><span class="sxs-lookup"><span data-stu-id="54b19-191">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value.</span></span> <span data-ttu-id="54b19-192">Значение, с которым выполняется сравнение, может быть постоянным значением или значением другого свойства для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="54b19-192">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-193">Фильтр равенства в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-194">В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все непрочитанные элементы.</span><span class="sxs-lookup"><span data-stu-id="54b19-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="54b19-195">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , не равным размеру элемента.</span><span class="sxs-lookup"><span data-stu-id="54b19-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="54b19-196">Фильтр равенства в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-196">Equality filter in EWS</span></span>

<span data-ttu-id="54b19-197">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех непрочитанных элементов с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="54b19-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="54b19-198">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , не равным размеру элемента.</span><span class="sxs-lookup"><span data-stu-id="54b19-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="54b19-199">Фильтр реляционного тестирования</span><span class="sxs-lookup"><span data-stu-id="54b19-199">Relational testing filter</span></span>

<span data-ttu-id="54b19-200">Фильтры реляционных тестов позволяют выполнять поиск всех элементов со значением в указанном свойстве, которое может быть больше ( \> ), больше или равно ( \> =), меньше ( \< ) или меньше или равно ( \< =) заданному значению.</span><span class="sxs-lookup"><span data-stu-id="54b19-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="54b19-201">Значение, с которым выполняется сравнение, может быть постоянным значением или значением другого свойства для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="54b19-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-202">Фильтр реляционного тестирования в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-203">В приведенном ниже примере показано, как с помощью управляемого API EWS создавать фильтры поиска, чтобы возвратить все элементы со значением в свойстве **итеминдекс** с указанным отношением в константное значение 3.</span><span class="sxs-lookup"><span data-stu-id="54b19-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="54b19-204">Фильтр реляционного тестирования в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="54b19-205">В приведенном ниже примере показано, как с помощью EWS создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое больше, чем значение константы 3.</span><span class="sxs-lookup"><span data-stu-id="54b19-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="54b19-206">В приведенном ниже примере показано, как создать фильтр поиска, чтобы возвратить все элементы со значением в свойстве **итеминдекс** , которое больше или равно значению константы 3.</span><span class="sxs-lookup"><span data-stu-id="54b19-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="54b19-207">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое меньше значения константы 3.</span><span class="sxs-lookup"><span data-stu-id="54b19-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="54b19-208">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое меньше или равно константе 3.</span><span class="sxs-lookup"><span data-stu-id="54b19-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="54b19-209">Фильтр отрицания</span><span class="sxs-lookup"><span data-stu-id="54b19-209">Negating filter</span></span>

<span data-ttu-id="54b19-210">Фильтр отрицания позволяет инвертировать другой фильтр и получить противоположные результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-210">A negating filter enables you to negate another filter and get the opposite search results.</span></span> <span data-ttu-id="54b19-211">Несмотря на то что другие фильтры возвращают результаты, которые удовлетворяют определенным условиям, фильтр отрицания возвращает результаты, которые не отвечают условиям фильтра, к которому он применяется.</span><span class="sxs-lookup"><span data-stu-id="54b19-211">While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-212">Фильтр отрицания в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-213">В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все элементы, у которых нет подстроки "заметки к собранию" в теме.</span><span class="sxs-lookup"><span data-stu-id="54b19-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="54b19-214">Фильтр отрицания в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-214">Negating filter in EWS</span></span>

<span data-ttu-id="54b19-215">В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых нет подстроки "заметки к собранию" в теме.</span><span class="sxs-lookup"><span data-stu-id="54b19-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="54b19-216">Составной фильтр</span><span class="sxs-lookup"><span data-stu-id="54b19-216">Compound filter</span></span>

<span data-ttu-id="54b19-217">Составной фильтр позволяет объединить несколько фильтров для создания более сложных условий поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="54b19-218">Вы можете комбинировать критерии, используя логические операторы и или.</span><span class="sxs-lookup"><span data-stu-id="54b19-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="54b19-219">Таким образом, вы можете выполнять поиски, например "все сообщения из Ольга Даниелс, которые содержат" заметки о собраниях "в теме".</span><span class="sxs-lookup"><span data-stu-id="54b19-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="54b19-220">Составной фильтр в управляемом API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="54b19-221">В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, который возвращает все элементы, отправленные из Ольга Даниелс и содержащие "заметки о собраниях" в теме.</span><span class="sxs-lookup"><span data-stu-id="54b19-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="54b19-222">Составной фильтр в EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-222">Compound filter in EWS</span></span>

<span data-ttu-id="54b19-223">В приведенном ниже примере показано, как использовать EWS для создания фильтра поиска, который возвращает все элементы, отправленные из Ольга Даниелс и содержащие "заметки о собраниях" в теме.</span><span class="sxs-lookup"><span data-stu-id="54b19-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="54b19-224">Пример: Поиск элементов с помощью фильтра поиска и управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="54b19-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-225"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="54b19-226">В следующих методах управляемого API EWS используются фильтры поиска:</span><span class="sxs-lookup"><span data-stu-id="54b19-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="54b19-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="54b19-227">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="54b19-228">ExchangeService. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="54b19-228">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="54b19-229">Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="54b19-229">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="54b19-230">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="54b19-230">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="54b19-231">В следующем примере используется метод **ExchangeService. FindItems** ; Тем не менее, одни и те же правила и концепции применяются ко всем методам.</span><span class="sxs-lookup"><span data-stu-id="54b19-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="54b19-232">В этом примере определен метод под названием **сеарчвисфилтер** .</span><span class="sxs-lookup"><span data-stu-id="54b19-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="54b19-233">Он принимает объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [Веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="54b19-233">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="54b19-234">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="54b19-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="54b19-235">Класс **SearchFilter** является базовым классом для всех различных фильтров поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="54b19-236">Эту функцию можно использовать с любыми фильтрами поиска, приведенными в примерах, приведенных в этой статье.</span><span class="sxs-lookup"><span data-stu-id="54b19-236">You can use this function with any of the search filters shown in the examples in this article.</span></span> <span data-ttu-id="54b19-237">В этом примере используется составной фильтр для возврата всех элементов из папки "Входящие" из Ольга Даниелс с "заметками о собраниях" в теме.</span><span class="sxs-lookup"><span data-stu-id="54b19-237">This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="54b19-238">Пример: Поиск элемента с помощью фильтра поиска и EWS</span><span class="sxs-lookup"><span data-stu-id="54b19-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="54b19-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-239"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="54b19-240">Следующие операции EWS используют фильтры поиска:</span><span class="sxs-lookup"><span data-stu-id="54b19-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="54b19-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="54b19-241">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="54b19-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="54b19-242">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="54b19-243">В приведенном ниже примере используется операция **FindItem** ; Тем не менее, одни и те же правила и концепции применимы к обеим операциям.</span><span class="sxs-lookup"><span data-stu-id="54b19-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="54b19-244">Фильтры поиска хранятся в элементе [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в запросах SOAP.</span><span class="sxs-lookup"><span data-stu-id="54b19-244">Search filters are contained in the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="54b19-245">В этом примере отправляется SOAP-запрос, эквивалентный поиску, который показан в предыдущем примере управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="54b19-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
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

<span data-ttu-id="54b19-246">В следующем примере показан ответ от сервера, включая результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
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
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="54b19-247">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="54b19-247">Next steps</span></span>
<span data-ttu-id="54b19-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="54b19-248"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="54b19-249">Теперь, когда вы знакомы с использованием фильтров поиска в основных операциях поиска, вы можете перейти на дополнительные приемы расширенного поиска.</span><span class="sxs-lookup"><span data-stu-id="54b19-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="54b19-250">Выполнение группового поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="54b19-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="54b19-251">Выполнение постраничного поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="54b19-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="54b19-252">См. также</span><span class="sxs-lookup"><span data-stu-id="54b19-252">See also</span></span>

- [<span data-ttu-id="54b19-253">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="54b19-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="54b19-254">Выполнение поиска AQS с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="54b19-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="54b19-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="54b19-255">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="54b19-256">ExchangeService. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="54b19-256">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="54b19-257">Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="54b19-257">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="54b19-258">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="54b19-258">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="54b19-259">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="54b19-259">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="54b19-260">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="54b19-260">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

