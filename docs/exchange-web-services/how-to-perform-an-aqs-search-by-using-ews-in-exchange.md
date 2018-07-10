---
title: Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Узнайте, как выполнять поиск с помощью строки запроса и AQS в управляемый API EWS или приложение веб-служб Exchange.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761113"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="3214c-103">Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3214c-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="3214c-104">Узнайте, как выполнять поиск с помощью строки запроса и AQS в управляемый API EWS или приложение веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3214c-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="3214c-105">Строки запросов представляют альтернативой [поисковых фильтров](how-to-use-search-filters-with-ews-in-exchange.md) для выражения условия поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="3214c-106">Самое большое преимущество использования строк запросов — это, что не требуется указать отдельное свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="3214c-107">Только что можно указывать значение и поиска будут применяться для всех полей часто используемых элементов.</span><span class="sxs-lookup"><span data-stu-id="3214c-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="3214c-108">Также можно уточнить поиск с помощью расширенный синтаксис запроса (AQS) вместо простого значения.</span><span class="sxs-lookup"><span data-stu-id="3214c-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="3214c-109">Тем не менее строки запросов имеют следующие ограничения, которые следует обратить внимание перед добавлением к панели инструментов:</span><span class="sxs-lookup"><span data-stu-id="3214c-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="3214c-110">**Ограниченный возможность выполнять поиск в определенных свойств.**</span><span class="sxs-lookup"><span data-stu-id="3214c-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="3214c-111">При выполнении поиска с помощью простого значения в строку запроса, поиск выполняется по всем индексированные свойства.</span><span class="sxs-lookup"><span data-stu-id="3214c-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="3214c-112">Можно уточнить поиск для конкретного свойства, но свойства, доступные для использования в строку AQS ограничены.</span><span class="sxs-lookup"><span data-stu-id="3214c-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="3214c-113">Если свойство, которое вы хотите найти не соответствует ни одному из свойств, доступных для AQS, рекомендуется использовать фильтр поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="3214c-114">**Настраиваемые свойства не поиск.**</span><span class="sxs-lookup"><span data-stu-id="3214c-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="3214c-115">От индекса выполняется поиск строки запроса и настраиваемых свойств не включаются в этом индексе.</span><span class="sxs-lookup"><span data-stu-id="3214c-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="3214c-116">Если требуется выполнять поиск настраиваемые свойства, используйте фильтр поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="3214c-117">**Осуществляет поиск только элемент управления для строки.**</span><span class="sxs-lookup"><span data-stu-id="3214c-117">**Limited control for string searches.**</span></span> <span data-ttu-id="3214c-118">Поиск строки запроса всегда игнорировать регистр и всегда поиск подстрок.</span><span class="sxs-lookup"><span data-stu-id="3214c-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="3214c-119">Если вы собираетесь выполнить с учетом регистра, префикс или поиск точного совпадения, используйте фильтр поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="3214c-120">**Недоступно для папки или папки поиска.**</span><span class="sxs-lookup"><span data-stu-id="3214c-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="3214c-121">Операции веб-служб Exchange для поиска папок не поддерживает использование строки запроса.</span><span class="sxs-lookup"><span data-stu-id="3214c-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="3214c-122">Кроме того в папках поиска не поддерживают строки запроса.</span><span class="sxs-lookup"><span data-stu-id="3214c-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="3214c-123">В обоих случаях фильтр поиска является единственно возможный вариант.</span><span class="sxs-lookup"><span data-stu-id="3214c-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="3214c-124">Создание строки запроса</span><span class="sxs-lookup"><span data-stu-id="3214c-124">Creating a query string</span></span>
<span data-ttu-id="3214c-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="3214c-125"></span></span>

