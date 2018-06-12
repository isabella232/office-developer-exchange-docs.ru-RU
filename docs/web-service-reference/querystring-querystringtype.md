---
title: Строка запроса (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: Элемент строки запроса содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834943"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="16976-103">Строка запроса (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="16976-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="16976-104">Элемент **строки запроса** содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).</span><span class="sxs-lookup"><span data-stu-id="16976-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="16976-105">**QueryStringType**</span><span class="sxs-lookup"><span data-stu-id="16976-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16976-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16976-106">Attributes and elements</span></span>

<span data-ttu-id="16976-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="16976-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16976-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16976-108">Attributes</span></span>

|<span data-ttu-id="16976-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="16976-109">**Attribute**</span></span>|<span data-ttu-id="16976-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16976-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16976-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="16976-111">ResetCache</span></span>  <br/> |<span data-ttu-id="16976-112">Указывает, что необходимо очистить кэш.</span><span class="sxs-lookup"><span data-stu-id="16976-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="16976-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="16976-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="16976-114">Указывает, что должны быть возвращены "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="16976-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="16976-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="16976-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="16976-116">Указывает, что выделенный терминов должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="16976-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="16976-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16976-117">Child elements</span></span>

<span data-ttu-id="16976-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="16976-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16976-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16976-119">Parent elements</span></span>

|<span data-ttu-id="16976-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16976-120">**Element**</span></span>|<span data-ttu-id="16976-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16976-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16976-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="16976-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="16976-123">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="16976-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="16976-124">Ниже приведен выражение XPath для этого элемента: /FindItem.</span><span class="sxs-lookup"><span data-stu-id="16976-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16976-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="16976-125">Text value</span></span>

