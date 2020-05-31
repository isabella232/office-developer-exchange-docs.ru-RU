---
title: Выполнение поиска AQS с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Узнайте, как выполнять поиск с помощью строк запросов и AQS в управляемом API EWS или приложении EWS.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761113"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="f14cb-103">Выполнение поиска AQS с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f14cb-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="f14cb-104">Узнайте, как выполнять поиск с помощью строк запросов и AQS в управляемом API EWS или приложении EWS.</span><span class="sxs-lookup"><span data-stu-id="f14cb-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="f14cb-105">Строки запросов предоставляют альтернативу [фильтрам поиска](how-to-use-search-filters-with-ews-in-exchange.md) для задания условий поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="f14cb-106">Крупнейшим преимуществом для использования строк запросов является то, что не требуется указывать одно свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="f14cb-107">Можно просто указать значение, и поиск будет применяться ко всем часто используемым полям элементов.</span><span class="sxs-lookup"><span data-stu-id="f14cb-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="f14cb-108">Вы также можете уточнить поиск с помощью расширенного синтаксиса запросов (AQS), а не простого значения.</span><span class="sxs-lookup"><span data-stu-id="f14cb-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="f14cb-109">Однако строки запросов имеют следующие ограничения, которые необходимо знать перед их добавлением на панель элементов:</span><span class="sxs-lookup"><span data-stu-id="f14cb-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="f14cb-110">**Ограниченная возможность поиска определенных свойств.**</span><span class="sxs-lookup"><span data-stu-id="f14cb-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="f14cb-111">При поиске с простым значением в строке запроса выполняется поиск по всем индексированным свойствам.</span><span class="sxs-lookup"><span data-stu-id="f14cb-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="f14cb-112">Вы можете уточнить поиск по определенным свойствам, но свойства, доступные для использования в строке AQS, ограничены.</span><span class="sxs-lookup"><span data-stu-id="f14cb-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="f14cb-113">Если свойство, которое вы хотите найти, не является одним из свойств, доступных для AQS, рассмотрите возможность использования фильтра поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="f14cb-114">**Не выполняется поиск настраиваемых свойств.**</span><span class="sxs-lookup"><span data-stu-id="f14cb-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="f14cb-115">Поиск строки запроса выполняется по индексу, а настраиваемые свойства не включены в этот индекс.</span><span class="sxs-lookup"><span data-stu-id="f14cb-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="f14cb-116">Если вам нужно искать настраиваемые свойства, используйте фильтр поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="f14cb-117">**Ограниченный элемент управления для поиска по строкам.**</span><span class="sxs-lookup"><span data-stu-id="f14cb-117">**Limited control for string searches.**</span></span> <span data-ttu-id="f14cb-118">Поиск строки запроса всегда игнорирует регистр и всегда выполняет поиск в подстроках.</span><span class="sxs-lookup"><span data-stu-id="f14cb-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="f14cb-119">Если вы хотите выполнять поиск с учетом регистра, префикса или точного совпадения, используйте фильтр поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="f14cb-120">**Недоступно для папок или папок поиска.**</span><span class="sxs-lookup"><span data-stu-id="f14cb-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="f14cb-121">Операции EWS для поиска папок не поддерживаются с помощью строки запроса.</span><span class="sxs-lookup"><span data-stu-id="f14cb-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="f14cb-122">Кроме того, папки поиска не поддерживают строки запросов.</span><span class="sxs-lookup"><span data-stu-id="f14cb-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="f14cb-123">В обоих случаях фильтр поиска является единственным вариантом.</span><span class="sxs-lookup"><span data-stu-id="f14cb-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="f14cb-124">Создание строки запроса</span><span class="sxs-lookup"><span data-stu-id="f14cb-124">Creating a query string</span></span>
<span data-ttu-id="f14cb-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="f14cb-125"><a name="bk_CreateQueryString"> </a></span></span>