<span data-ttu-id="3214c-126">Строки запроса в управляемый API EWS и веб-служб Exchange, интерпретируются как подмножество AQS синтаксис.</span><span class="sxs-lookup"><span data-stu-id="3214c-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="3214c-127">Строки AQS состоят из значения или пары ключевых слов и значений, разделенных точкой с запятой (:).</span><span class="sxs-lookup"><span data-stu-id="3214c-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="3214c-128">Если значение указано без ключевое слово, все индексированные свойства выполняется поиск значения.</span><span class="sxs-lookup"><span data-stu-id="3214c-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="3214c-129">Если ключевое слово соединяться со значением, ключевое слово задает свойство для поиска соответствующего значения.</span><span class="sxs-lookup"><span data-stu-id="3214c-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="3214c-130">**В таблице 1. Поддерживаемые AQS ключевых слов**</span><span class="sxs-lookup"><span data-stu-id="3214c-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="3214c-131">**Ключевое слово**</span><span class="sxs-lookup"><span data-stu-id="3214c-131">**Keyword**</span></span>|<span data-ttu-id="3214c-132">**Value type**</span><span class="sxs-lookup"><span data-stu-id="3214c-132">**Value type**</span></span>|<span data-ttu-id="3214c-133">**Пример**</span><span class="sxs-lookup"><span data-stu-id="3214c-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3214c-134">subject</span><span class="sxs-lookup"><span data-stu-id="3214c-134">subject</span></span>  <br/> |<span data-ttu-id="3214c-135">String</span><span class="sxs-lookup"><span data-stu-id="3214c-135">String</span></span>  <br/> |<span data-ttu-id="3214c-136">Тема: проекта</span><span class="sxs-lookup"><span data-stu-id="3214c-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="3214c-137">body</span><span class="sxs-lookup"><span data-stu-id="3214c-137">body</span></span>  <br/> |<span data-ttu-id="3214c-138">String</span><span class="sxs-lookup"><span data-stu-id="3214c-138">String</span></span>  <br/> |<span data-ttu-id="3214c-139">графики BODY: продаж</span><span class="sxs-lookup"><span data-stu-id="3214c-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="3214c-140">вложение</span><span class="sxs-lookup"><span data-stu-id="3214c-140">attachment</span></span>  <br/> |<span data-ttu-id="3214c-141">String</span><span class="sxs-lookup"><span data-stu-id="3214c-141">String</span></span>  <br/> |<span data-ttu-id="3214c-142">вложения: отчет</span><span class="sxs-lookup"><span data-stu-id="3214c-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="3214c-143">to</span><span class="sxs-lookup"><span data-stu-id="3214c-143">to</span></span>  <br/> |<span data-ttu-id="3214c-144">String</span><span class="sxs-lookup"><span data-stu-id="3214c-144">String</span></span>  <br/> |<span data-ttu-id="3214c-145">Чтобы: «Sadie Daniels»</span><span class="sxs-lookup"><span data-stu-id="3214c-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="3214c-146">from</span><span class="sxs-lookup"><span data-stu-id="3214c-146">from</span></span>  <br/> |<span data-ttu-id="3214c-147">String</span><span class="sxs-lookup"><span data-stu-id="3214c-147">String</span></span>  <br/> |<span data-ttu-id="3214c-148">от: надеюсь,</span><span class="sxs-lookup"><span data-stu-id="3214c-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="3214c-149">cc</span><span class="sxs-lookup"><span data-stu-id="3214c-149">cc</span></span>  <br/> |<span data-ttu-id="3214c-150">String</span><span class="sxs-lookup"><span data-stu-id="3214c-150">String</span></span>  <br/> |<span data-ttu-id="3214c-151">Копия: «Ronnie Sturgis»</span><span class="sxs-lookup"><span data-stu-id="3214c-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="3214c-152">bcc</span><span class="sxs-lookup"><span data-stu-id="3214c-152">bcc</span></span>  <br/> |<span data-ttu-id="3214c-153">String</span><span class="sxs-lookup"><span data-stu-id="3214c-153">String</span></span>  <br/> |<span data-ttu-id="3214c-154">BCC:mack</span><span class="sxs-lookup"><span data-stu-id="3214c-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="3214c-155">participants</span><span class="sxs-lookup"><span data-stu-id="3214c-155">participants</span></span>  <br/> |<span data-ttu-id="3214c-156">String</span><span class="sxs-lookup"><span data-stu-id="3214c-156">String</span></span>  <br/> |<span data-ttu-id="3214c-157">Участники: sadie</span><span class="sxs-lookup"><span data-stu-id="3214c-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="3214c-158">category</span><span class="sxs-lookup"><span data-stu-id="3214c-158">category</span></span>  <br/> |<span data-ttu-id="3214c-159">String</span><span class="sxs-lookup"><span data-stu-id="3214c-159">String</span></span>  <br/> |<span data-ttu-id="3214c-160">Категория: проект</span><span class="sxs-lookup"><span data-stu-id="3214c-160">category:project</span></span>  <br/> |
|<span data-ttu-id="3214c-161">importance</span><span class="sxs-lookup"><span data-stu-id="3214c-161">importance</span></span>  <br/> |<span data-ttu-id="3214c-162">String</span><span class="sxs-lookup"><span data-stu-id="3214c-162">String</span></span>  <br/> |<span data-ttu-id="3214c-163">Важность: высокая</span><span class="sxs-lookup"><span data-stu-id="3214c-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="3214c-164">Тип</span><span class="sxs-lookup"><span data-stu-id="3214c-164">kind</span></span>  <br/> |<span data-ttu-id="3214c-165">Тип элемента</span><span class="sxs-lookup"><span data-stu-id="3214c-165">Item type</span></span>  <br/> |<span data-ttu-id="3214c-166">Тип: собрания</span><span class="sxs-lookup"><span data-stu-id="3214c-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="3214c-167">Отправленные</span><span class="sxs-lookup"><span data-stu-id="3214c-167">sent</span></span>  <br/> |<span data-ttu-id="3214c-168">Date</span><span class="sxs-lookup"><span data-stu-id="3214c-168">Date</span></span>  <br/> |<span data-ttu-id="3214c-169">отправлено: 12/10/2013</span><span class="sxs-lookup"><span data-stu-id="3214c-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="3214c-170">Получено</span><span class="sxs-lookup"><span data-stu-id="3214c-170">received</span></span>  <br/> |<span data-ttu-id="3214c-171">Date</span><span class="sxs-lookup"><span data-stu-id="3214c-171">Date</span></span>  <br/> |<span data-ttu-id="3214c-172">Получено: за вчерашний день</span><span class="sxs-lookup"><span data-stu-id="3214c-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="3214c-173">hasattachment</span><span class="sxs-lookup"><span data-stu-id="3214c-173">hasattachment</span></span>  <br/> |<span data-ttu-id="3214c-174">Логический</span><span class="sxs-lookup"><span data-stu-id="3214c-174">Boolean</span></span>  <br/> |<span data-ttu-id="3214c-175">Имеет вложение: true</span><span class="sxs-lookup"><span data-stu-id="3214c-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="3214c-176">помечен флажком|с флажком|с флагом</span><span class="sxs-lookup"><span data-stu-id="3214c-176">isflagged</span></span>  <br/> |<span data-ttu-id="3214c-177">Логический</span><span class="sxs-lookup"><span data-stu-id="3214c-177">Boolean</span></span>  <br/> |<span data-ttu-id="3214c-178">isflagged:true</span><span class="sxs-lookup"><span data-stu-id="3214c-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="3214c-179">isread</span><span class="sxs-lookup"><span data-stu-id="3214c-179">isread</span></span>  <br/> |<span data-ttu-id="3214c-180">Логический</span><span class="sxs-lookup"><span data-stu-id="3214c-180">Boolean</span></span>  <br/> |<span data-ttu-id="3214c-181">isread:false</span><span class="sxs-lookup"><span data-stu-id="3214c-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="3214c-182">size</span><span class="sxs-lookup"><span data-stu-id="3214c-182">size</span></span>  <br/> |<span data-ttu-id="3214c-183">Число</span><span class="sxs-lookup"><span data-stu-id="3214c-183">Number</span></span>  <br/> |<span data-ttu-id="3214c-184">Размер:\>5000</span><span class="sxs-lookup"><span data-stu-id="3214c-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="3214c-185">Давайте рассмотрим, как работают разных типов значений.</span><span class="sxs-lookup"><span data-stu-id="3214c-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="3214c-186">С помощью значение типа string</span><span class="sxs-lookup"><span data-stu-id="3214c-186">Using a string value type</span></span>

