---
title: Строка запроса (Куеристрингтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: Элемент QueryString содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459190"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="ce6ea-103">Строка запроса (Куеристрингтипе)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="ce6ea-104">Элемент **QueryString** содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).</span><span class="sxs-lookup"><span data-stu-id="ce6ea-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="ce6ea-105">**куеристрингтипе**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce6ea-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ce6ea-106">Attributes and elements</span></span>

<span data-ttu-id="ce6ea-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce6ea-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ce6ea-108">Attributes</span></span>

|<span data-ttu-id="ce6ea-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-109">**Attribute**</span></span>|<span data-ttu-id="ce6ea-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce6ea-111">ресеткаче</span><span class="sxs-lookup"><span data-stu-id="ce6ea-111">ResetCache</span></span>  <br/> |<span data-ttu-id="ce6ea-112">Указывает, что необходимо сбросить кэш.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-113">ретурнделетедитемс</span><span class="sxs-lookup"><span data-stu-id="ce6ea-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="ce6ea-114">Указывает, что необходимо возвратить удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-115">ретурнхигхлигхттермс</span><span class="sxs-lookup"><span data-stu-id="ce6ea-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="ce6ea-116">Указывает, что выделенные термины должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ce6ea-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ce6ea-117">Child elements</span></span>

<span data-ttu-id="ce6ea-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce6ea-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ce6ea-119">Parent elements</span></span>

|<span data-ttu-id="ce6ea-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-120">**Element**</span></span>|<span data-ttu-id="ce6ea-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce6ea-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="ce6ea-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ce6ea-123">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="ce6ea-124">Ниже приведено выражение XPath для этого элемента:/Финдитем.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce6ea-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ce6ea-125">Text value</span></span>

<span data-ttu-id="ce6ea-126">Текстовое значение элемента **QueryString** представляет запрос к почтовому ящику, который выполняется с помощью подмножества [расширенного синтаксиса запросов (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce6ea-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="ce6ea-127">В разделе "Примечания" представлены сведения о поддерживаемых параметрах синтаксиса для строк запросов.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce6ea-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="ce6ea-128">Remarks</span></span>

<span data-ttu-id="ce6ea-129">В Exchange Server 2010 этот элемент относится к типу string схемы XML.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="ce6ea-130">В версиях Exchange, начиная с Exchange Server 2013, включая Exchange Online, типом для этого элемента является **куеристрингтипе**.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="ce6ea-131">Это изменение не нарушает существующие клиенты, так как добавляет три новых дополнительных атрибута.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="ce6ea-132">Элемент **QueryString** исключает использование ограничений EWS.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="ce6ea-133">AQS в EWS поддерживает три типа ограничений: ограничение этапа Word, ограничение диапазона дат и ограничение типов сообщений.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="ce6ea-134">В следующих таблицах перечислены поддерживаемые свойства поиска для каждого типа ограничения.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="ce6ea-135">**Ограничение для этапов Word**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-135">**Word phase restriction**</span></span>

|<span data-ttu-id="ce6ea-136">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-136">**Property**</span></span>|<span data-ttu-id="ce6ea-137">**Пример**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-137">**Example**</span></span>|<span data-ttu-id="ce6ea-138">**Function**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce6ea-139">from</span><span class="sxs-lookup"><span data-stu-id="ce6ea-139">from</span></span>  <br/> |<span data-ttu-id="ce6ea-140">От: Деан</span><span class="sxs-lookup"><span data-stu-id="ce6ea-140">From:Dean</span></span>  <br/> <span data-ttu-id="ce6ea-141">From: "Деан Халстеад"</span><span class="sxs-lookup"><span data-stu-id="ce6ea-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="ce6ea-142">Поиск элементов, отправленных из Деан.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="ce6ea-143">Элементы поиска, отправленные из Деан Халстеад.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="ce6ea-144">Отправитель должен быть в точности "Деан Халстеад".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="ce6ea-145">на</span><span class="sxs-lookup"><span data-stu-id="ce6ea-145">to</span></span>  <br/> |<span data-ttu-id="ce6ea-146">Кому: Деан</span><span class="sxs-lookup"><span data-stu-id="ce6ea-146">To:Dean</span></span>  <br/> |<span data-ttu-id="ce6ea-147">Поиск элементов, отправленных в Деан.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-148">копия;</span><span class="sxs-lookup"><span data-stu-id="ce6ea-148">cc</span></span>  <br/> |<span data-ttu-id="ce6ea-149">CC: Деан</span><span class="sxs-lookup"><span data-stu-id="ce6ea-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="ce6ea-150">Поиск элементов с Деан в строке "копия".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-151">СК.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-151">bcc</span></span>  <br/> |<span data-ttu-id="ce6ea-152">СК: Деан</span><span class="sxs-lookup"><span data-stu-id="ce6ea-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="ce6ea-153">Поиск элементов с Деан в строке "Скрытая копия".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-154">Participants</span><span class="sxs-lookup"><span data-stu-id="ce6ea-154">Participants</span></span>  <br/> |<span data-ttu-id="ce6ea-155">Участники: Деан</span><span class="sxs-lookup"><span data-stu-id="ce6ea-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="ce6ea-156">Поиск элементов с Деан в полях "Кому", "копия" или "Скрытая копия".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-157">Subject</span><span class="sxs-lookup"><span data-stu-id="ce6ea-157">Subject</span></span>  <br/> |<span data-ttu-id="ce6ea-158">Тема: Product</span><span class="sxs-lookup"><span data-stu-id="ce6ea-158">Subject:product</span></span>  <br/> <span data-ttu-id="ce6ea-159">Тема: (разработка продукта)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="ce6ea-160">Тема: "Разработка продуктов"</span><span class="sxs-lookup"><span data-stu-id="ce6ea-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="ce6ea-161">Поиск элементов с товаром в теме.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="ce6ea-162">Поиск элементов с продуктом и разработкой в теме.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-163">Основной текст</span><span class="sxs-lookup"><span data-stu-id="ce6ea-163">Body</span></span>  <br/> <span data-ttu-id="ce6ea-164">Контент</span><span class="sxs-lookup"><span data-stu-id="ce6ea-164">Content</span></span>  <br/> |<span data-ttu-id="ce6ea-165">Основной текст: ход выполнения</span><span class="sxs-lookup"><span data-stu-id="ce6ea-165">Body:progress</span></span>  <br/> <span data-ttu-id="ce6ea-166">Контент: ход выполнения</span><span class="sxs-lookup"><span data-stu-id="ce6ea-166">Content:progress</span></span>  <br/> |<span data-ttu-id="ce6ea-167">Поиск элементов с ходом выполнения в теле.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-168">Вложение</span><span class="sxs-lookup"><span data-stu-id="ce6ea-168">Attachment</span></span>  <br/> |<span data-ttu-id="ce6ea-169">Вложение: отчет</span><span class="sxs-lookup"><span data-stu-id="ce6ea-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="ce6ea-170">Поиск элементов с отчетом в имени файла вложения или в его тексте.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-171">(свойство не задано)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="ce6ea-172">Разработка продукта</span><span class="sxs-lookup"><span data-stu-id="ce6ea-172">Product Development</span></span>  <br/> |<span data-ttu-id="ce6ea-173">Поиск элементов, которые содержат как продукты, так и разработку во всех свойствах этапа слов.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="ce6ea-174">Сравнение ограничений для этапа Word всегда не учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="ce6ea-175">Ограничение на этап Word поддерживает два типа совпадений: совпадение префиксов или точное совпадение.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="ce6ea-176">Префикс "ПОИСКПОЗ" является поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="ce6ea-177">Если требуется точное совпадение, используйте двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="ce6ea-178">Например, Subject: "продукт" соответствует "продукту", но не "производству" в теме.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="ce6ea-179">Несколько слов в двойных кавычках ограничивают оба этапа и порядок слов.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="ce6ea-180">Например, "Win Product" соответствует только "Win Product", а не "Win95 Product" или "Product of Win".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="ce6ea-181">Можно использовать звездочку ( \* ), чтобы определить префикс с ограничением порядка.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="ce6ea-182">Например, "Win Product" \* соответствует "Win95 Product", "Windows Production Line", но не "Windows New Product" или "Product of Win".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="ce6ea-183">Можно выполнять поиск по всем сообщениям, отправляемым с домена или в домен.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="ce6ea-184">Например, from: "@hotmail. com" возвращает все сообщения, отправленные из hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="ce6ea-185">В следующей таблице описываются ограничения диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="ce6ea-186">**Ограничение диапазона дат**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-186">**Date range restriction**</span></span>

|<span data-ttu-id="ce6ea-187">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-187">**Property**</span></span>|<span data-ttu-id="ce6ea-188">**Пример**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-188">**Example**</span></span>|<span data-ttu-id="ce6ea-189">**Function**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce6ea-190">Sent</span><span class="sxs-lookup"><span data-stu-id="ce6ea-190">Sent</span></span>  <br/> |<span data-ttu-id="ce6ea-191">Отправлено: на прошлой неделе</span><span class="sxs-lookup"><span data-stu-id="ce6ea-191">Sent:last week</span></span>  <br/> <span data-ttu-id="ce6ea-192">Отправлено: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="ce6ea-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="ce6ea-193">Отправлено: 01/01/2001.. 01/15/2001</span><span class="sxs-lookup"><span data-stu-id="ce6ea-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="ce6ea-194">Поиск элементов, отправленных за последнюю неделю.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="ce6ea-195">Поиск элементов, отправленных на 1 января 2001.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="ce6ea-196">Поиск элементов, отправленных между 1 января по 2001 и 15 января 2001.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-197">ПОЛУЧЕНО</span><span class="sxs-lookup"><span data-stu-id="ce6ea-197">Received</span></span>  <br/> |<span data-ttu-id="ce6ea-198">Получено: сегодня</span><span class="sxs-lookup"><span data-stu-id="ce6ea-198">Received:today</span></span>  <br/> <span data-ttu-id="ce6ea-199">Получено: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="ce6ea-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="ce6ea-200">Элементы поиска, полученные сегодня.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-200">Search items received today.</span></span>  <br/> <span data-ttu-id="ce6ea-201">Элементы поиска, полученные 1 января 2001 г.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="ce6ea-202">Две точки (..) — это оператор диапазона.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="ce6ea-203">Его можно использовать для определения диапазона с начальной и конечной датами.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="ce6ea-204">Чтобы указать дату, можно использовать относительные даты.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="ce6ea-205">Поддерживаются следующие относительные даты:</span><span class="sxs-lookup"><span data-stu-id="ce6ea-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="ce6ea-206">Относительные даты: сегодня, завтра, вчера</span><span class="sxs-lookup"><span data-stu-id="ce6ea-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="ce6ea-207">Относительные даты для нескольких слов: Эта неделя, следующий месяц, последняя неделя, последний месяц или следующий год</span><span class="sxs-lookup"><span data-stu-id="ce6ea-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="ce6ea-208">Дни: воскресенье, понедельник, вторник, среда, четверг, пятница, Суббота</span><span class="sxs-lookup"><span data-stu-id="ce6ea-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="ce6ea-209">Январь, Февраль, Март, Апрель, Май, Июнь, Июль, Август, Сентябрь, Октябрь, Ноябрь, Декабрь</span><span class="sxs-lookup"><span data-stu-id="ce6ea-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="ce6ea-210">В следующей таблице описываются ограничения на типы сообщений.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="ce6ea-211">**Ограничение на тип сообщения**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-211">**Message type restriction**</span></span>

|<span data-ttu-id="ce6ea-212">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-212">**Property**</span></span>|<span data-ttu-id="ce6ea-213">**Пример**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-213">**Example**</span></span>|<span data-ttu-id="ce6ea-214">**Function**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce6ea-215">Kind</span><span class="sxs-lookup"><span data-stu-id="ce6ea-215">Kind</span></span>  <br/> |<span data-ttu-id="ce6ea-216">Вид: задачи</span><span class="sxs-lookup"><span data-stu-id="ce6ea-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="ce6ea-217">Поиск во всех элементах задач.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="ce6ea-218">AQS в EWS использует свойство **Kind** , чтобы указать тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="ce6ea-219">Свойство Kind можно использовать со следующими типами элементов:</span><span class="sxs-lookup"><span data-stu-id="ce6ea-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="ce6ea-220">email</span><span class="sxs-lookup"><span data-stu-id="ce6ea-220">email</span></span>
    
- <span data-ttu-id="ce6ea-221">meetings</span><span class="sxs-lookup"><span data-stu-id="ce6ea-221">meetings</span></span>
    
- <span data-ttu-id="ce6ea-222">tasks</span><span class="sxs-lookup"><span data-stu-id="ce6ea-222">tasks</span></span>
    
- <span data-ttu-id="ce6ea-223">notes</span><span class="sxs-lookup"><span data-stu-id="ce6ea-223">notes</span></span>
    
- <span data-ttu-id="ce6ea-224">docs</span><span class="sxs-lookup"><span data-stu-id="ce6ea-224">docs</span></span>
    
- <span data-ttu-id="ce6ea-225">journals</span><span class="sxs-lookup"><span data-stu-id="ce6ea-225">journals</span></span>
    
- <span data-ttu-id="ce6ea-226">contacts</span><span class="sxs-lookup"><span data-stu-id="ce6ea-226">contacts</span></span>
    
- <span data-ttu-id="ce6ea-227">im</span><span class="sxs-lookup"><span data-stu-id="ce6ea-227">im</span></span>
    
<span data-ttu-id="ce6ea-228">В следующей таблице описываются логические соединители группировки.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="ce6ea-229">**Группировка логических соединителей**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="ce6ea-230">**Connector**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-230">**Connector**</span></span>|<span data-ttu-id="ce6ea-231">**Пример**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-231">**Example**</span></span>|<span data-ttu-id="ce6ea-232">**Function**</span><span class="sxs-lookup"><span data-stu-id="ce6ea-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce6ea-233">И</span><span class="sxs-lookup"><span data-stu-id="ce6ea-233">AND</span></span>  <br/> |<span data-ttu-id="ce6ea-234">Тема: продукт и Тема: Разработка</span><span class="sxs-lookup"><span data-stu-id="ce6ea-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="ce6ea-235">Тема: (продукт и разработка)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="ce6ea-236">Тема: (разработка продукта)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="ce6ea-237">Поиск элементов в теме с помощью продукта и разработки.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-238">OR</span><span class="sxs-lookup"><span data-stu-id="ce6ea-238">OR</span></span>  <br/> |<span data-ttu-id="ce6ea-239">Текст: проект или текст: предложение</span><span class="sxs-lookup"><span data-stu-id="ce6ea-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="ce6ea-240">Основной текст: (проект или предложение)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="ce6ea-241">Поиск элементов с помощью продукта или разработки в теле.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="ce6ea-242">NOT</span><span class="sxs-lookup"><span data-stu-id="ce6ea-242">NOT</span></span>  <br/> |<span data-ttu-id="ce6ea-243">НЕТ текста: предложение</span><span class="sxs-lookup"><span data-stu-id="ce6ea-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="ce6ea-244">Основной текст: (нет предложения)</span><span class="sxs-lookup"><span data-stu-id="ce6ea-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="ce6ea-245">Поиск в сообщениях без предложения в теле.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="ce6ea-246">И всегда является соединителем по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-246">AND is always the default connector.</span></span> <span data-ttu-id="ce6ea-247">Например, Subject: Subject: Project и Body: предложение равно "subject": "Body": предложение.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="ce6ea-248">Логические соединители чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="ce6ea-249">Например, body: (проект или предложение) выполняет поиск в сообщениях с помощью "проект", "или" и "предложение" в тексте, а не "проект" или "предложение".</span><span class="sxs-lookup"><span data-stu-id="ce6ea-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="ce6ea-250">Символ "плюс" (+) эквивалентен и.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="ce6ea-251">Символ дефиса (-) эквивалентен параметру NOT.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="ce6ea-252">Например, body: (проект-предложение) выполняет поиск в сообщениях с "Project", но без предложения "предложение" в теле.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="ce6ea-253">Строка запроса также может содержать неиндексированные свойства для поиска.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="ce6ea-254">Если строка запроса содержит неиндексированные свойства, поиск может выполнить поиск Exchange по индексированным свойствам и поиск хранилища для неиндексированных свойств.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="ce6ea-255">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="ce6ea-256">Пример</span><span class="sxs-lookup"><span data-stu-id="ce6ea-256">Example</span></span>

<span data-ttu-id="ce6ea-257">В приведенном ниже примере показан запрос на поиск сообщений в папке "Входящие" с автообнаружением в теме.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="ce6ea-258">В следующем примере показан успешный ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="ce6ea-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="ce6ea-259">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ce6ea-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce6ea-260">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ce6ea-260">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce6ea-261">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ce6ea-261">Schema name</span></span>  <br/> |<span data-ttu-id="ce6ea-262">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ce6ea-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ce6ea-263">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ce6ea-263">Validation file</span></span>  <br/> |<span data-ttu-id="ce6ea-264">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ce6ea-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce6ea-265">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ce6ea-265">Can be empty</span></span>  <br/> |<span data-ttu-id="ce6ea-266">False</span><span class="sxs-lookup"><span data-stu-id="ce6ea-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce6ea-267">См. также</span><span class="sxs-lookup"><span data-stu-id="ce6ea-267">See also</span></span>



[<span data-ttu-id="ce6ea-268">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="ce6ea-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="ce6ea-269">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="ce6ea-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="ce6ea-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce6ea-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