<span data-ttu-id="f14cb-126">Строки запросов в управляемом API EWS и EWS интерпретируются как подмножество синтаксиса AQS.</span><span class="sxs-lookup"><span data-stu-id="f14cb-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="f14cb-127">Строки AQS состоят из пар "значения" или "ключевое слово/значение", разделенных двоеточием (:).</span><span class="sxs-lookup"><span data-stu-id="f14cb-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="f14cb-128">Если значение задано без ключевого слова, выполняется поиск по всем индексированным свойствам.</span><span class="sxs-lookup"><span data-stu-id="f14cb-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="f14cb-129">Если ключевое слово связанно со значением, ключевое слово указывает свойство для поиска соответствующего значения.</span><span class="sxs-lookup"><span data-stu-id="f14cb-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="f14cb-130">**Таблица 1. Поддерживаемые ключевые слова AQS**</span><span class="sxs-lookup"><span data-stu-id="f14cb-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="f14cb-131">**Недопустим**</span><span class="sxs-lookup"><span data-stu-id="f14cb-131">**Keyword**</span></span>|<span data-ttu-id="f14cb-132">**Тип значения**</span><span class="sxs-lookup"><span data-stu-id="f14cb-132">**Value type**</span></span>|<span data-ttu-id="f14cb-133">**Пример**</span><span class="sxs-lookup"><span data-stu-id="f14cb-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f14cb-134">subject</span><span class="sxs-lookup"><span data-stu-id="f14cb-134">subject</span></span>  <br/> |<span data-ttu-id="f14cb-135">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-135">String</span></span>  <br/> |<span data-ttu-id="f14cb-136">Тема: Project</span><span class="sxs-lookup"><span data-stu-id="f14cb-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="f14cb-137">body</span><span class="sxs-lookup"><span data-stu-id="f14cb-137">body</span></span>  <br/> |<span data-ttu-id="f14cb-138">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-138">String</span></span>  <br/> |<span data-ttu-id="f14cb-139">текст: данные о продажах</span><span class="sxs-lookup"><span data-stu-id="f14cb-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="f14cb-140">attachment</span><span class="sxs-lookup"><span data-stu-id="f14cb-140">attachment</span></span>  <br/> |<span data-ttu-id="f14cb-141">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-141">String</span></span>  <br/> |<span data-ttu-id="f14cb-142">вложение: отчет</span><span class="sxs-lookup"><span data-stu-id="f14cb-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="f14cb-143">to</span><span class="sxs-lookup"><span data-stu-id="f14cb-143">to</span></span>  <br/> |<span data-ttu-id="f14cb-144">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-144">String</span></span>  <br/> |<span data-ttu-id="f14cb-145">Кому: "Ольга Даниелс"</span><span class="sxs-lookup"><span data-stu-id="f14cb-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="f14cb-146">from</span><span class="sxs-lookup"><span data-stu-id="f14cb-146">from</span></span>  <br/> |<span data-ttu-id="f14cb-147">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-147">String</span></span>  <br/> |<span data-ttu-id="f14cb-148">от: надеюсь</span><span class="sxs-lookup"><span data-stu-id="f14cb-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="f14cb-149">копия;</span><span class="sxs-lookup"><span data-stu-id="f14cb-149">cc</span></span>  <br/> |<span data-ttu-id="f14cb-150">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-150">String</span></span>  <br/> |<span data-ttu-id="f14cb-151">CC: "ронние Стургис"</span><span class="sxs-lookup"><span data-stu-id="f14cb-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="f14cb-152">СК.</span><span class="sxs-lookup"><span data-stu-id="f14cb-152">bcc</span></span>  <br/> |<span data-ttu-id="f14cb-153">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-153">String</span></span>  <br/> |<span data-ttu-id="f14cb-154">СК: МАКК</span><span class="sxs-lookup"><span data-stu-id="f14cb-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="f14cb-155">participants</span><span class="sxs-lookup"><span data-stu-id="f14cb-155">participants</span></span>  <br/> |<span data-ttu-id="f14cb-156">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-156">String</span></span>  <br/> |<span data-ttu-id="f14cb-157">Участники: Ольга</span><span class="sxs-lookup"><span data-stu-id="f14cb-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="f14cb-158">category</span><span class="sxs-lookup"><span data-stu-id="f14cb-158">category</span></span>  <br/> |<span data-ttu-id="f14cb-159">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-159">String</span></span>  <br/> |<span data-ttu-id="f14cb-160">Категория: Project</span><span class="sxs-lookup"><span data-stu-id="f14cb-160">category:project</span></span>  <br/> |
|<span data-ttu-id="f14cb-161">importance</span><span class="sxs-lookup"><span data-stu-id="f14cb-161">importance</span></span>  <br/> |<span data-ttu-id="f14cb-162">String</span><span class="sxs-lookup"><span data-stu-id="f14cb-162">String</span></span>  <br/> |<span data-ttu-id="f14cb-163">importance:high</span><span class="sxs-lookup"><span data-stu-id="f14cb-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="f14cb-164">kind</span><span class="sxs-lookup"><span data-stu-id="f14cb-164">kind</span></span>  <br/> |<span data-ttu-id="f14cb-165">Тип элемента</span><span class="sxs-lookup"><span data-stu-id="f14cb-165">Item type</span></span>  <br/> |<span data-ttu-id="f14cb-166">вид: собрания</span><span class="sxs-lookup"><span data-stu-id="f14cb-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="f14cb-167">sent</span><span class="sxs-lookup"><span data-stu-id="f14cb-167">sent</span></span>  <br/> |<span data-ttu-id="f14cb-168">Дата</span><span class="sxs-lookup"><span data-stu-id="f14cb-168">Date</span></span>  <br/> |<span data-ttu-id="f14cb-169">Отправлено: 12/10/2013</span><span class="sxs-lookup"><span data-stu-id="f14cb-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="f14cb-170">received</span><span class="sxs-lookup"><span data-stu-id="f14cb-170">received</span></span>  <br/> |<span data-ttu-id="f14cb-171">Дата</span><span class="sxs-lookup"><span data-stu-id="f14cb-171">Date</span></span>  <br/> |<span data-ttu-id="f14cb-172">получено: вчера</span><span class="sxs-lookup"><span data-stu-id="f14cb-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="f14cb-173">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="f14cb-173">hasattachment</span></span>  <br/> |<span data-ttu-id="f14cb-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f14cb-174">Boolean</span></span>  <br/> |<span data-ttu-id="f14cb-175">Имеет вложение: true</span><span class="sxs-lookup"><span data-stu-id="f14cb-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="f14cb-176">с пометкой</span><span class="sxs-lookup"><span data-stu-id="f14cb-176">isflagged</span></span>  <br/> |<span data-ttu-id="f14cb-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="f14cb-177">Boolean</span></span>  <br/> |<span data-ttu-id="f14cb-178">с пометкой: истина</span><span class="sxs-lookup"><span data-stu-id="f14cb-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="f14cb-179">IsRead</span><span class="sxs-lookup"><span data-stu-id="f14cb-179">isread</span></span>  <br/> |<span data-ttu-id="f14cb-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f14cb-180">Boolean</span></span>  <br/> |<span data-ttu-id="f14cb-181">чтение: false</span><span class="sxs-lookup"><span data-stu-id="f14cb-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="f14cb-182">size</span><span class="sxs-lookup"><span data-stu-id="f14cb-182">size</span></span>  <br/> |<span data-ttu-id="f14cb-183">Номер</span><span class="sxs-lookup"><span data-stu-id="f14cb-183">Number</span></span>  <br/> |<span data-ttu-id="f14cb-184">Размер:\>5000</span><span class="sxs-lookup"><span data-stu-id="f14cb-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="f14cb-185">Давайте посмотрим, как работают различные типы значений.</span><span class="sxs-lookup"><span data-stu-id="f14cb-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="f14cb-186">Использование типа строковых значений</span><span class="sxs-lookup"><span data-stu-id="f14cb-186">Using a string value type</span></span>