<span data-ttu-id="3214c-187">Типы строковое значение, по умолчанию, как поиск подстрок префикс, которые не учитывают регистр.</span><span class="sxs-lookup"><span data-stu-id="3214c-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="3214c-188">Который означает, что поиск Тема: проекта будет соответствовать любой из следующие темы:</span><span class="sxs-lookup"><span data-stu-id="3214c-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="3214c-189">Примечания к собранию проекта</span><span class="sxs-lookup"><span data-stu-id="3214c-189">Project meeting notes</span></span>
    
- <span data-ttu-id="3214c-190">У вас есть планов проектов?</span><span class="sxs-lookup"><span data-stu-id="3214c-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="3214c-191">Декабрь прогнозов продаж</span><span class="sxs-lookup"><span data-stu-id="3214c-191">December sales projections</span></span>
    
<span data-ttu-id="3214c-192">Вы можете изменить поиска, чтобы сделать обязательным наличие слово целиком, а не соответствующего префиксы введите строку в кавычки.</span><span class="sxs-lookup"><span data-stu-id="3214c-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="3214c-193">Поиск Тема: «project» не будет выполняться значение «Декабря прогнозов продаж» из списка соответствий.</span><span class="sxs-lookup"><span data-stu-id="3214c-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="3214c-194">Обратите внимание на то, что значение является по-прежнему без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="3214c-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="3214c-195">При использовании нескольких слов в строке запроса соответствие требуется, что оба слова отображаются в полях поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="3214c-196">Например поиск план Тема: проекта будет соответствующих следующие темы:</span><span class="sxs-lookup"><span data-stu-id="3214c-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="3214c-197">План проекта</span><span class="sxs-lookup"><span data-stu-id="3214c-197">Project plan</span></span>
    
