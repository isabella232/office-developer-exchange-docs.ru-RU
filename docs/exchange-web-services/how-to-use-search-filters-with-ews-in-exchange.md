---
title: Используйте фильтры поиска с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Узнайте, как использовать фильтры поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 0652c36fd610c2f9dfe22b55323b368997137e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761139"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="8a2ee-103">Используйте фильтры поиска с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="8a2ee-104">Узнайте, как использовать фильтры поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8a2ee-105">Фильтры поиска являются основным средством для выражения условия поиска в управляемый API EWS или приложение веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="8a2ee-106">Рекомендуется использовать фильтры поиска, в отличие от [строки запроса](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), чтобы выполнить перечисленные ниже:</span><span class="sxs-lookup"><span data-stu-id="8a2ee-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="8a2ee-107">Поиск на определенное свойство или набор свойств.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="8a2ee-108">Поиск с использованием нескольких условий поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="8a2ee-109">Фильтры поиска являются единственным вариантом при выполнении одной из следующих:</span><span class="sxs-lookup"><span data-stu-id="8a2ee-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="8a2ee-110">Поиск настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-110">Searching custom properties.</span></span>  
- <span data-ttu-id="8a2ee-111">Выполняет поиск для выполнения строк с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="8a2ee-112">Выполняется поиск точного совпадения строки или префикс для выполнения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="8a2ee-113">Для выполнения битовой маски выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="8a2ee-114">Поиск элементов, которые имеют определенное свойство задано, независимо от значения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="8a2ee-115">Поиск папок.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-115">Searching for folders.</span></span>
- <span data-ttu-id="8a2ee-116">Создание папки поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="8a2ee-117">Определите, какой тип фильтра поиска нужно</span><span class="sxs-lookup"><span data-stu-id="8a2ee-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="8a2ee-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-118"></span></span>