<span data-ttu-id="f14cb-187">Типы строковых значений по умолчанию выполняют поиск в виде префикса подстроки без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="f14cb-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="f14cb-188">Это означает, что поиск темы: Project соответствует любой из следующих субъектов:</span><span class="sxs-lookup"><span data-stu-id="f14cb-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="f14cb-189">Заметки к собранию проекта</span><span class="sxs-lookup"><span data-stu-id="f14cb-189">Project meeting notes</span></span>
    
- <span data-ttu-id="f14cb-190">У вас есть планы проекта?</span><span class="sxs-lookup"><span data-stu-id="f14cb-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="f14cb-191">Проекции продаж за Декабрь</span><span class="sxs-lookup"><span data-stu-id="f14cb-191">December sales projections</span></span>
    
<span data-ttu-id="f14cb-192">Вы можете изменить поиск так, чтобы он затребовал целое слово, а не сопоставленные префиксы, заключив строку в кавычки.</span><span class="sxs-lookup"><span data-stu-id="f14cb-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="f14cb-193">Поиск темы: "Project" исключит значение "предпродажные проекции" из списка совпадений.</span><span class="sxs-lookup"><span data-stu-id="f14cb-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="f14cb-194">Обратите внимание, что значение по-прежнему не зависит от регистра.</span><span class="sxs-lookup"><span data-stu-id="f14cb-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="f14cb-195">Если вы используете несколько слов в строке запроса, для сравнения необходимо, чтобы оба слова отображались в полях поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="f14cb-196">Например, Поиск темы: план проекта будет соотнесен с любой из следующих субъектов:</span><span class="sxs-lookup"><span data-stu-id="f14cb-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="f14cb-197">План проекта</span><span class="sxs-lookup"><span data-stu-id="f14cb-197">Project plan</span></span>
    