- <span data-ttu-id="3214c-198">У вас есть планов проектов?</span><span class="sxs-lookup"><span data-stu-id="3214c-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="3214c-199">Отправлять мне план проекта</span><span class="sxs-lookup"><span data-stu-id="3214c-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="3214c-200">Планирование вех проекта</span><span class="sxs-lookup"><span data-stu-id="3214c-200">Planning project milestones</span></span>
    
<span data-ttu-id="3214c-201">Если несколько слов заключить в кавычки, они рассматриваются как одной фразы.</span><span class="sxs-lookup"><span data-stu-id="3214c-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="3214c-202">Поиск Тема: «план проекта» будет соответствовать только темы «План проекта» в предыдущем списке.</span><span class="sxs-lookup"><span data-stu-id="3214c-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="3214c-203">С помощью тип значение тип элемента</span><span class="sxs-lookup"><span data-stu-id="3214c-203">Using an item type value type</span></span>

<span data-ttu-id="3214c-204">Чтобы ограничить результаты поиска конкретным типом элемента, например, электронной почты или приглашений на собрания можно использовать следующие значения типа элемента с ключевым словом **вида** :</span><span class="sxs-lookup"><span data-stu-id="3214c-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="3214c-205">contacts</span><span class="sxs-lookup"><span data-stu-id="3214c-205">contacts</span></span>    
- <span data-ttu-id="3214c-206">документы</span><span class="sxs-lookup"><span data-stu-id="3214c-206">docs</span></span>    
- <span data-ttu-id="3214c-207">email</span><span class="sxs-lookup"><span data-stu-id="3214c-207">email</span></span>    
- <span data-ttu-id="3214c-208">факсы</span><span class="sxs-lookup"><span data-stu-id="3214c-208">faxes</span></span>    
- <span data-ttu-id="3214c-209">обмен мгновенными сообщениями (соответствует мгновенных сообщений)</span><span class="sxs-lookup"><span data-stu-id="3214c-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="3214c-210">журналы.</span><span class="sxs-lookup"><span data-stu-id="3214c-210">journals</span></span>    
- <span data-ttu-id="3214c-211">собрания (соответствует встреч и приглашений на собрания)</span><span class="sxs-lookup"><span data-stu-id="3214c-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="3214c-212">notes</span><span class="sxs-lookup"><span data-stu-id="3214c-212">notes</span></span>    
- <span data-ttu-id="3214c-213">posts</span><span class="sxs-lookup"><span data-stu-id="3214c-213">posts</span></span>    
- <span data-ttu-id="3214c-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="3214c-214">rssfeeds</span></span>    
- <span data-ttu-id="3214c-215">tasks</span><span class="sxs-lookup"><span data-stu-id="3214c-215">tasks</span></span>    
- <span data-ttu-id="3214c-216">Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="3214c-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="3214c-217">С помощью типа значения даты</span><span class="sxs-lookup"><span data-stu-id="3214c-217">Using a date value type</span></span>