<span data-ttu-id="16976-126">Текстовое значение **строки запроса** элемент представляет почтового ящика запросы, выполненные с помощью подмножество [Расширенного синтаксиса запроса (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="16976-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="16976-127">Сведения о поддерживаемых синтаксис параметров строки запроса см.</span><span class="sxs-lookup"><span data-stu-id="16976-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16976-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="16976-128">Remarks</span></span>

<span data-ttu-id="16976-129">В Exchange Server 2010 этот элемент относится к типу string схемы XML.</span><span class="sxs-lookup"><span data-stu-id="16976-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="16976-130">В версиях Exchange, начиная с Exchange Server 2013 включая Exchange Online тип для этого элемента — **QueryStringType**.</span><span class="sxs-lookup"><span data-stu-id="16976-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="16976-131">Это изменение не нарушает все существующие клиенты, так как трех новых необязательные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="16976-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="16976-132">Элемент **строки запроса** исключает использование ограничения веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="16976-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="16976-133">AQS в веб-служб Exchange поддерживает три типа ограничений: этап ограничения, ограничение диапазон даты и ограничения типа сообщения word.</span><span class="sxs-lookup"><span data-stu-id="16976-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="16976-134">В следующей таблице перечислены поддерживаемые поиска свойств для каждого типа ограничений.</span><span class="sxs-lookup"><span data-stu-id="16976-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="16976-135">**Ограничение этап Word**</span><span class="sxs-lookup"><span data-stu-id="16976-135">**Word phase restriction**</span></span>

|<span data-ttu-id="16976-136">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="16976-136">**Property**</span></span>|<span data-ttu-id="16976-137">**Пример**</span><span class="sxs-lookup"><span data-stu-id="16976-137">**Example**</span></span>|<span data-ttu-id="16976-138">**�������**</span><span class="sxs-lookup"><span data-stu-id="16976-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="16976-139">from</span><span class="sxs-lookup"><span data-stu-id="16976-139">from</span></span>  <br/> |<span data-ttu-id="16976-140">От: Дин</span><span class="sxs-lookup"><span data-stu-id="16976-140">From:Dean</span></span>  <br/> <span data-ttu-id="16976-141">От: «Дин Halstead»</span><span class="sxs-lookup"><span data-stu-id="16976-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="16976-142">Поиск элементов, отправляемых с Дин.</span><span class="sxs-lookup"><span data-stu-id="16976-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="16976-143">Поиск элементов, отправляемых с Halstead Дин.</span><span class="sxs-lookup"><span data-stu-id="16976-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="16976-144">Отправитель должен быть точно «Дин Halstead».</span><span class="sxs-lookup"><span data-stu-id="16976-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="16976-145">to</span><span class="sxs-lookup"><span data-stu-id="16976-145">to</span></span>  <br/> |<span data-ttu-id="16976-146">Чтобы: Дин</span><span class="sxs-lookup"><span data-stu-id="16976-146">To:Dean</span></span>  <br/> |<span data-ttu-id="16976-147">Поиск элементов, отправленных Дин.</span><span class="sxs-lookup"><span data-stu-id="16976-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="16976-148">cc</span><span class="sxs-lookup"><span data-stu-id="16976-148">cc</span></span>  <br/> |<span data-ttu-id="16976-149">Cc:Dean</span><span class="sxs-lookup"><span data-stu-id="16976-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="16976-150">Поиск элементов с Дин в строке копия.</span><span class="sxs-lookup"><span data-stu-id="16976-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="16976-151">bcc</span><span class="sxs-lookup"><span data-stu-id="16976-151">bcc</span></span>  <br/> |<span data-ttu-id="16976-152">BCC:Dean</span><span class="sxs-lookup"><span data-stu-id="16976-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="16976-153">Поиск элементов с Дин строки Скрытая копия.</span><span class="sxs-lookup"><span data-stu-id="16976-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="16976-154">Участники</span><span class="sxs-lookup"><span data-stu-id="16976-154">Participants</span></span>  <br/> |<span data-ttu-id="16976-155">Участники: Дин</span><span class="sxs-lookup"><span data-stu-id="16976-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="16976-156">Поиск элементов с Дин Кому, копия или Скрытая копия поля.</span><span class="sxs-lookup"><span data-stu-id="16976-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="16976-157">Subject</span><span class="sxs-lookup"><span data-stu-id="16976-157">Subject</span></span>  <br/> |<span data-ttu-id="16976-158">Тема: продукта</span><span class="sxs-lookup"><span data-stu-id="16976-158">Subject:product</span></span>  <br/> <span data-ttu-id="16976-159">Тема:(product development)</span><span class="sxs-lookup"><span data-stu-id="16976-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="16976-160">Тема: «разработка продукта»</span><span class="sxs-lookup"><span data-stu-id="16976-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="16976-161">Поиск элементов с продукта в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="16976-162">Поиск элементов с помощью продуктов и разработки в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="16976-163">Body</span><span class="sxs-lookup"><span data-stu-id="16976-163">Body</span></span>  <br/> <span data-ttu-id="16976-164">Контент</span><span class="sxs-lookup"><span data-stu-id="16976-164">Content</span></span>  <br/> |<span data-ttu-id="16976-165">BODY: хода выполнения</span><span class="sxs-lookup"><span data-stu-id="16976-165">Body:progress</span></span>  <br/> <span data-ttu-id="16976-166">Содержимое: хода выполнения</span><span class="sxs-lookup"><span data-stu-id="16976-166">Content:progress</span></span>  <br/> |<span data-ttu-id="16976-167">Поиск элементов с о ходе выполнения в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="16976-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="16976-168">Attachment</span><span class="sxs-lookup"><span data-stu-id="16976-168">Attachment</span></span>  <br/> |<span data-ttu-id="16976-169">Вложения: отчет</span><span class="sxs-lookup"><span data-stu-id="16976-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="16976-170">Поиск элементов с отчета в теле имя или файл файл вложения.</span><span class="sxs-lookup"><span data-stu-id="16976-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="16976-171">(свойство не указан)</span><span class="sxs-lookup"><span data-stu-id="16976-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="16976-172">Разработка продукта</span><span class="sxs-lookup"><span data-stu-id="16976-172">Product Development</span></span>  <br/> |<span data-ttu-id="16976-173">Поиск элементов, которые содержат продукта и разработки решений в все свойства этап word.</span><span class="sxs-lookup"><span data-stu-id="16976-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="16976-174">Этап ограничение соответствие всегда без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="16976-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="16976-175">Ограничение этап Word поддерживает два типа соответствия: префикс или точное соответствие.</span><span class="sxs-lookup"><span data-stu-id="16976-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="16976-176">Соответствие префикса — это поведение по умолчанию совпадение.</span><span class="sxs-lookup"><span data-stu-id="16976-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="16976-177">Если вы хотите точное совпадение, используйте двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="16976-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="16976-178">Например, тема: «продукт» соответствует «продукт», но не «производственной» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="16976-179">Несколько слов в двойные кавычки ограничить этапов word и их порядок.</span><span class="sxs-lookup"><span data-stu-id="16976-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="16976-180">Для примера «win продукта» соответствует только «win продукт», не «win95 продукт» или «продукт win».</span><span class="sxs-lookup"><span data-stu-id="16976-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="16976-181">Можно использовать символ звездочки (\*) для определения соответствие префикса с порядком ограниченного доступа.</span><span class="sxs-lookup"><span data-stu-id="16976-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="16976-182">Например, «win продукта»\* соответствует «win95 продукт», «строка рабочей windows», но не «новый продукт windows» или «продукт win».</span><span class="sxs-lookup"><span data-stu-id="16976-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="16976-183">Можно выполнить поиск всех сообщений, отправляемых из или в домен.</span><span class="sxs-lookup"><span data-stu-id="16976-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="16976-184">Например, from:"@hotmail.com» возвращает все сообщения, отправляемые hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="16976-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="16976-185">В следующей таблице описаны ограничения диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="16976-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="16976-186">**Ограничение диапазона дат**</span><span class="sxs-lookup"><span data-stu-id="16976-186">**Date range restriction**</span></span>

|<span data-ttu-id="16976-187">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="16976-187">**Property**</span></span>|<span data-ttu-id="16976-188">**Пример**</span><span class="sxs-lookup"><span data-stu-id="16976-188">**Example**</span></span>|<span data-ttu-id="16976-189">**�������**</span><span class="sxs-lookup"><span data-stu-id="16976-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="16976-190">Sent</span><span class="sxs-lookup"><span data-stu-id="16976-190">Sent</span></span>  <br/> |<span data-ttu-id="16976-191">Отправлено: прошлую неделю</span><span class="sxs-lookup"><span data-stu-id="16976-191">Sent:last week</span></span>  <br/> <span data-ttu-id="16976-192">Отправлено: 01/01/2001 г.</span><span class="sxs-lookup"><span data-stu-id="16976-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="16976-193">Sent:01/01/2001..01/15/2001</span><span class="sxs-lookup"><span data-stu-id="16976-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="16976-194">Поиск элементов, отправленных прошлую неделю.</span><span class="sxs-lookup"><span data-stu-id="16976-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="16976-195">Поиск элементов, переданного по 1-го января 2001 года.</span><span class="sxs-lookup"><span data-stu-id="16976-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="16976-196">Поиск элементов, передаваемых между 1 января 2001 года и 15 января 2001 года.</span><span class="sxs-lookup"><span data-stu-id="16976-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="16976-197">Получено</span><span class="sxs-lookup"><span data-stu-id="16976-197">Received</span></span>  <br/> |<span data-ttu-id="16976-198">Получено: сегодня</span><span class="sxs-lookup"><span data-stu-id="16976-198">Received:today</span></span>  <br/> <span data-ttu-id="16976-199">Получено: 01/01/2001 г.</span><span class="sxs-lookup"><span data-stu-id="16976-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="16976-200">Поиск элементов, полученных сегодня.</span><span class="sxs-lookup"><span data-stu-id="16976-200">Search items received today.</span></span>  <br/> <span data-ttu-id="16976-201">Поиск элементов, полученного по 1-го января 2001 года.</span><span class="sxs-lookup"><span data-stu-id="16976-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="16976-202">Две точки (.) — это оператор диапазона.</span><span class="sxs-lookup"><span data-stu-id="16976-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="16976-203">Используется для определения диапазона с начала и Дата окончания.</span><span class="sxs-lookup"><span data-stu-id="16976-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="16976-204">Чтобы указать дату, можно использовать относительные даты.</span><span class="sxs-lookup"><span data-stu-id="16976-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="16976-205">Поддерживаются следующие относительные даты:</span><span class="sxs-lookup"><span data-stu-id="16976-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="16976-206">Относительные даты: сегодня, завтра, за вчерашний день</span><span class="sxs-lookup"><span data-stu-id="16976-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="16976-207">Multiword относительные даты: этой неделе следующего месяца, последнюю неделю за месяц или следующий год</span><span class="sxs-lookup"><span data-stu-id="16976-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="16976-208">Дней: Воскресенье, понедельник, Вторник, среда, четверг, пятница, суббота</span><span class="sxs-lookup"><span data-stu-id="16976-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="16976-209">Январь, февраль, март, апрель, возможно, июня, июля, августа, сентябрь, октябрь, ноябрь, декабрь</span><span class="sxs-lookup"><span data-stu-id="16976-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="16976-210">В следующей таблице описаны ограничения типов сообщений.</span><span class="sxs-lookup"><span data-stu-id="16976-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="16976-211">**Ограничение типа сообщения**</span><span class="sxs-lookup"><span data-stu-id="16976-211">**Message type restriction**</span></span>

|<span data-ttu-id="16976-212">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="16976-212">**Property**</span></span>|<span data-ttu-id="16976-213">**Пример**</span><span class="sxs-lookup"><span data-stu-id="16976-213">**Example**</span></span>|<span data-ttu-id="16976-214">**�������**</span><span class="sxs-lookup"><span data-stu-id="16976-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="16976-215">Тип</span><span class="sxs-lookup"><span data-stu-id="16976-215">Kind</span></span>  <br/> |<span data-ttu-id="16976-216">Тип: задачи</span><span class="sxs-lookup"><span data-stu-id="16976-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="16976-217">Поиск во всех элементах задач.</span><span class="sxs-lookup"><span data-stu-id="16976-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="16976-218">AQS в веб-свойство **типа** используется для указания типа сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="16976-219">Тип свойства можно с помощью следующих типов элементов:</span><span class="sxs-lookup"><span data-stu-id="16976-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="16976-220">email</span><span class="sxs-lookup"><span data-stu-id="16976-220">email</span></span>
    
- <span data-ttu-id="16976-221">собрания</span><span class="sxs-lookup"><span data-stu-id="16976-221">meetings</span></span>
    
- <span data-ttu-id="16976-222">tasks</span><span class="sxs-lookup"><span data-stu-id="16976-222">tasks</span></span>
    
- <span data-ttu-id="16976-223">notes</span><span class="sxs-lookup"><span data-stu-id="16976-223">notes</span></span>
    
- <span data-ttu-id="16976-224">документы</span><span class="sxs-lookup"><span data-stu-id="16976-224">docs</span></span>
    
- <span data-ttu-id="16976-225">журналы.</span><span class="sxs-lookup"><span data-stu-id="16976-225">journals</span></span>
    
- <span data-ttu-id="16976-226">contacts</span><span class="sxs-lookup"><span data-stu-id="16976-226">contacts</span></span>
    
- <span data-ttu-id="16976-227">обмен мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="16976-227">im</span></span>
    
<span data-ttu-id="16976-228">В следующей таблице описываются группировки логической соединители.</span><span class="sxs-lookup"><span data-stu-id="16976-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="16976-229">**Соединители логической группировки**</span><span class="sxs-lookup"><span data-stu-id="16976-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="16976-230">**Соединитель**</span><span class="sxs-lookup"><span data-stu-id="16976-230">**Connector**</span></span>|<span data-ttu-id="16976-231">**Пример**</span><span class="sxs-lookup"><span data-stu-id="16976-231">**Example**</span></span>|<span data-ttu-id="16976-232">**�������**</span><span class="sxs-lookup"><span data-stu-id="16976-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="16976-233">AND</span><span class="sxs-lookup"><span data-stu-id="16976-233">AND</span></span>  <br/> |<span data-ttu-id="16976-234">Тема: продукта и Тема: Разработка</span><span class="sxs-lookup"><span data-stu-id="16976-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="16976-235">Тема:(product AND development)</span><span class="sxs-lookup"><span data-stu-id="16976-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="16976-236">Тема:(product development)</span><span class="sxs-lookup"><span data-stu-id="16976-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="16976-237">Поиск элементов с помощью продуктов и разработки в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="16976-238">OR</span><span class="sxs-lookup"><span data-stu-id="16976-238">OR</span></span>  <br/> |<span data-ttu-id="16976-239">BODY: проекта или тело: предложения</span><span class="sxs-lookup"><span data-stu-id="16976-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="16976-240">BODY:(project OR proposal)</span><span class="sxs-lookup"><span data-stu-id="16976-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="16976-241">Поиск элементов с продуктом или разработки в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="16976-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="16976-242">NOT</span><span class="sxs-lookup"><span data-stu-id="16976-242">NOT</span></span>  <br/> |<span data-ttu-id="16976-243">Body: предложения</span><span class="sxs-lookup"><span data-stu-id="16976-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="16976-244">:(NOT proposal) текста</span><span class="sxs-lookup"><span data-stu-id="16976-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="16976-245">Поиск в тексте сообщения без предложения.</span><span class="sxs-lookup"><span data-stu-id="16976-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="16976-246">Всегда и соединитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="16976-246">AND is always the default connector.</span></span> <span data-ttu-id="16976-247">Тема: проекта и тело: предложения совпадает с body: предложения Тема: проекта.</span><span class="sxs-lookup"><span data-stu-id="16976-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="16976-248">Логическая соединители чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="16976-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="16976-249">Например, body:(project Or proposal) выполняет поиск сообщений с «project», «или» и «предложения» в теле вместо «project» или «предложения».</span><span class="sxs-lookup"><span data-stu-id="16976-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="16976-250">Знак плюса (+) является эквивалентом AND.</span><span class="sxs-lookup"><span data-stu-id="16976-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="16976-251">НЕ эквивалентно символ дефиса (-).</span><span class="sxs-lookup"><span data-stu-id="16976-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="16976-252">Например, body:(project-proposal) выполняет поиск сообщений с «project», но без «предложения» в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="16976-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="16976-253">Строка запроса также может содержать неиндексируемых свойств для поиска.</span><span class="sxs-lookup"><span data-stu-id="16976-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="16976-254">Если строка запроса содержит неиндексируемых свойств, поиска может выполнить поиск Exchange на индексированные свойства и поиска хранилища на неиндексируемых свойств.</span><span class="sxs-lookup"><span data-stu-id="16976-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="16976-255">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="16976-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="16976-256">Пример</span><span class="sxs-lookup"><span data-stu-id="16976-256">Example</span></span>

<span data-ttu-id="16976-257">В следующем примере показано запрос на поиск сообщений в папке "Входящие" с помощью службы автообнаружения в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="16976-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="16976-258">В следующем примере показано успешного ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="16976-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a><span data-ttu-id="16976-259">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16976-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16976-260">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16976-260">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="16976-261">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16976-261">Schema name</span></span>  <br/> |<span data-ttu-id="16976-262">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="16976-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="16976-263">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16976-263">Validation file</span></span>  <br/> |<span data-ttu-id="16976-264">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16976-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16976-265">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16976-265">Can be empty</span></span>  <br/> |<span data-ttu-id="16976-266">False</span><span class="sxs-lookup"><span data-stu-id="16976-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16976-267">См. также</span><span class="sxs-lookup"><span data-stu-id="16976-267">See also</span></span>



[<span data-ttu-id="16976-268">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="16976-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="16976-269">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="16976-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="16976-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="16976-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