- <span data-ttu-id="f14cb-198">У вас есть планы проекта?</span><span class="sxs-lookup"><span data-stu-id="f14cb-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="f14cb-199">Отправьте мне план проекта.</span><span class="sxs-lookup"><span data-stu-id="f14cb-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="f14cb-200">Планирование вех проекта</span><span class="sxs-lookup"><span data-stu-id="f14cb-200">Planning project milestones</span></span>
    
<span data-ttu-id="f14cb-201">Если вы заключаете несколько слов в кавычки, они рассматриваются как одна фраза.</span><span class="sxs-lookup"><span data-stu-id="f14cb-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="f14cb-202">Поиск темы: "план проекта" будет сопоставлен только теме "план проекта" из предыдущего списка.</span><span class="sxs-lookup"><span data-stu-id="f14cb-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="f14cb-203">Использование типа значения типа элемента</span><span class="sxs-lookup"><span data-stu-id="f14cb-203">Using an item type value type</span></span>

<span data-ttu-id="f14cb-204">Вы можете использовать следующие значения типа элементов с ключевым словом **Kind** , чтобы ограничить результаты поиска только определенным типом элемента, например адресами электронной почты или приглашения на собрания:</span><span class="sxs-lookup"><span data-stu-id="f14cb-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="f14cb-205">contacts</span><span class="sxs-lookup"><span data-stu-id="f14cb-205">contacts</span></span>    
- <span data-ttu-id="f14cb-206">docs</span><span class="sxs-lookup"><span data-stu-id="f14cb-206">docs</span></span>    
- <span data-ttu-id="f14cb-207">email</span><span class="sxs-lookup"><span data-stu-id="f14cb-207">email</span></span>    
- <span data-ttu-id="f14cb-208">faxes</span><span class="sxs-lookup"><span data-stu-id="f14cb-208">faxes</span></span>    
- <span data-ttu-id="f14cb-209">Обмен мгновенными сообщениями (соответствует мгновенным сообщениям)</span><span class="sxs-lookup"><span data-stu-id="f14cb-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="f14cb-210">journals</span><span class="sxs-lookup"><span data-stu-id="f14cb-210">journals</span></span>    
- <span data-ttu-id="f14cb-211">собрания (соответствуют приглашениям на встречи и собрания);</span><span class="sxs-lookup"><span data-stu-id="f14cb-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="f14cb-212">notes</span><span class="sxs-lookup"><span data-stu-id="f14cb-212">notes</span></span>    
- <span data-ttu-id="f14cb-213">posts</span><span class="sxs-lookup"><span data-stu-id="f14cb-213">posts</span></span>    
- <span data-ttu-id="f14cb-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="f14cb-214">rssfeeds</span></span>    
- <span data-ttu-id="f14cb-215">tasks</span><span class="sxs-lookup"><span data-stu-id="f14cb-215">tasks</span></span>    
- <span data-ttu-id="f14cb-216">voicemail</span><span class="sxs-lookup"><span data-stu-id="f14cb-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="f14cb-217">Использование типа значения Date</span><span class="sxs-lookup"><span data-stu-id="f14cb-217">Using a date value type</span></span>