<span data-ttu-id="3214c-218">Можно выполнить поиск типов значений даты в несколько различных способов.</span><span class="sxs-lookup"><span data-stu-id="3214c-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="3214c-219">Проще всего поиск в конкретный день.</span><span class="sxs-lookup"><span data-stu-id="3214c-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="3214c-220">Поиск с помощью полученных: 12/11/2013 вернет все элементы, полученного по 11 декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="3214c-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="3214c-221">Тем не менее можно также быть менее конкретным.</span><span class="sxs-lookup"><span data-stu-id="3214c-221">However, you can also be less specific.</span></span> <span data-ttu-id="3214c-222">Поиск с помощью полученных: 12/11 вернет все элементы, полученного по 11 декабря текущего года.</span><span class="sxs-lookup"><span data-stu-id="3214c-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="3214c-223">Другая возможность — это использование названия месяца.</span><span class="sxs-lookup"><span data-stu-id="3214c-223">Another option is to use the month names.</span></span> <span data-ttu-id="3214c-224">Можно выполнить поиск с помощью полученных: 11 декабря 2013 г. или 11 декабря для получения тех же результатов, получаемых: 12/11/2013 и полученных: 12/11, соответственно.</span><span class="sxs-lookup"><span data-stu-id="3214c-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="3214c-225">Можно также выполнить поиск с помощью полученных: Декабрь для получения всех элементов, полученных за месяц декабря в текущем году.</span><span class="sxs-lookup"><span data-stu-id="3214c-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="3214c-226">Использование названия дней недели является также параметр.</span><span class="sxs-lookup"><span data-stu-id="3214c-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="3214c-227">Поиск с помощью полученных: вторник вернет все элементы, полученного по вторник текущей недели.</span><span class="sxs-lookup"><span data-stu-id="3214c-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="3214c-228">Типы значения дат также поддерживает набор ключевых слов поиска относительно текущего времени.</span><span class="sxs-lookup"><span data-stu-id="3214c-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="3214c-229">Поддерживаются следующие ключевые слова:</span><span class="sxs-lookup"><span data-stu-id="3214c-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="3214c-230">today</span><span class="sxs-lookup"><span data-stu-id="3214c-230">today</span></span>  
- <span data-ttu-id="3214c-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="3214c-231">tomorrow</span></span>
- <span data-ttu-id="3214c-232">yesterday</span><span class="sxs-lookup"><span data-stu-id="3214c-232">yesterday</span></span>
- <span data-ttu-id="3214c-233">this week</span><span class="sxs-lookup"><span data-stu-id="3214c-233">this week</span></span>    
- <span data-ttu-id="3214c-234">На прошлой неделе</span><span class="sxs-lookup"><span data-stu-id="3214c-234">last week</span></span>    
- <span data-ttu-id="3214c-235">следующего месяца</span><span class="sxs-lookup"><span data-stu-id="3214c-235">next month</span></span>    
- <span data-ttu-id="3214c-236">последний месяц</span><span class="sxs-lookup"><span data-stu-id="3214c-236">past month</span></span>    
- <span data-ttu-id="3214c-237">следующий год</span><span class="sxs-lookup"><span data-stu-id="3214c-237">coming year</span></span>
    
