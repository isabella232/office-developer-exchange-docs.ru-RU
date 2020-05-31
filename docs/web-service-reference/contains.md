---
title: Хранится
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
description: Элемент Contains представляет выражение поиска, которое определяет, содержит ли данное свойство предоставленное значение константы String.
ms.openlocfilehash: b25b69aadf2c331527a17ad81ed46f61aa7b93c2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354290"
---
# <a name="contains"></a><span data-ttu-id="cb55a-103">Хранится</span><span class="sxs-lookup"><span data-stu-id="cb55a-103">Contains</span></span>

<span data-ttu-id="cb55a-104">Элемент **Contains** представляет выражение поиска, которое определяет, содержит ли данное свойство предоставленное значение константы String.</span><span class="sxs-lookup"><span data-stu-id="cb55a-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


<span data-ttu-id="cb55a-105">**контаинсекспрессионтипе**</span><span class="sxs-lookup"><span data-stu-id="cb55a-105">**ContainsExpressionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cb55a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cb55a-106">Attributes and elements</span></span>

<span data-ttu-id="cb55a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cb55a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb55a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cb55a-108">Attributes</span></span>

|<span data-ttu-id="cb55a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cb55a-109">**Attribute**</span></span>|<span data-ttu-id="cb55a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb55a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb55a-111">**контаинментмоде**</span><span class="sxs-lookup"><span data-stu-id="cb55a-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="cb55a-112">Определяет границы поиска.</span><span class="sxs-lookup"><span data-stu-id="cb55a-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="cb55a-113">**контаинменткомпарисон**</span><span class="sxs-lookup"><span data-stu-id="cb55a-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="cb55a-114">Определяет, будут ли при поиске игнорироваться регистры и пробелы.</span><span class="sxs-lookup"><span data-stu-id="cb55a-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="cb55a-115">Значения атрибутов Контаинментмоде</span><span class="sxs-lookup"><span data-stu-id="cb55a-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="cb55a-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cb55a-116">**Value**</span></span>|<span data-ttu-id="cb55a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb55a-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb55a-118">фуллстринг</span><span class="sxs-lookup"><span data-stu-id="cb55a-118">FullString</span></span>  <br/> |<span data-ttu-id="cb55a-119">Между полной строкой и константой выполняется сравнение.</span><span class="sxs-lookup"><span data-stu-id="cb55a-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="cb55a-120">Значение свойства и заданная константа в точности совпадают.</span><span class="sxs-lookup"><span data-stu-id="cb55a-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="cb55a-121">Префиксом</span><span class="sxs-lookup"><span data-stu-id="cb55a-121">Prefixed</span></span>  <br/> |<span data-ttu-id="cb55a-122">Сравнение между префиксом строки и константой.</span><span class="sxs-lookup"><span data-stu-id="cb55a-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="cb55a-123">Подстроку</span><span class="sxs-lookup"><span data-stu-id="cb55a-123">Substring</span></span>  <br/> |<span data-ttu-id="cb55a-124">Сравнение между подстрокой строки и константой.</span><span class="sxs-lookup"><span data-stu-id="cb55a-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="cb55a-125">префиксонвордс</span><span class="sxs-lookup"><span data-stu-id="cb55a-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="cb55a-126">В качестве префикса для отдельных слов в строке и константы используется сравнение.</span><span class="sxs-lookup"><span data-stu-id="cb55a-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="cb55a-127">ексактфрасе</span><span class="sxs-lookup"><span data-stu-id="cb55a-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="cb55a-128">Точная фраза в строке и константа сравнивается.</span><span class="sxs-lookup"><span data-stu-id="cb55a-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="cb55a-129">Значения атрибутов Контаинменткомпарисон</span><span class="sxs-lookup"><span data-stu-id="cb55a-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="cb55a-130">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cb55a-130">**Value**</span></span>|<span data-ttu-id="cb55a-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb55a-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb55a-132">Интересующ</span><span class="sxs-lookup"><span data-stu-id="cb55a-132">Exact</span></span>  <br/> |<span data-ttu-id="cb55a-133">Сравнение должно быть точным.</span><span class="sxs-lookup"><span data-stu-id="cb55a-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="cb55a-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="cb55a-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="cb55a-135">При сравнении регистр игнорируется.</span><span class="sxs-lookup"><span data-stu-id="cb55a-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="cb55a-136">игноренонспаЦингчарактерс</span><span class="sxs-lookup"><span data-stu-id="cb55a-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="cb55a-137">При сравнении не учитываются пробелы.</span><span class="sxs-lookup"><span data-stu-id="cb55a-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="cb55a-138">Свободное</span><span class="sxs-lookup"><span data-stu-id="cb55a-138">Loose</span></span>  <br/> |<span data-ttu-id="cb55a-139">Для удаления.</span><span class="sxs-lookup"><span data-stu-id="cb55a-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cb55a-140">игнорекасеанднонспаЦингчарактерс</span><span class="sxs-lookup"><span data-stu-id="cb55a-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="cb55a-141">При сравнении игнорируются символы с разделителями и символы, отличные от пробелов.</span><span class="sxs-lookup"><span data-stu-id="cb55a-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="cb55a-142">лусеандигнорекасе</span><span class="sxs-lookup"><span data-stu-id="cb55a-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="cb55a-143">Для удаления.</span><span class="sxs-lookup"><span data-stu-id="cb55a-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cb55a-144">лусеандигноренонспаце</span><span class="sxs-lookup"><span data-stu-id="cb55a-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="cb55a-145">Для удаления.</span><span class="sxs-lookup"><span data-stu-id="cb55a-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="cb55a-146">лусеандигнорекасеандигноренонспаце</span><span class="sxs-lookup"><span data-stu-id="cb55a-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="cb55a-147">Для удаления.</span><span class="sxs-lookup"><span data-stu-id="cb55a-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cb55a-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cb55a-148">Child elements</span></span>

