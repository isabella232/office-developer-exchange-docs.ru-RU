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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459190"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="9d3f7-103">Строка запроса (Куеристрингтипе)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="9d3f7-104">Элемент **QueryString** содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).</span><span class="sxs-lookup"><span data-stu-id="9d3f7-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="9d3f7-105">**куеристрингтипе**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d3f7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9d3f7-106">Attributes and elements</span></span>

<span data-ttu-id="9d3f7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d3f7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9d3f7-108">Attributes</span></span>

|<span data-ttu-id="9d3f7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-109">**Attribute**</span></span>|<span data-ttu-id="9d3f7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9d3f7-111">ресеткаче</span><span class="sxs-lookup"><span data-stu-id="9d3f7-111">ResetCache</span></span>  <br/> |<span data-ttu-id="9d3f7-112">Указывает, что необходимо сбросить кэш.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-113">ретурнделетедитемс</span><span class="sxs-lookup"><span data-stu-id="9d3f7-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="9d3f7-114">Указывает, что необходимо возвратить удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-115">ретурнхигхлигхттермс</span><span class="sxs-lookup"><span data-stu-id="9d3f7-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="9d3f7-116">Указывает, что выделенные термины должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9d3f7-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9d3f7-117">Child elements</span></span>

<span data-ttu-id="9d3f7-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d3f7-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9d3f7-119">Parent elements</span></span>

|<span data-ttu-id="9d3f7-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-120">**Element**</span></span>|<span data-ttu-id="9d3f7-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d3f7-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="9d3f7-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="9d3f7-123">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="9d3f7-124">Ниже приведено выражение XPath для этого элемента:/Финдитем.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d3f7-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9d3f7-125">Text value</span></span>