<span data-ttu-id="3214c-238">Типов значений даты также необходимо сравнить с реляционные операторы, такие как больше или меньше, чем, или указанный диапазон с оператором диапазона **.**. Например, полученных:\>11/30/2013 отправлено:\>= за вчерашний день, и received:12/1/2013..today являются все строки допустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="3214c-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="3214c-239">С помощью типа логическое значение</span><span class="sxs-lookup"><span data-stu-id="3214c-239">Using a Boolean value type</span></span>

<span data-ttu-id="3214c-240">Типы логическое значение может быть «true» или «false».</span><span class="sxs-lookup"><span data-stu-id="3214c-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="3214c-241">Значения не учитывают регистр, поэтому isread:false будут создавать те же результаты, что isread:FALSE.</span><span class="sxs-lookup"><span data-stu-id="3214c-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="3214c-242">С помощью числовой тип значения</span><span class="sxs-lookup"><span data-stu-id="3214c-242">Using a number value type</span></span>

<span data-ttu-id="3214c-243">Числовой тип значение может быть выполнен как точного совпадения, но они могут также быть поиск с помощью реляционные операторы, такие как больше или меньше чем.</span><span class="sxs-lookup"><span data-stu-id="3214c-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="3214c-244">Например, размер: 10000 возвращает только элементы, которые имеют размер точно 10000 байт, но размер:\>= 10000 которого возвращаются элементы, которые имеют размер не менее 10000 в байтах.</span><span class="sxs-lookup"><span data-stu-id="3214c-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="3214c-245">Также можно указать диапазон, используя оператор диапазона ( ****.).</span><span class="sxs-lookup"><span data-stu-id="3214c-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="3214c-246">Например размер: 7000..8000 возвращает элементов, которые имеют размер от 7000 до 8000.</span><span class="sxs-lookup"><span data-stu-id="3214c-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="3214c-247">С помощью логических операторов</span><span class="sxs-lookup"><span data-stu-id="3214c-247">Using logical operators</span></span>