|<span data-ttu-id="cb55a-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb55a-149">**Element**</span></span>|<span data-ttu-id="cb55a-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb55a-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb55a-151">фиелдури</span><span class="sxs-lookup"><span data-stu-id="cb55a-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="cb55a-152">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="cb55a-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-153">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="cb55a-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="cb55a-154">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="cb55a-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-155">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="cb55a-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="cb55a-156">Определяет свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="cb55a-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-157">Константа</span><span class="sxs-lookup"><span data-stu-id="cb55a-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="cb55a-158">Определяет постоянное значение в ограничении.</span><span class="sxs-lookup"><span data-stu-id="cb55a-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb55a-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cb55a-159">Parent elements</span></span>

|<span data-ttu-id="cb55a-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb55a-160">**Element**</span></span>|<span data-ttu-id="cb55a-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb55a-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb55a-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="cb55a-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="cb55a-163">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="cb55a-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-164">Not</span><span class="sxs-lookup"><span data-stu-id="cb55a-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="cb55a-165">Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="cb55a-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-166">And</span><span class="sxs-lookup"><span data-stu-id="cb55a-166">And</span></span>](and.md) <br/> |<span data-ttu-id="cb55a-167">Представляет выражение поиска, которое позволяет выполнять логическую операцию и операцию между двумя или более выражениями поиска.</span><span class="sxs-lookup"><span data-stu-id="cb55a-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="cb55a-168">Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.</span><span class="sxs-lookup"><span data-stu-id="cb55a-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="cb55a-169">Or</span><span class="sxs-lookup"><span data-stu-id="cb55a-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="cb55a-170">Представляет выражение поиска, которое выполняет операцию логического или для содержащегося в нем выражения поиска.</span><span class="sxs-lookup"><span data-stu-id="cb55a-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="cb55a-171">Элемент [or](or.md) возвращает **значение true** , если любой из дочерних элементов возвращает **значение true**.</span><span class="sxs-lookup"><span data-stu-id="cb55a-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb55a-172">Примечания</span><span class="sxs-lookup"><span data-stu-id="cb55a-172">Remarks</span></span>

<span data-ttu-id="cb55a-173">Атрибуты используются для определения способа сравнения элементов.</span><span class="sxs-lookup"><span data-stu-id="cb55a-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="cb55a-174">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cb55a-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb55a-175">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cb55a-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb55a-176">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cb55a-176">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb55a-177">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cb55a-177">Schema Name</span></span>  <br/> |<span data-ttu-id="cb55a-178">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cb55a-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb55a-179">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cb55a-179">Validation File</span></span>  <br/> |<span data-ttu-id="cb55a-180">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cb55a-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb55a-181">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cb55a-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb55a-182">False</span><span class="sxs-lookup"><span data-stu-id="cb55a-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb55a-183">См. также</span><span class="sxs-lookup"><span data-stu-id="cb55a-183">See also</span></span>

- [<span data-ttu-id="cb55a-184">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cb55a-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