<span data-ttu-id="f14cb-218">Типы значений даты можно искать несколькими различными способами.</span><span class="sxs-lookup"><span data-stu-id="f14cb-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="f14cb-219">Самый простой способ найти определенную дату.</span><span class="sxs-lookup"><span data-stu-id="f14cb-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="f14cb-220">При поиске с полученным сообщением: 12/11/2013 возвращает все элементы, полученные на 11 декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="f14cb-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="f14cb-221">Однако вы также можете использовать менее конкретные особенности.</span><span class="sxs-lookup"><span data-stu-id="f14cb-221">However, you can also be less specific.</span></span> <span data-ttu-id="f14cb-222">Поиск с полученным: 12/11 возвращает все элементы, полученные на 11 декабря текущего года.</span><span class="sxs-lookup"><span data-stu-id="f14cb-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="f14cb-223">Кроме того, можно использовать названия месяцев.</span><span class="sxs-lookup"><span data-stu-id="f14cb-223">Another option is to use the month names.</span></span> <span data-ttu-id="f14cb-224">Вы можете выполнять поиск с помощью Received: 11 декабря 2013 или 11 декабря, чтобы получить те же результаты, что и получено: 12/11/2013 и получено: 12/11, соответственно.</span><span class="sxs-lookup"><span data-stu-id="f14cb-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="f14cb-225">Вы также можете выполнять поиск с помощью Received: Декабрь для получения всех элементов, полученных в декабре, в текущем году.</span><span class="sxs-lookup"><span data-stu-id="f14cb-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="f14cb-226">Использование названий дней недели также является параметром.</span><span class="sxs-lookup"><span data-stu-id="f14cb-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="f14cb-227">Поиск с получением: вторник возвращает все элементы, полученные во вторник текущей недели.</span><span class="sxs-lookup"><span data-stu-id="f14cb-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="f14cb-228">Типы значений даты также поддерживают набор ключевых слов для поиска относительно текущего времени.</span><span class="sxs-lookup"><span data-stu-id="f14cb-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="f14cb-229">Поддерживаются следующие ключевые слова:</span><span class="sxs-lookup"><span data-stu-id="f14cb-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="f14cb-230">today</span><span class="sxs-lookup"><span data-stu-id="f14cb-230">today</span></span>  
- <span data-ttu-id="f14cb-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="f14cb-231">tomorrow</span></span>
- <span data-ttu-id="f14cb-232">yesterday</span><span class="sxs-lookup"><span data-stu-id="f14cb-232">yesterday</span></span>
- <span data-ttu-id="f14cb-233">this week</span><span class="sxs-lookup"><span data-stu-id="f14cb-233">this week</span></span>    
- <span data-ttu-id="f14cb-234">На прошлой неделе</span><span class="sxs-lookup"><span data-stu-id="f14cb-234">last week</span></span>    
- <span data-ttu-id="f14cb-235">следующий месяц</span><span class="sxs-lookup"><span data-stu-id="f14cb-235">next month</span></span>    
- <span data-ttu-id="f14cb-236">последний месяц</span><span class="sxs-lookup"><span data-stu-id="f14cb-236">past month</span></span>    
- <span data-ttu-id="f14cb-237">следующий год</span><span class="sxs-lookup"><span data-stu-id="f14cb-237">coming year</span></span>
    