<span data-ttu-id="8a2ee-119">Перед созданием поисковый фильтр сначала определите, какой тип фильтра.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="8a2ee-120">Типы фильтра реализуются потомкам классы класса [SearchFilter](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в управляемый API веб-служб Exchange, а дочерние элементы элемента [ограничение](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-120">The filter types are implemented as descendant classes of the [SearchFilter](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="8a2ee-121">**В таблице 1. Типы фильтров поиска**</span><span class="sxs-lookup"><span data-stu-id="8a2ee-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="8a2ee-122">**Тип фильтра**</span><span class="sxs-lookup"><span data-stu-id="8a2ee-122">**Filter type**</span></span>|<span data-ttu-id="8a2ee-123">**Управляемый API EWS класс**</span><span class="sxs-lookup"><span data-stu-id="8a2ee-123">**EWS Managed API class**</span></span>|<span data-ttu-id="8a2ee-124">**Элемент веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="8a2ee-124">**EWS element**</span></span>|<span data-ttu-id="8a2ee-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a2ee-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="8a2ee-126">Содержит фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="8a2ee-127">ContainsSubstring</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-128">Contains</span><span class="sxs-lookup"><span data-stu-id="8a2ee-128">Contains</span></span>](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-129">Наиболее тип фильтра для использования для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-129">The best filter type to use for string comparisons.</span></span> <span data-ttu-id="8a2ee-130">Позволяет управлять регистра, следует ли игнорировать пробел и устанавливать вложенности режим.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-130">It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="8a2ee-131">Битовая маска фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="8a2ee-132">ExcludesBitmask</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-133">Исключает</span><span class="sxs-lookup"><span data-stu-id="8a2ee-133">Excludes</span></span>](http://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-134">Можно найти целое число свойств как битовой маски и возвращать только результаты, соответствующий указанного Битовая маска, которая неопределенные битов.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="8a2ee-135">Существует ли фильтр</span><span class="sxs-lookup"><span data-stu-id="8a2ee-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-136">Существует</span><span class="sxs-lookup"><span data-stu-id="8a2ee-136">Exists</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-137">Существует</span><span class="sxs-lookup"><span data-stu-id="8a2ee-137">Exists</span></span>](http://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-138">Возвращает все элементы, которые имеют этот параметр указан, независимо от того, значение указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="8a2ee-139">Равенство фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-140">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-140">IsEqualTo</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8a2ee-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-141">IsNotEqualTo</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-142">Выражение IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-142">IsEqualTo</span></span>](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="8a2ee-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-143">IsNotEqualTo</span></span>](http://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-144">Сравнивает значение указанного свойства с указанным константа или значение другого свойства и возвращаются все элементы, которые имеют одинаковые значения (в случае фильтром **выражение IsEqualTo** ) или не равно значение (в случае **IsNotEqualTo **фильтр).</span><span class="sxs-lookup"><span data-stu-id="8a2ee-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="8a2ee-145">Реляционные тестирования фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="8a2ee-146">IsGreaterThan</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8a2ee-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-147">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8a2ee-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="8a2ee-148">IsLessThan</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8a2ee-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-149">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="8a2ee-150">IsGreaterThan</span></span>](http://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="8a2ee-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-151">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="8a2ee-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="8a2ee-152">IsLessThan</span></span>](http://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="8a2ee-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="8a2ee-153">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-154">Возвращает все элементы, для которых значение для указанного свойства в соответствующие отношения для указанного константа или другого свойства.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="8a2ee-155">К примеру фильтром **IsGreaterThan** возвращает все элементы, которые имеют значение, которое больше, чем значение, указанное в указанное свойство.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="8a2ee-156">Операция над значением фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-157">Не</span><span class="sxs-lookup"><span data-stu-id="8a2ee-157">Not</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-158">Не</span><span class="sxs-lookup"><span data-stu-id="8a2ee-158">Not</span></span>](http://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-159">Инвертирует результат другие фильтры.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="8a2ee-160">Составные фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="8a2ee-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="8a2ee-161">SearchFilterCollection</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8a2ee-162">И</span><span class="sxs-lookup"><span data-stu-id="8a2ee-162">And</span></span>](http://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="8a2ee-163">Или</span><span class="sxs-lookup"><span data-stu-id="8a2ee-163">Or</span></span>](http://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="8a2ee-164">Объединяет несколько фильтров, позволяя выполнять более сложные условия поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="8a2ee-165">Содержит фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-165">Contains filter</span></span>

<span data-ttu-id="8a2ee-166">Содержит объект фильтра — это лучший вариант для поиска свойства строки.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-166">A contains filter is the best choice for searching string properties.</span></span> <span data-ttu-id="8a2ee-167">С помощью содержит фильтра, можно управлять аспектами сравнения строк, таких как учет регистра букв и порядок обработки пробелы, задав вложенности режим и режим сравнения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-167">With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-168">Содержит фильтр в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="8a2ee-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-169"></span></span>

<span data-ttu-id="8a2ee-170">Если вы используете управляемый API веб-служб Exchange, режим вложения с помощью свойства [ContainmentMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) класса [ContainsSubstring](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) и задайте режим сравнения с помощью свойства [ComparisonMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) ** ContainsSubstring** класса.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="8a2ee-171">Следующем примере показано, как создать фильтр поиска, которая выполняет поиск поле темы элементов поиск подстроки «собрания».</span><span class="sxs-lookup"><span data-stu-id="8a2ee-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="8a2ee-172">В этом примере не учитывает регистр, но не пропускает пробелы.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
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

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="8a2ee-173">Содержит фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-173">Contains filter in EWS</span></span>
<span data-ttu-id="8a2ee-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-174"></span></span>

<span data-ttu-id="8a2ee-175">В веб-служб Exchange режим вложения с помощью атрибута **ContainmentMode** на элемент [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) и задайте режим сравнения с помощью атрибута **ContainmentComparison** на элемент **Contains** .</span><span class="sxs-lookup"><span data-stu-id="8a2ee-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="8a2ee-176">Следующем примере показано, как создать фильтр поиска для поиска в поле Тема элементов поиск подстроки «собрания».</span><span class="sxs-lookup"><span data-stu-id="8a2ee-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="8a2ee-177">В этом примере не учитывает регистр, но не пропускает пробелы.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="8a2ee-178">Битовая маска фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-178">Bitmask filter</span></span>

<span data-ttu-id="8a2ee-179">Битовая маска фильтра позволяет вам для поиска свойств целое число как битовой маски и возвращать результаты которой определенные биты не установлено в значение указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-180">Битовая маска фильтра в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-181">Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые имеют значение в настраиваемое свойство **ItemIndex** (определенные в [Пример: поиск элементов с помощью поисковый фильтр и управляемый API EWS](#bk_ExampleEWSMA) раздела этой статьи), не имеющие второй бит (10 в двоичном формате).</span><span class="sxs-lookup"><span data-stu-id="8a2ee-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
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

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="8a2ee-182">Битовая маска фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="8a2ee-183">Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые имеют значение в настраиваемое свойство **ItemIndex** (определенные в [Пример: поиск элементов с помощью поисковый фильтр и управляемый API EWS](#bk_ExampleEWSMA) этой статьи) у которых нет второй бит (10 в двоичном формате).</span><span class="sxs-lookup"><span data-stu-id="8a2ee-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="8a2ee-184">Существует ли фильтр</span><span class="sxs-lookup"><span data-stu-id="8a2ee-184">Exists filter</span></span>

<span data-ttu-id="8a2ee-185">Существует ли фильтр позволяет выполнять поиск для элементов, которые имеют определенное свойство задать для них, независимо от значения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-186">Существует ли фильтр в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-187">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют пользовательское свойство **ItemIndex** задать.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="8a2ee-188">Существует ли фильтр в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-188">Exists filter in EWS</span></span>

<span data-ttu-id="8a2ee-189">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют пользовательское свойство **ItemIndex** задать.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="8a2ee-190">Равенство фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-190">Equality filter</span></span>

<span data-ttu-id="8a2ee-191">Равенство фильтры позволяют выполнять поиск всех элементов, которые имеют значение для указанного свойства, определенное значение равно или не равно определенного значения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-191">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value.</span></span> <span data-ttu-id="8a2ee-192">Значение для сравнения с может быть константа или значение другого свойства для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-192">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-193">Равенство фильтр в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-194">Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые не будут прочитаны.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="8a2ee-195">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют значение в свойстве **ItemIndex** , не равно размер элемента.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="8a2ee-196">Равенство фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-196">Equality filter in EWS</span></span>

<span data-ttu-id="8a2ee-197">Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые не будут прочитаны.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="8a2ee-198">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют значение в свойстве **ItemIndex** , не равно размер элемента.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="8a2ee-199">Реляционные тестирования фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-199">Relational testing filter</span></span>

<span data-ttu-id="8a2ee-200">Реляционные тестирования фильтры позволяют выполнять поиск всех элементов, для которых значение в указанное свойство, которое соответствует любому из больше, чем (\>), больше или равно (\>=), меньше, чем (\<), или меньше или равно (\<=) заданным значением.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="8a2ee-201">Значение для сравнения с может быть константа или значение другого свойства для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-202">Реляционные тестирования фильтра в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-203">Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтров поиска для возвращения всех элементов со значением в свойства **ItemIndex** с указанного отношения константное значение 3.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
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

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="8a2ee-204">Реляционные тестирования фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="8a2ee-205">Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов со значением в свойство **ItemIndex** , больше, чем константное значение 3.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="8a2ee-206">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в **ItemIndex** свойства, которое больше или равно постоянным значением 3.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="8a2ee-207">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в свойство **ItemIndex** , меньше, чем константное значение 3.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="8a2ee-208">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в свойство **ItemIndex** , меньше или равно постоянным значением 3.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="8a2ee-209">Операция над значением фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-209">Negating filter</span></span>

<span data-ttu-id="8a2ee-210">Фильтр negating позволяет сведет другого фильтра и положительно результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-210">A negating filter enables you to negate another filter and get the opposite search results.</span></span> <span data-ttu-id="8a2ee-211">В то время как другие фильтры возврата результатов, соответствующих определенным условиям, negating фильтр возвращает результаты, которые не соответствуют условиям, указанным фильтр, который применяется к.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-211">While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-212">Операция над значением фильтра в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-213">Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, не связанные с подстроки «собрания» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="8a2ee-214">Операция над значением фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-214">Negating filter in EWS</span></span>

<span data-ttu-id="8a2ee-215">Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, не связанные с подстроки «собрания» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="8a2ee-216">Составные фильтра</span><span class="sxs-lookup"><span data-stu-id="8a2ee-216">Compound filter</span></span>

<span data-ttu-id="8a2ee-217">Составные фильтра позволяет объединять несколько фильтров для создания более сложного условия поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="8a2ee-218">Критерии, можно объединить с помощью логических операторов и и или.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="8a2ee-219">Таким образом можно выполнить поиск как «все сообщения из Sadie Daniels, содержащий «собрания» в теме».</span><span class="sxs-lookup"><span data-stu-id="8a2ee-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="8a2ee-220">Составные фильтр в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="8a2ee-221">Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска, которое возвращает все элементы, отправленные из Sadie Daniels и содержат «собрания» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="8a2ee-222">Составные фильтра в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-222">Compound filter in EWS</span></span>

<span data-ttu-id="8a2ee-223">Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска, которое возвращает все элементы, которые отправляются из Sadie Daniels и содержат «собрания» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="8a2ee-224">Пример: Поиск элементов с помощью поисковый фильтр и управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="8a2ee-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-225"></span></span>

<span data-ttu-id="8a2ee-226">Фильтры поиска использовать следующие методы управляемый API EWS:</span><span class="sxs-lookup"><span data-stu-id="8a2ee-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="8a2ee-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="8a2ee-227">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="8a2ee-228">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="8a2ee-228">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="8a2ee-229">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="8a2ee-229">Folder.FindFolders</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="8a2ee-230">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="8a2ee-230">Folder.FindItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="8a2ee-231">В следующем примере используется метод **ExchangeService.FindItems** ; Тем не менее же правила и основные понятия применяются ко всем методам.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="8a2ee-232">В следующем примере определяется метод с именем **SearchWithFilter** .</span><span class="sxs-lookup"><span data-stu-id="8a2ee-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="8a2ee-233">Принимает объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект [SearchFilter](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) как параметры.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-233">It takes an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="8a2ee-234">В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a2ee-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="8a2ee-235">Класс **SearchFilter** является базовым классом для всех различных поисковых фильтров.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
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

<span data-ttu-id="8a2ee-236">Эта функция с любыми поисковых фильтров, показано в примерах в этой статье.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-236">You can use this function with any of the search filters shown in the examples in this article.</span></span> <span data-ttu-id="8a2ee-237">В этом примере использует составные фильтр для возврата всех элементов в папке "Входящие" Sadie Daniels с «собрания» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-237">This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="8a2ee-238">Пример: Поиск элемента с помощью поисковый фильтр и веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="8a2ee-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-239"></span></span>

<span data-ttu-id="8a2ee-240">Фильтры поиска использовать следующие операции EWS:</span><span class="sxs-lookup"><span data-stu-id="8a2ee-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="8a2ee-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="8a2ee-241">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="8a2ee-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="8a2ee-242">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="8a2ee-243">В следующем примере используется операция **FindItem** ; Тем не менее же правил и концепции применить обе операции.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="8a2ee-244">Фильтры поиска содержатся в элементе [ограничения](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) запросов SOAP.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-244">Search filters are contained in the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="8a2ee-245">В этом примере отправляет запрос SOAP, который соответствует поиска, приведенные в предыдущем примере управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8a2ee-246">В следующем примере показано ответ от сервера, включая результаты поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="next-steps"></a><span data-ttu-id="8a2ee-247">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8a2ee-247">Next steps</span></span>
<span data-ttu-id="8a2ee-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="8a2ee-248"></span></span>

<span data-ttu-id="8a2ee-249">Теперь, когда вы знакомы с использованием поисковых фильтров в обычного поиска, можно перейти к более сложные приемы поиска.</span><span class="sxs-lookup"><span data-stu-id="8a2ee-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="8a2ee-250">Выполнение поиска по сгруппированных с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8a2ee-251">Выполнение поиска по выгружаемый с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="8a2ee-252">См. также</span><span class="sxs-lookup"><span data-stu-id="8a2ee-252">See also</span></span>

- [<span data-ttu-id="8a2ee-253">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="8a2ee-254">Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2ee-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="8a2ee-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="8a2ee-255">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="8a2ee-256">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="8a2ee-256">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="8a2ee-257">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="8a2ee-257">Folder.FindFolders</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="8a2ee-258">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="8a2ee-258">Folder.FindItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="8a2ee-259">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="8a2ee-259">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="8a2ee-260">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="8a2ee-260">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