<span data-ttu-id="3214c-248">Строки запросов поддерживает следующие логические операторы.</span><span class="sxs-lookup"><span data-stu-id="3214c-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="3214c-249">**В таблице 2. Поддерживаемые логические операторы**</span><span class="sxs-lookup"><span data-stu-id="3214c-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="3214c-250">**Оператор**</span><span class="sxs-lookup"><span data-stu-id="3214c-250">**Operator**</span></span>|<span data-ttu-id="3214c-251">**�������**</span><span class="sxs-lookup"><span data-stu-id="3214c-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3214c-252">AND</span><span class="sxs-lookup"><span data-stu-id="3214c-252">AND</span></span>  <br/> |<span data-ttu-id="3214c-253">проект и от: «Sadie Daniels»</span><span class="sxs-lookup"><span data-stu-id="3214c-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="3214c-254">Тема:(project AND plan)</span><span class="sxs-lookup"><span data-stu-id="3214c-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="3214c-255">OR</span><span class="sxs-lookup"><span data-stu-id="3214c-255">OR</span></span>  <br/> |<span data-ttu-id="3214c-256">Тема: собрания или из: «Полная надеюсь»</span><span class="sxs-lookup"><span data-stu-id="3214c-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="3214c-257">от: ("Sadie Daniels" или "Надеюсь, полная")</span><span class="sxs-lookup"><span data-stu-id="3214c-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="3214c-258">NOT</span><span class="sxs-lookup"><span data-stu-id="3214c-258">NOT</span></span>  <br/> |<span data-ttu-id="3214c-259">НЕ от: «Ronnie Sturgis»</span><span class="sxs-lookup"><span data-stu-id="3214c-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="3214c-260">Получено: не сегодня</span><span class="sxs-lookup"><span data-stu-id="3214c-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="3214c-261">Обратите внимание на то, что можно использовать следующие операторы объединить несколько условий или объединить несколько значений в паре одного ключевое слово/значение.</span><span class="sxs-lookup"><span data-stu-id="3214c-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="3214c-262">Тем не менее при присоединении к несколько значений в паре одного ключевое слово/значение, следует использовать круглые скобки для обозначения несколько значений.</span><span class="sxs-lookup"><span data-stu-id="3214c-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="3214c-263">Чтобы понять, почему, рассмотрите возможность поиска в из: «Sadie Daniels» или «Надеюсь валовой».</span><span class="sxs-lookup"><span data-stu-id="3214c-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="3214c-264">В этом поиска фактически считается следующим критериям:</span><span class="sxs-lookup"><span data-stu-id="3214c-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="3214c-265">— Это элемент из Sadie Daniels, OR</span><span class="sxs-lookup"><span data-stu-id="3214c-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="3214c-266">Элемент содержит фразу «Полная надеюсь» в индексированные свойства.</span><span class="sxs-lookup"><span data-stu-id="3214c-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="3214c-267">С другой стороны, из: ("Sadie Daniels" или "Полная надеюсь") обрабатывается как:</span><span class="sxs-lookup"><span data-stu-id="3214c-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="3214c-268">— Это элемент из Sadie Daniels, OR</span><span class="sxs-lookup"><span data-stu-id="3214c-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="3214c-269">— Это элемент из надеюсь полная</span><span class="sxs-lookup"><span data-stu-id="3214c-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="3214c-270">— Это оператор по умолчанию при нескольких условия, но не логический оператор, который включен и.</span><span class="sxs-lookup"><span data-stu-id="3214c-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="3214c-271">Например имеет вложение: true Тема: project эквивалентен имеет: вложения: true и Тема: проекта.</span><span class="sxs-lookup"><span data-stu-id="3214c-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="3214c-272">Пример: Поиск элементов с помощью строки запроса и управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="3214c-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="3214c-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="3214c-273"></span></span>

<span data-ttu-id="3214c-274">В следующем примере определяется метод с именем **SearchWithQueryString** .</span><span class="sxs-lookup"><span data-stu-id="3214c-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="3214c-275">Требуется объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект **string** , представляющий строки запроса в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="3214c-275">It takes an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="3214c-276">В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3214c-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

<span data-ttu-id="3214c-277">Этот метод можно использовать для поиска всех элементов с фразой «план проекта» в теме сообщения, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="3214c-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="3214c-278">Пример: Поиск элементов с помощью строки запроса и веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="3214c-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="3214c-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="3214c-279"></span></span>

<span data-ttu-id="3214c-280">В этом примере запрос SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) выполняется поиск всех элементов в папке "Входящие" с фразой «план проекта» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="3214c-280">In this example, a SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3214c-281">В следующем примере показано ответ от сервера с результатами поиска.</span><span class="sxs-lookup"><span data-stu-id="3214c-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="3214c-282">См. также</span><span class="sxs-lookup"><span data-stu-id="3214c-282">See also</span></span>

- [<span data-ttu-id="3214c-283">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="3214c-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="3214c-284">Используйте фильтры поиска с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3214c-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="3214c-285">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="3214c-285">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="3214c-286">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="3214c-286">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