<span data-ttu-id="f14cb-238">Типы значений даты также можно сравнивать с операторами отношений, которые больше или меньше или указаны как диапазон с оператором Range **..**. Например, получено:\>11/30/2013, отправлено\>: = вчера и получено: 12/1/2013.. сегодня все допустимые строки запросов.</span><span class="sxs-lookup"><span data-stu-id="f14cb-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="f14cb-239">Использование типа логического значения</span><span class="sxs-lookup"><span data-stu-id="f14cb-239">Using a Boolean value type</span></span>

<span data-ttu-id="f14cb-240">Логические типы значений могут быть "true" или "false".</span><span class="sxs-lookup"><span data-stu-id="f14cb-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="f14cb-241">В значениях регистр не учитывается, поэтому для свойства Read: false результаты будут такими же, как для свойства Read: FALSE.</span><span class="sxs-lookup"><span data-stu-id="f14cb-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="f14cb-242">Использование типа числового значения</span><span class="sxs-lookup"><span data-stu-id="f14cb-242">Using a number value type</span></span>

<span data-ttu-id="f14cb-243">Числовые типы значений могут выполнять поиск в виде точных совпадений, но их также можно искать с помощью операторов отношения, таких как больше или меньше.</span><span class="sxs-lookup"><span data-stu-id="f14cb-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="f14cb-244">Например, размер: 10000 будет возвращать только элементы, размер которых равен 10000 байт, но размер:\>= 10000 будет возвращать элементы, размер которых не превышает 10000 байт.</span><span class="sxs-lookup"><span data-stu-id="f14cb-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="f14cb-245">Кроме того, можно указать диапазон с помощью оператора диапазона ( **..**).</span><span class="sxs-lookup"><span data-stu-id="f14cb-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="f14cb-246">Например, размер: 7000.. 8000 будут возвращать элементы, размер которых составляет от 7000 до 8000.</span><span class="sxs-lookup"><span data-stu-id="f14cb-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="f14cb-247">Использование логических операторов</span><span class="sxs-lookup"><span data-stu-id="f14cb-247">Using logical operators</span></span>

