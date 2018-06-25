---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Элемент Contains представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761758"
---
# <a name="contains"></a><span data-ttu-id="cd128-103">Contains</span><span class="sxs-lookup"><span data-stu-id="cd128-103">Contains</span></span>

<span data-ttu-id="cd128-104">Элемент **Contains** представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.</span><span class="sxs-lookup"><span data-stu-id="cd128-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 <span data-ttu-id="cd128-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="cd128-105">**ContainsExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd128-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cd128-106">Attributes and elements</span></span>

<span data-ttu-id="cd128-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cd128-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd128-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cd128-108">Attributes</span></span>

|<span data-ttu-id="cd128-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cd128-109">**Attribute**</span></span>|<span data-ttu-id="cd128-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd128-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd128-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="cd128-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="cd128-112">Определяет границы поиска.</span><span class="sxs-lookup"><span data-stu-id="cd128-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="cd128-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="cd128-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="cd128-114">Определяет, будет ли поиска игнорироваться регистр и пробелы.</span><span class="sxs-lookup"><span data-stu-id="cd128-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="cd128-115">Значения атрибутов ContainmentMode</span><span class="sxs-lookup"><span data-stu-id="cd128-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="cd128-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cd128-116">**Value**</span></span>|<span data-ttu-id="cd128-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd128-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd128-118">FullString</span><span class="sxs-lookup"><span data-stu-id="cd128-118">FullString</span></span>  <br/> |<span data-ttu-id="cd128-119">Полной строки сравнивается константу.</span><span class="sxs-lookup"><span data-stu-id="cd128-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="cd128-120">Значение свойства и указанная константа, точно совпадают.</span><span class="sxs-lookup"><span data-stu-id="cd128-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="cd128-121">Префикс</span><span class="sxs-lookup"><span data-stu-id="cd128-121">Prefixed</span></span>  <br/> |<span data-ttu-id="cd128-122">Префикс строки сравнивается константу.</span><span class="sxs-lookup"><span data-stu-id="cd128-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="cd128-123">Подстроки</span><span class="sxs-lookup"><span data-stu-id="cd128-123">Substring</span></span>  <br/> |<span data-ttu-id="cd128-124">Подстрока строки сравнивается константу.</span><span class="sxs-lookup"><span data-stu-id="cd128-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="cd128-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="cd128-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="cd128-126">Префикс на отдельные слова в строке сравнивается константу.</span><span class="sxs-lookup"><span data-stu-id="cd128-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="cd128-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="cd128-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="cd128-128">Точной фразы в строке сравнивается константу.</span><span class="sxs-lookup"><span data-stu-id="cd128-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="cd128-129">Значения атрибутов ContainmentComparison</span><span class="sxs-lookup"><span data-stu-id="cd128-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="cd128-130">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cd128-130">**Value**</span></span>|<span data-ttu-id="cd128-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd128-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd128-132">Точное</span><span class="sxs-lookup"><span data-stu-id="cd128-132">Exact</span></span>  <br/> |<span data-ttu-id="cd128-133">Сравнение нужно ввести точно.</span><span class="sxs-lookup"><span data-stu-id="cd128-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="cd128-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="cd128-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="cd128-135">Сравнение не учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="cd128-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="cd128-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="cd128-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="cd128-137">Сравнение игнорирует дополнительный символов.</span><span class="sxs-lookup"><span data-stu-id="cd128-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="cd128-138">Слабый контроль</span><span class="sxs-lookup"><span data-stu-id="cd128-138">Loose</span></span>  <br/> |<span data-ttu-id="cd128-139">Требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="cd128-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cd128-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="cd128-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="cd128-141">Сравнение игнорирует строчных букв и дополнительный символов.</span><span class="sxs-lookup"><span data-stu-id="cd128-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="cd128-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="cd128-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="cd128-143">Требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="cd128-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cd128-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="cd128-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="cd128-145">Требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="cd128-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cd128-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="cd128-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="cd128-147">Требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="cd128-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cd128-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cd128-148">Child elements</span></span>

|<span data-ttu-id="cd128-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd128-149">**Element**</span></span>|<span data-ttu-id="cd128-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd128-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd128-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="cd128-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="cd128-152">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="cd128-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="cd128-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="cd128-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="cd128-154">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="cd128-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="cd128-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="cd128-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="cd128-156">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="cd128-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="cd128-157">Константы</span><span class="sxs-lookup"><span data-stu-id="cd128-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="cd128-158">Задает значение константы в качестве ограничения.</span><span class="sxs-lookup"><span data-stu-id="cd128-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd128-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cd128-159">Parent elements</span></span>

|<span data-ttu-id="cd128-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd128-160">**Element**</span></span>|<span data-ttu-id="cd128-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd128-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd128-162">Ограничения</span><span class="sxs-lookup"><span data-stu-id="cd128-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="cd128-163">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="cd128-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="cd128-164">Не</span><span class="sxs-lookup"><span data-stu-id="cd128-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="cd128-165">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="cd128-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="cd128-166">И</span><span class="sxs-lookup"><span data-stu-id="cd128-166">And</span></span>](and.md) <br/> |<span data-ttu-id="cd128-167">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="cd128-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="cd128-168">Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.</span><span class="sxs-lookup"><span data-stu-id="cd128-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="cd128-169">Или</span><span class="sxs-lookup"><span data-stu-id="cd128-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="cd128-170">Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="cd128-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="cd128-171">Элемент [или](or.md) возвращает **значение true** , если какие-либо из их дочерних элементов возвращало **значение true**.</span><span class="sxs-lookup"><span data-stu-id="cd128-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd128-172">Замечания</span><span class="sxs-lookup"><span data-stu-id="cd128-172">Remarks</span></span>

<span data-ttu-id="cd128-173">Атрибуты используются для определения сопоставления элементов.</span><span class="sxs-lookup"><span data-stu-id="cd128-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="cd128-174">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cd128-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd128-175">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cd128-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd128-176">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cd128-176">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd128-177">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cd128-177">Schema Name</span></span>  <br/> |<span data-ttu-id="cd128-178">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cd128-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd128-179">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cd128-179">Validation File</span></span>  <br/> |<span data-ttu-id="cd128-180">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd128-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd128-181">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cd128-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd128-182">False</span><span class="sxs-lookup"><span data-stu-id="cd128-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd128-183">См. также</span><span class="sxs-lookup"><span data-stu-id="cd128-183">See also</span></span>



- [<span data-ttu-id="cd128-184">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cd128-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