<span data-ttu-id="9d3f7-126">Текстовое значение элемента **QueryString** представляет запрос к почтовому ящику, который выполняется с помощью подмножества [расширенного синтаксиса запросов (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9d3f7-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="9d3f7-127">В разделе "Примечания" представлены сведения о поддерживаемых параметрах синтаксиса для строк запросов.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d3f7-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="9d3f7-128">Remarks</span></span>

<span data-ttu-id="9d3f7-129">В Exchange Server 2010 этот элемент относится к типу string схемы XML.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="9d3f7-130">В версиях Exchange, начиная с Exchange Server 2013, включая Exchange Online, типом для этого элемента является **куеристрингтипе**.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="9d3f7-131">Это изменение не нарушает существующие клиенты, так как добавляет три новых дополнительных атрибута.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="9d3f7-132">Элемент **QueryString** исключает использование ограничений EWS.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="9d3f7-133">AQS в EWS поддерживает три типа ограничений: ограничение этапа Word, ограничение диапазона дат и ограничение типов сообщений.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="9d3f7-134">В следующих таблицах перечислены поддерживаемые свойства поиска для каждого типа ограничения.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="9d3f7-135">**Ограничение для этапов Word**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-135">**Word phase restriction**</span></span>

|<span data-ttu-id="9d3f7-136">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-136">**Property**</span></span>|<span data-ttu-id="9d3f7-137">**Пример**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-137">**Example**</span></span>|<span data-ttu-id="9d3f7-138">**Function**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9d3f7-139">from</span><span class="sxs-lookup"><span data-stu-id="9d3f7-139">from</span></span>  <br/> |<span data-ttu-id="9d3f7-140">От: Деан</span><span class="sxs-lookup"><span data-stu-id="9d3f7-140">From:Dean</span></span>  <br/> <span data-ttu-id="9d3f7-141">From: "Деан Халстеад"</span><span class="sxs-lookup"><span data-stu-id="9d3f7-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="9d3f7-142">Поиск элементов, отправленных из Деан.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="9d3f7-143">Элементы поиска, отправленные из Деан Халстеад.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="9d3f7-144">Отправитель должен быть в точности "Деан Халстеад".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="9d3f7-145">на</span><span class="sxs-lookup"><span data-stu-id="9d3f7-145">to</span></span>  <br/> |<span data-ttu-id="9d3f7-146">Кому: Деан</span><span class="sxs-lookup"><span data-stu-id="9d3f7-146">To:Dean</span></span>  <br/> |<span data-ttu-id="9d3f7-147">Поиск элементов, отправленных в Деан.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-148">копия;</span><span class="sxs-lookup"><span data-stu-id="9d3f7-148">cc</span></span>  <br/> |<span data-ttu-id="9d3f7-149">CC: Деан</span><span class="sxs-lookup"><span data-stu-id="9d3f7-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="9d3f7-150">Поиск элементов с Деан в строке "копия".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-151">СК.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-151">bcc</span></span>  <br/> |<span data-ttu-id="9d3f7-152">СК: Деан</span><span class="sxs-lookup"><span data-stu-id="9d3f7-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="9d3f7-153">Поиск элементов с Деан в строке "Скрытая копия".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-154">Participants</span><span class="sxs-lookup"><span data-stu-id="9d3f7-154">Participants</span></span>  <br/> |<span data-ttu-id="9d3f7-155">Участники: Деан</span><span class="sxs-lookup"><span data-stu-id="9d3f7-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="9d3f7-156">Поиск элементов с Деан в полях "Кому", "копия" или "Скрытая копия".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-157">Subject</span><span class="sxs-lookup"><span data-stu-id="9d3f7-157">Subject</span></span>  <br/> |<span data-ttu-id="9d3f7-158">Тема: Product</span><span class="sxs-lookup"><span data-stu-id="9d3f7-158">Subject:product</span></span>  <br/> <span data-ttu-id="9d3f7-159">Тема: (разработка продукта)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="9d3f7-160">Тема: "Разработка продуктов"</span><span class="sxs-lookup"><span data-stu-id="9d3f7-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="9d3f7-161">Поиск элементов с товаром в теме.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="9d3f7-162">Поиск элементов с продуктом и разработкой в теме.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-163">Основной текст</span><span class="sxs-lookup"><span data-stu-id="9d3f7-163">Body</span></span>  <br/> <span data-ttu-id="9d3f7-164">Контент</span><span class="sxs-lookup"><span data-stu-id="9d3f7-164">Content</span></span>  <br/> |<span data-ttu-id="9d3f7-165">Основной текст: ход выполнения</span><span class="sxs-lookup"><span data-stu-id="9d3f7-165">Body:progress</span></span>  <br/> <span data-ttu-id="9d3f7-166">Контент: ход выполнения</span><span class="sxs-lookup"><span data-stu-id="9d3f7-166">Content:progress</span></span>  <br/> |<span data-ttu-id="9d3f7-167">Поиск элементов с ходом выполнения в теле.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-168">Вложение</span><span class="sxs-lookup"><span data-stu-id="9d3f7-168">Attachment</span></span>  <br/> |<span data-ttu-id="9d3f7-169">Вложение: отчет</span><span class="sxs-lookup"><span data-stu-id="9d3f7-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="9d3f7-170">Поиск элементов с отчетом в имени файла вложения или в его тексте.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-171">(свойство не задано)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="9d3f7-172">Разработка продукта</span><span class="sxs-lookup"><span data-stu-id="9d3f7-172">Product Development</span></span>  <br/> |<span data-ttu-id="9d3f7-173">Поиск элементов, которые содержат как продукты, так и разработку во всех свойствах этапа слов.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="9d3f7-174">Сравнение ограничений для этапа Word всегда не учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="9d3f7-175">Ограничение на этап Word поддерживает два типа совпадений: совпадение префиксов или точное совпадение.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="9d3f7-176">Префикс "ПОИСКПОЗ" является поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="9d3f7-177">Если требуется точное совпадение, используйте двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="9d3f7-178">Например, Subject: "продукт" соответствует "продукту", но не "производству" в теме.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="9d3f7-179">Несколько слов в двойных кавычках ограничивают оба этапа и порядок слов.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="9d3f7-180">Например, "Win Product" соответствует только "Win Product", а не "Win95 Product" или "Product of Win".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="9d3f7-181">Можно использовать звездочку ( \* ), чтобы определить префикс с ограничением порядка.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="9d3f7-182">Например, "Win Product" \* соответствует "Win95 Product", "Windows Production Line", но не "Windows New Product" или "Product of Win".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="9d3f7-183">Можно выполнять поиск по всем сообщениям, отправляемым с домена или в домен.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="9d3f7-184">Например, from: "@hotmail. com" возвращает все сообщения, отправленные из hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="9d3f7-185">В следующей таблице описываются ограничения диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="9d3f7-186">**Ограничение диапазона дат**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-186">**Date range restriction**</span></span>

|<span data-ttu-id="9d3f7-187">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-187">**Property**</span></span>|<span data-ttu-id="9d3f7-188">**Пример**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-188">**Example**</span></span>|<span data-ttu-id="9d3f7-189">**Function**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9d3f7-190">Sent</span><span class="sxs-lookup"><span data-stu-id="9d3f7-190">Sent</span></span>  <br/> |<span data-ttu-id="9d3f7-191">Отправлено: на прошлой неделе</span><span class="sxs-lookup"><span data-stu-id="9d3f7-191">Sent:last week</span></span>  <br/> <span data-ttu-id="9d3f7-192">Отправлено: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="9d3f7-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="9d3f7-193">Отправлено: 01/01/2001.. 01/15/2001</span><span class="sxs-lookup"><span data-stu-id="9d3f7-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="9d3f7-194">Поиск элементов, отправленных за последнюю неделю.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="9d3f7-195">Поиск элементов, отправленных на 1 января 2001.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="9d3f7-196">Поиск элементов, отправленных между 1 января по 2001 и 15 января 2001.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-197">ПОЛУЧЕНО</span><span class="sxs-lookup"><span data-stu-id="9d3f7-197">Received</span></span>  <br/> |<span data-ttu-id="9d3f7-198">Получено: сегодня</span><span class="sxs-lookup"><span data-stu-id="9d3f7-198">Received:today</span></span>  <br/> <span data-ttu-id="9d3f7-199">Получено: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="9d3f7-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="9d3f7-200">Элементы поиска, полученные сегодня.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-200">Search items received today.</span></span>  <br/> <span data-ttu-id="9d3f7-201">Элементы поиска, полученные 1 января 2001 г.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="9d3f7-202">Две точки (..) — это оператор диапазона.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="9d3f7-203">Его можно использовать для определения диапазона с начальной и конечной датами.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="9d3f7-204">Чтобы указать дату, можно использовать относительные даты.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="9d3f7-205">Поддерживаются следующие относительные даты:</span><span class="sxs-lookup"><span data-stu-id="9d3f7-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="9d3f7-206">Относительные даты: сегодня, завтра, вчера</span><span class="sxs-lookup"><span data-stu-id="9d3f7-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="9d3f7-207">Относительные даты для нескольких слов: Эта неделя, следующий месяц, последняя неделя, последний месяц или следующий год</span><span class="sxs-lookup"><span data-stu-id="9d3f7-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="9d3f7-208">Дни: воскресенье, понедельник, вторник, среда, четверг, пятница, Суббота</span><span class="sxs-lookup"><span data-stu-id="9d3f7-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="9d3f7-209">Январь, Февраль, Март, Апрель, Май, Июнь, Июль, Август, Сентябрь, Октябрь, Ноябрь, Декабрь</span><span class="sxs-lookup"><span data-stu-id="9d3f7-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="9d3f7-210">В следующей таблице описываются ограничения на типы сообщений.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="9d3f7-211">**Ограничение на тип сообщения**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-211">**Message type restriction**</span></span>

|<span data-ttu-id="9d3f7-212">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-212">**Property**</span></span>|<span data-ttu-id="9d3f7-213">**Пример**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-213">**Example**</span></span>|<span data-ttu-id="9d3f7-214">**Function**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9d3f7-215">Kind</span><span class="sxs-lookup"><span data-stu-id="9d3f7-215">Kind</span></span>  <br/> |<span data-ttu-id="9d3f7-216">Вид: задачи</span><span class="sxs-lookup"><span data-stu-id="9d3f7-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="9d3f7-217">Поиск во всех элементах задач.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="9d3f7-218">AQS в EWS использует свойство **Kind** , чтобы указать тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="9d3f7-219">Свойство Kind можно использовать со следующими типами элементов:</span><span class="sxs-lookup"><span data-stu-id="9d3f7-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="9d3f7-220">email</span><span class="sxs-lookup"><span data-stu-id="9d3f7-220">email</span></span>
    
- <span data-ttu-id="9d3f7-221">meetings</span><span class="sxs-lookup"><span data-stu-id="9d3f7-221">meetings</span></span>
    
- <span data-ttu-id="9d3f7-222">tasks</span><span class="sxs-lookup"><span data-stu-id="9d3f7-222">tasks</span></span>
    
- <span data-ttu-id="9d3f7-223">notes</span><span class="sxs-lookup"><span data-stu-id="9d3f7-223">notes</span></span>
    
- <span data-ttu-id="9d3f7-224">docs</span><span class="sxs-lookup"><span data-stu-id="9d3f7-224">docs</span></span>
    
- <span data-ttu-id="9d3f7-225">journals</span><span class="sxs-lookup"><span data-stu-id="9d3f7-225">journals</span></span>
    
- <span data-ttu-id="9d3f7-226">contacts</span><span class="sxs-lookup"><span data-stu-id="9d3f7-226">contacts</span></span>
    
- <span data-ttu-id="9d3f7-227">im</span><span class="sxs-lookup"><span data-stu-id="9d3f7-227">im</span></span>
    
<span data-ttu-id="9d3f7-228">В следующей таблице описываются логические соединители группировки.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="9d3f7-229">**Группировка логических соединителей**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="9d3f7-230">**Connector**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-230">**Connector**</span></span>|<span data-ttu-id="9d3f7-231">**Пример**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-231">**Example**</span></span>|<span data-ttu-id="9d3f7-232">**Function**</span><span class="sxs-lookup"><span data-stu-id="9d3f7-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9d3f7-233">И</span><span class="sxs-lookup"><span data-stu-id="9d3f7-233">AND</span></span>  <br/> |<span data-ttu-id="9d3f7-234">Тема: продукт и Тема: Разработка</span><span class="sxs-lookup"><span data-stu-id="9d3f7-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="9d3f7-235">Тема: (продукт и разработка)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="9d3f7-236">Тема: (разработка продукта)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="9d3f7-237">Поиск элементов в теме с помощью продукта и разработки.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-238">OR</span><span class="sxs-lookup"><span data-stu-id="9d3f7-238">OR</span></span>  <br/> |<span data-ttu-id="9d3f7-239">Текст: проект или текст: предложение</span><span class="sxs-lookup"><span data-stu-id="9d3f7-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="9d3f7-240">Основной текст: (проект или предложение)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="9d3f7-241">Поиск элементов с помощью продукта или разработки в теле.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="9d3f7-242">NOT</span><span class="sxs-lookup"><span data-stu-id="9d3f7-242">NOT</span></span>  <br/> |<span data-ttu-id="9d3f7-243">НЕТ текста: предложение</span><span class="sxs-lookup"><span data-stu-id="9d3f7-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="9d3f7-244">Основной текст: (нет предложения)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="9d3f7-245">Поиск в сообщениях без предложения в теле.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="9d3f7-246">И всегда является соединителем по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-246">AND is always the default connector.</span></span> <span data-ttu-id="9d3f7-247">Например, Subject: Subject: Project и Body: предложение равно "subject": "Body": предложение.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="9d3f7-248">Логические соединители чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="9d3f7-249">Например, body: (проект или предложение) выполняет поиск в сообщениях с помощью "проект", "или" и "предложение" в тексте, а не "проект" или "предложение".</span><span class="sxs-lookup"><span data-stu-id="9d3f7-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="9d3f7-250">Символ "плюс" (+) эквивалентен и.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="9d3f7-251">Символ дефиса (-) эквивалентен параметру NOT.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="9d3f7-252">Например, body: (проект-предложение) выполняет поиск в сообщениях с "Project", но без предложения "предложение" в теле.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="9d3f7-253">Строка запроса также может содержать неиндексированные свойства для поиска.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="9d3f7-254">Если строка запроса содержит неиндексированные свойства, поиск может выполнить поиск Exchange по индексированным свойствам и поиск хранилища для неиндексированных свойств.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="9d3f7-255">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="9d3f7-256">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3f7-256">Example</span></span>

<span data-ttu-id="9d3f7-257">В приведенном ниже примере показан запрос на поиск сообщений в папке "Входящие" с автообнаружением в теме.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
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

<span data-ttu-id="9d3f7-258">В следующем примере показан успешный ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-258">The following example shows a successful response to the request.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="9d3f7-259">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9d3f7-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d3f7-260">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9d3f7-260">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d3f7-261">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9d3f7-261">Schema name</span></span>  <br/> |<span data-ttu-id="9d3f7-262">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9d3f7-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d3f7-263">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9d3f7-263">Validation file</span></span>  <br/> |<span data-ttu-id="9d3f7-264">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9d3f7-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d3f7-265">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9d3f7-265">Can be empty</span></span>  <br/> |<span data-ttu-id="9d3f7-266">False</span><span class="sxs-lookup"><span data-stu-id="9d3f7-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d3f7-267">См. также</span><span class="sxs-lookup"><span data-stu-id="9d3f7-267">See also</span></span>



[<span data-ttu-id="9d3f7-268">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="9d3f7-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="9d3f7-269">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="9d3f7-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="9d3f7-270">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d3f7-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