<span data-ttu-id="f14cb-248">Строки запросов поддерживают следующие логические операторы.</span><span class="sxs-lookup"><span data-stu-id="f14cb-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="f14cb-249">**Таблица 2. Поддерживаемые логические операторы**</span><span class="sxs-lookup"><span data-stu-id="f14cb-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="f14cb-250">**Operator**</span><span class="sxs-lookup"><span data-stu-id="f14cb-250">**Operator**</span></span>|<span data-ttu-id="f14cb-251">**Примеры**</span><span class="sxs-lookup"><span data-stu-id="f14cb-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f14cb-252">И</span><span class="sxs-lookup"><span data-stu-id="f14cb-252">AND</span></span>  <br/> |<span data-ttu-id="f14cb-253">Project и from: "Ольга Даниелс"</span><span class="sxs-lookup"><span data-stu-id="f14cb-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="f14cb-254">Тема: (проект и план)</span><span class="sxs-lookup"><span data-stu-id="f14cb-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="f14cb-255">OR</span><span class="sxs-lookup"><span data-stu-id="f14cb-255">OR</span></span>  <br/> |<span data-ttu-id="f14cb-256">Тема: собрание или из: "надеюсь, брутто"</span><span class="sxs-lookup"><span data-stu-id="f14cb-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="f14cb-257">от:("Ольга Даниелс" или "надеюсь, брутто")</span><span class="sxs-lookup"><span data-stu-id="f14cb-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="f14cb-258">NOT</span><span class="sxs-lookup"><span data-stu-id="f14cb-258">NOT</span></span>  <br/> |<span data-ttu-id="f14cb-259">НЕ из: "ронние Стургис"</span><span class="sxs-lookup"><span data-stu-id="f14cb-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="f14cb-260">получено: не сегодня</span><span class="sxs-lookup"><span data-stu-id="f14cb-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="f14cb-261">Обратите внимание, что с помощью этих операторов можно присоединяться к нескольким критериям или присоединяться к нескольким значениям в одной и той же комбинации ключевых слов и значений.</span><span class="sxs-lookup"><span data-stu-id="f14cb-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="f14cb-262">Однако при соединении нескольких значений в одной пары ключевое слово/значение следует использовать круглые скобки для заключения нескольких значений.</span><span class="sxs-lookup"><span data-stu-id="f14cb-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="f14cb-263">Сведения о том, почему следует искать с помощью: "Ольга Даниелс" или "надеюсь, брутто".</span><span class="sxs-lookup"><span data-stu-id="f14cb-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="f14cb-264">Этот поиск фактически интерпретируется как следующие условия:</span><span class="sxs-lookup"><span data-stu-id="f14cb-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="f14cb-265">Элемент из Ольга Даниелс или</span><span class="sxs-lookup"><span data-stu-id="f14cb-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="f14cb-266">Элемент имеет фразу "надеюсь брутто" в любом из его индексированных свойств.</span><span class="sxs-lookup"><span data-stu-id="f14cb-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="f14cb-267">В отличие от:("Ольга Даниелс" или "надеюсь брутто"), интерпретируется как:</span><span class="sxs-lookup"><span data-stu-id="f14cb-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="f14cb-268">Элемент из Ольга Даниелс или</span><span class="sxs-lookup"><span data-stu-id="f14cb-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="f14cb-269">Элемент от "самый общий"</span><span class="sxs-lookup"><span data-stu-id="f14cb-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="f14cb-270">Оператор по умолчанию, если задано несколько критериев, но логический оператор не включен, и.</span><span class="sxs-lookup"><span data-stu-id="f14cb-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="f14cb-271">Например, есть вложение: true Subject: Project эквивалентно: вложение: true AND Subject: Project.</span><span class="sxs-lookup"><span data-stu-id="f14cb-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="f14cb-272">Пример: Поиск элементов с помощью строки запроса и управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="f14cb-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="f14cb-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="f14cb-273"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="f14cb-274">В этом примере определен метод под названием **сеарчвискуеристринг** .</span><span class="sxs-lookup"><span data-stu-id="f14cb-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="f14cb-275">Он принимает объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [веллкновнфолдернаме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект **String** , который представляет строку запроса в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="f14cb-275">It takes an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="f14cb-276">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f14cb-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

<span data-ttu-id="f14cb-277">Этот метод можно использовать для поиска всех элементов с фразой "план проекта" в теме, как показано в этом примере.</span><span class="sxs-lookup"><span data-stu-id="f14cb-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="f14cb-278">Пример: Поиск элементов с помощью строки запроса и EWS</span><span class="sxs-lookup"><span data-stu-id="f14cb-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="f14cb-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="f14cb-279"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="f14cb-280">В этом примере запрос на SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) находит все элементы в папке "Входящие", используя фразу "план проекта" в теме.</span><span class="sxs-lookup"><span data-stu-id="f14cb-280">In this example, a SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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

<span data-ttu-id="f14cb-281">В следующем примере показан ответ от сервера с результатами поиска.</span><span class="sxs-lookup"><span data-stu-id="f14cb-281">The following example shows the response from the server with the search results.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="f14cb-282">См. также</span><span class="sxs-lookup"><span data-stu-id="f14cb-282">See also</span></span>

- [<span data-ttu-id="f14cb-283">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="f14cb-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="f14cb-284">Использование фильтров поиска с EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f14cb-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="f14cb-285">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="f14cb-285">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="f14cb-286">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="f14cb-286">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

