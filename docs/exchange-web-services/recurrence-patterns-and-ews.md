---
title: Шаблоны повторения и веб-служб Exchange
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Сведения о шаблоны повторения и ряд повторяющейся в Exchange.
ms.openlocfilehash: ac10e9b9a347abb5907b77f0e0e7315e4e86d97a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761244"
---
# <a name="recurrence-patterns-and-ews"></a><span data-ttu-id="9d6a3-103">Шаблоны повторения и веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-103">Recurrence patterns and EWS</span></span>

<span data-ttu-id="9d6a3-104">Сведения о шаблоны повторения и ряд повторяющейся в Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-104">Learn about recurrence patterns and recurring series in Exchange.</span></span>
  
<span data-ttu-id="9d6a3-105">Серии повторяющихся — встречи или собрания, повторяет согласно заданному шаблону.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-105">A recurring series is an appointment or meeting that repeats according to a defined pattern.</span></span> <span data-ttu-id="9d6a3-106">Серии повторяющихся либо может иметь определенного количества экземпляров или можно повторить неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-106">A recurring series can either have a specific number of occurrences or can repeat indefinitely.</span></span> <span data-ttu-id="9d6a3-107">Кроме того, серии повторяющихся может иметь исключения, которые не отвечают шаблону остальную часть вхождений и может иметь вхождения, которые были удалены из шаблона.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-107">Additionally, a recurring series can have exceptions that don't follow the pattern of the rest of the occurrences, and can have occurrences that have been deleted from the pattern.</span></span> <span data-ttu-id="9d6a3-108">Для работы с серии повторяющихся и их элементы связанного календаря можно использовать управляемый API EWS и веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-108">You can use the EWS Managed API and EWS to work with recurring series and their associated calendar items.</span></span>
  
## <a name="recurring-calendar-items"></a><span data-ttu-id="9d6a3-109">Повторяющихся элементов календаря</span><span class="sxs-lookup"><span data-stu-id="9d6a3-109">Recurring calendar items</span></span>

<span data-ttu-id="9d6a3-110">Все элементы календаря попадают в одну из следующих четырех категорий:</span><span class="sxs-lookup"><span data-stu-id="9d6a3-110">All calendar items fall into one of the following four categories:</span></span>
  
- <span data-ttu-id="9d6a3-111">Неповторяющихся элементов календаря</span><span class="sxs-lookup"><span data-stu-id="9d6a3-111">Non-recurring calendar items</span></span>
    
- <span data-ttu-id="9d6a3-112">Повторяющееся образцов</span><span class="sxs-lookup"><span data-stu-id="9d6a3-112">Recurring masters</span></span>
    
- <span data-ttu-id="9d6a3-113">Вхождения в цикле</span><span class="sxs-lookup"><span data-stu-id="9d6a3-113">Occurrences in a series</span></span>
    
- <span data-ttu-id="9d6a3-114">Измененные вхождений в серии, известных как исключения</span><span class="sxs-lookup"><span data-stu-id="9d6a3-114">Modified occurrences in a series, known as exceptions</span></span>
    
<span data-ttu-id="9d6a3-115">В этой статье мы рассмотрим трех типов элементов календаря, являющихся частью серии повторяющихся.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-115">In this article, we'll look at the three types of calendar items that are part of a recurring series.</span></span>
  
<span data-ttu-id="9d6a3-116">Будет полезно понять, как повторяющееся реализован на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-116">It's helpful to understand how recurring series are implemented on the Exchange server.</span></span> <span data-ttu-id="9d6a3-117">Вместо создания элемент уникальных для каждого повтора в ряду, сервер создает только один элемент фактические в календаре, известных как образца повторения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-117">Instead of creating a separate distinct item for each occurrence in a recurring series, the server creates only one actual item in the calendar, known as the recurring master.</span></span> <span data-ttu-id="9d6a3-118">Формат образца повторения очень похоже на неповторяющейся встречи с добавлением информации шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-118">The format of a recurring master is very similar to a non-recurring appointment, with the addition of recurrence pattern information.</span></span> <span data-ttu-id="9d6a3-119">Сервер создает на основе шаблона повторения в ответ на запросы клиентов для данные о встрече, используя процесс с именем расширения вхождений.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-119">The server then generates occurrences based on the recurrence pattern in response to client requests for appointment information, using a process called expansion.</span></span> <span data-ttu-id="9d6a3-120">Эти созданный вхождений не сохраняются на сервере без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-120">These generated occurrences are not permanently stored on the server.</span></span> <span data-ttu-id="9d6a3-121">Это важно понимать, как поиск элементов календаря определяет, какие сведения о получении и ли расширение происходит.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-121">This is important to understand because the way that you search for calendar items determines what information you receive and whether expansion occurs.</span></span>
  
## <a name="recurrence-patterns"></a><span data-ttu-id="9d6a3-122">Расписания повторения</span><span class="sxs-lookup"><span data-stu-id="9d6a3-122">Recurrence patterns</span></span>

<span data-ttu-id="9d6a3-123">Основной блок в повторяющееся, который делает возможным расширения — это шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-123">The key piece to a recurring series that makes expansion possible is the recurrence pattern.</span></span> <span data-ttu-id="9d6a3-124">Шаблон повторения найдено в образце повторяющихся и описание набор критериев для расчета вхождений на основе даты и времени образца повторения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-124">The recurrence pattern is found on the recurring master, and describes a set of criteria for calculating occurrences based on the date and time of the recurring master.</span></span>
  
<span data-ttu-id="9d6a3-125">**В таблице 1. Шаблоны повторения недоступны**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-125">**Table 1. Available recurrence patterns**</span></span>

|<span data-ttu-id="9d6a3-126">**Управляемый API EWS класс**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-126">**EWS Managed API class**</span></span>|<span data-ttu-id="9d6a3-127">**Элемент веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-127">**EWS element**</span></span>|<span data-ttu-id="9d6a3-128">**�������**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-128">**Examples**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="9d6a3-129">Recurrence.DailyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-129">Recurrence.DailyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-130">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-130">DailyRecurrence</span></span>](http://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-131">Повторите каждый день.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-131">Repeat every day.</span></span>  <br/> <span data-ttu-id="9d6a3-132">Повторите каждый второй день.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-132">Repeat every other day.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-133">Recurrence.MonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-133">Recurrence.MonthlyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-134">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-134">AbsoluteMonthlyRecurrence</span></span>](http://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-135">Повторите ежемесячно в 10 день месяца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-135">Repeat every month on the tenth day of the month.</span></span>  <br/> <span data-ttu-id="9d6a3-136">Повторите каждые два месяца двадцати первый день месяца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-136">Repeat every other month on the twenty-first day of the month.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-137">Recurrence.RelativeMonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-137">Recurrence.RelativeMonthlyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-138">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-138">RelativeMonthlyRecurrence</span></span>](http://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-139">Повторите во второй вторник каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-139">Repeat on the second Tuesday of every month.</span></span>  <br/> <span data-ttu-id="9d6a3-140">Повторите в третий четверг каждые три месяца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-140">Repeat on the third Thursday of the month every three months.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-141">Recurrence.RelativeYearlyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-141">Recurrence.RelativeYearlyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-142">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-142">RelativeYearlyRecurrence</span></span>](http://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-143">Повторите в первый понедельник августа каждый год.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-143">Repeat on the first Monday of August every year.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-144">Recurrence.WeeklyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-144">Recurrence.WeeklyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-145">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-145">WeeklyRecurrence</span></span>](http://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-146">Повторите каждый понедельник.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-146">Repeat every Monday.</span></span>  <br/> <span data-ttu-id="9d6a3-147">Повторите вторникам и четверг каждые две недели.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-147">Repeat every Tuesday and Thursday every other week.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-148">Recurrence.YearlyPattern</span><span class="sxs-lookup"><span data-stu-id="9d6a3-148">Recurrence.YearlyPattern</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-149">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-149">AbsoluteYearlyRecurrence</span></span>](http://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-150">Повторите на 1-го сентября каждый год.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-150">Repeat on September 1st every year.</span></span>  <br/> |
   
<span data-ttu-id="9d6a3-151">Другие важную информацию для шаблона повторения — при завершении повторения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-151">The other important piece of information for a recurrence pattern is when the recurrence ends.</span></span> <span data-ttu-id="9d6a3-152">Это может быть выражено как заданное количество вхождений, Дата завершения или необходимости нет конца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-152">This can be expressed as either a set number of occurrences, as an end date, or as having no end.</span></span>
  
<span data-ttu-id="9d6a3-153">**В таблице 2. Параметры для окончания встречи**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-153">**Table 2. Options for the end of a recurring series**</span></span>

|<span data-ttu-id="9d6a3-154">**Управляемый API EWS метод или свойство**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-154">**EWS Managed API method/property**</span></span>|<span data-ttu-id="9d6a3-155">**Элемент веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-155">**EWS element**</span></span>|<span data-ttu-id="9d6a3-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-156">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="9d6a3-157">Recurrence.NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="9d6a3-157">Recurrence.NumberOfOccurrences</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-158">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-158">NumberedRecurrence</span></span>](http://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-159">Значение этого свойства или элемент указывает число вхождений.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-159">The value of this property or element specifies the number of occurrences.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-160">Recurrence.EndDate</span><span class="sxs-lookup"><span data-stu-id="9d6a3-160">Recurrence.EndDate</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-161">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-161">EndDateRecurrence</span></span>](http://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-162">Последнее вхождение в серии попадает на или до даты, указанного идентификатором этого свойства или элемента.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-162">The last occurrence in the series falls on or before the date specified by this property or element.</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-163">Recurrence.HasEnd</span><span class="sxs-lookup"><span data-stu-id="9d6a3-163">Recurrence.HasEnd</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9d6a3-164">Recurrence.NeverEnds</span><span class="sxs-lookup"><span data-stu-id="9d6a3-164">Recurrence.NeverEnds</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9d6a3-165">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d6a3-165">NoEndRecurrence</span></span>](http://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |<span data-ttu-id="9d6a3-166">Серия имеет нет конца.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-166">The series has no end.</span></span>  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a><span data-ttu-id="9d6a3-167">Расширенное и не были развернуты представлений</span><span class="sxs-lookup"><span data-stu-id="9d6a3-167">Expanded vs. non-expanded views</span></span>

<span data-ttu-id="9d6a3-168">С помощью метода **FindAppointments** в управляемый API веб-служб Exchange (или операции **FindItem** с элементом **представления календаря** в веб-служб Exchange) вызывает процесса расширения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-168">Using the **FindAppointments** method in the EWS Managed API (or the **FindItem** operation with a **CalendarView** element in EWS) invokes the expansion process.</span></span> <span data-ttu-id="9d6a3-169">Это скрывает повторяющихся встреч главных в наборе результатов и вместо этого представляет расширенное представление этого повторяющегося ряда.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-169">This hides recurring master appointments from the result set, and instead presents an expanded view of that recurring series.</span></span> <span data-ttu-id="9d6a3-170">Вхождения и исключения повторяющихся образец, попадающие в параметры представления календаря включены в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-170">Occurrences of and exceptions to the recurring master that fall within the parameters of the calendar view are included in the result set.</span></span> <span data-ttu-id="9d6a3-171">С другой стороны, с помощью метода **FindItems** в управляемый API веб-служб Exchange (или операции **FindItem** с **IndexedPageItemView** или **FractionalPageItemView** элемент в веб-служб Exchange), не вызывает процесса расширения и вхождений и исключения, не включаются.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-171">Conversely, using the **FindItems** method in the EWS Managed API (or the **FindItem** operation with a **IndexedPageItemView** or **FractionalPageItemView** element in EWS), does not invoke the expansion process, and occurrences and exceptions are not included.</span></span> <span data-ttu-id="9d6a3-172">Давайте рассмотрим пример сравнения двух методов.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-172">Let's look at an example comparing the two methods.</span></span> 
  
<span data-ttu-id="9d6a3-173">**В таблице 3. Методы и операций поиска встреч**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-173">**Table 3. Methods and operations for finding appointments**</span></span>

|<span data-ttu-id="9d6a3-174">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-174">**EWS Managed API method**</span></span>|<span data-ttu-id="9d6a3-175">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-175">**EWS operation**</span></span>|<span data-ttu-id="9d6a3-176">**При развертывании серии?**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-176">**Expands series?**</span></span>|<span data-ttu-id="9d6a3-177">**Компоненты, входящие в результаты**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-177">**Items included in results**</span></span>|
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9d6a3-178">ExchangeService.FindAppointments</span><span class="sxs-lookup"><span data-stu-id="9d6a3-178">ExchangeService.FindAppointments</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="9d6a3-179">[Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [представления календаря](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="9d6a3-179">[FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with a [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="9d6a3-180">Да</span><span class="sxs-lookup"><span data-stu-id="9d6a3-180">Yes</span></span>  <br/> |<span data-ttu-id="9d6a3-181">Неповторяющихся встреч, отдельных экземпляров повторяющегося ряда и исключений из серии повторяющихся</span><span class="sxs-lookup"><span data-stu-id="9d6a3-181">Non-recurring appointments, single occurrences of recurring series, and exceptions to recurring series</span></span>  <br/> |
|[<span data-ttu-id="9d6a3-182">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="9d6a3-182">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="9d6a3-183">[Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) элемент или элемент [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="9d6a3-183">[FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with an [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="9d6a3-184">Нет</span><span class="sxs-lookup"><span data-stu-id="9d6a3-184">No</span></span>  <br/> |<span data-ttu-id="9d6a3-185">Неповторяющихся встреч и повторяющихся встреч главной</span><span class="sxs-lookup"><span data-stu-id="9d6a3-185">Non-recurring appointments and recurring master appointments</span></span>  <br/> |
   
<span data-ttu-id="9d6a3-186">Sadie выполнил установил сын для swim группы.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-186">Sadie has just signed her son up for swim team.</span></span> <span data-ttu-id="9d6a3-187">Группа имеет practice каждый день в 8:30:00 утра среда запуск 2 июля с последней, прием на 6 августа.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-187">The team has practice every Wednesday morning at 8:30 AM, starting July 2, with the last practice being on August 6.</span></span> <span data-ttu-id="9d6a3-188">Желающие не забудьте о practice, Sadie добавляет повторяющейся встречи в свой календарь, чтобы напомнить ему.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-188">Not wanting to forget about practice, Sadie adds a recurring appointment to her calendar to remind her.</span></span>
  
<span data-ttu-id="9d6a3-189">**В таблице 4. Sadie's повторяющейся встречи**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-189">**Table 4. Sadie's recurring appointment**</span></span>

|<span data-ttu-id="9d6a3-190">**Поле встречи**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-190">**Appointment field**</span></span>|<span data-ttu-id="9d6a3-191">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9d6a3-191">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9d6a3-192">Subject</span><span class="sxs-lookup"><span data-stu-id="9d6a3-192">Subject</span></span>  <br/> |<span data-ttu-id="9d6a3-193">Swim Practice группы</span><span class="sxs-lookup"><span data-stu-id="9d6a3-193">Swim Team Practice</span></span>  <br/> |
|<span data-ttu-id="9d6a3-194">Начало</span><span class="sxs-lookup"><span data-stu-id="9d6a3-194">Start</span></span>  <br/> |<span data-ttu-id="9d6a3-195">2 июля 2014 г. 8:30:00</span><span class="sxs-lookup"><span data-stu-id="9d6a3-195">July 2, 2014 8:30 AM</span></span>  <br/> |
|<span data-ttu-id="9d6a3-196">End</span><span class="sxs-lookup"><span data-stu-id="9d6a3-196">End</span></span>  <br/> |<span data-ttu-id="9d6a3-197">2 июля 2014 г. 10:00 по</span><span class="sxs-lookup"><span data-stu-id="9d6a3-197">July 2, 2014 10:00 AM</span></span>  <br/> |
|<span data-ttu-id="9d6a3-198">Повторяется</span><span class="sxs-lookup"><span data-stu-id="9d6a3-198">Recurs</span></span>  <br/> |<span data-ttu-id="9d6a3-199">Каждую среду</span><span class="sxs-lookup"><span data-stu-id="9d6a3-199">Every Wednesday</span></span>  <br/> |
|<span data-ttu-id="9d6a3-200">Последнее вхождение</span><span class="sxs-lookup"><span data-stu-id="9d6a3-200">Last occurrence</span></span>  <br/> |<span data-ttu-id="9d6a3-201">6 августа 2014 г. 8:30:00</span><span class="sxs-lookup"><span data-stu-id="9d6a3-201">August 6, 2014 8:30 AM</span></span>  <br/> |
   
<span data-ttu-id="9d6a3-202">Краткий обзор календаря показывает, что команда будет иметь всего шесть рекомендациям.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-202">A quick look at a calendar shows that the team will have a total of six practices.</span></span> <span data-ttu-id="9d6a3-203">Тем не менее не существует шесть элементов различных встречи в календаре.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-203">However, there aren't six distinct appointment items in the calendar.</span></span> <span data-ttu-id="9d6a3-204">Вместо этого существует только один повторяющейся встречи главной, представляющее серии.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-204">Instead, there is just one recurring master appointment representing the series.</span></span>
  
<span data-ttu-id="9d6a3-205">Теперь давайте взглянем на поиск встреч в календаре пользователя Sadie, которые происходят в рамках июля.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-205">Now let's look at finding appointments on Sadie's calendar that occur within the month of July.</span></span> <span data-ttu-id="9d6a3-206">В следующем примере кода метод **FindItems** в управляемый API Exchange для создания представления не были развернуты Sadie элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-206">The following code example uses the **FindItems** method in the Exchange Managed API to produce a non-expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="9d6a3-207">Этот код приводит к следующей запрос [FindItem операции](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9d6a3-207">That code results in the following [FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with an [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9d6a3-208">Ответ сервера включает в себя только один элемент, хозяином повторяющихся указанный в параметре значение элемента [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) **RecurringMaster**.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-208">The server's response includes only a single item, the recurring master, indicated by the [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element value of **RecurringMaster**.</span></span> <span data-ttu-id="9d6a3-209">Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-209">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="9d6a3-210">Теперь давайте сравнить с расширенное представление.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-210">Now let's compare with an expanded view.</span></span> <span data-ttu-id="9d6a3-211">В следующем примере кода метод **FindAppointments** в управляемый API веб-служб Exchange для создания развернутого представления календаря в Sadie.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-211">The following code example uses the **FindAppointments** method in the EWS Managed API to create an expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="9d6a3-212">Этот код приводит к следующей [операции FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) запроса с элемент [представления календаря](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9d6a3-212">This code results in the following [FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with a [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9d6a3-213">Настоящее время отклика сервера включает в себя пять вхождений, другая — для каждого среда июля.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-213">This time, the server response includes five occurrences, one for each Wednesday in July.</span></span> <span data-ttu-id="9d6a3-214">Элементы [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) на все эти элементы имеют значение **экземпляра**.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-214">The [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) elements on these items all have a value of **Occurrence**.</span></span> <span data-ttu-id="9d6a3-215">Обратите внимание, что повторяющиеся главных не указан в ответе.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-215">Note that the recurring master is not present in the response.</span></span> <span data-ttu-id="9d6a3-216">Значения элементов [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-216">The values of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="9d6a3-217">После того как образцом повторения, вхождения или исключение всегда можно [извлечь связанные элементы](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="9d6a3-217">After you have a recurring master, an occurrence, or an exception, you can always [retrieve the other related items](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="9d6a3-218">Учитывая вхождение или исключение, вы можете получить повторяющихся основной и наоборот.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-218">Given an occurrence or exception, you can retrieve the recurring master, and vice versa.</span></span>
  
## <a name="working-with-recurring-calendar-items"></a><span data-ttu-id="9d6a3-219">Работа с повторяющихся элементов календаря</span><span class="sxs-lookup"><span data-stu-id="9d6a3-219">Working with recurring calendar items</span></span>

<span data-ttu-id="9d6a3-220">Можно использовать те же операций и методы для работы с серии повторяющихся как для работы с элементами календаря неповторяющейся.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-220">You use all the same methods and operations to work with recurring series as you use to work with non-recurring calendar items.</span></span> <span data-ttu-id="9d6a3-221">Отличие заключается, что в зависимости от того, элемент, который можно использовать для вызова этих методов или операции, выполняемые действия можно применять для всего ряда или только одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-221">The difference is that, depending on the item you use to invoke those methods or operations, the actions you take can apply to the entire series, or just a single occurrence.</span></span> <span data-ttu-id="9d6a3-222">[Действия, предпринимаемые в образце повторяющихся](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) будут применяться ко все вхождения серии, во время [действия, предпринимаемые для одного экземпляра или исключение](how-to-update-a-recurring-series-by-using-ews.md) применяется только к этому вхождение или исключение.</span><span class="sxs-lookup"><span data-stu-id="9d6a3-222">[Actions taken on the recurring master](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) will apply to all occurrences in the series, while [actions taken to a single occurrence or exception](how-to-update-a-recurring-series-by-using-ews.md) will only apply to that occurrence or exception.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="9d6a3-223">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="9d6a3-223">In this section</span></span>

- [<span data-ttu-id="9d6a3-224">Доступ к ряду с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-224">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d6a3-225">Создание встречи с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-225">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d6a3-226">Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-226">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d6a3-227">Обновление серии повторяющихся с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-227">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="9d6a3-228">Обновление серии повторяющихся с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-228">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="9d6a3-229">См. также</span><span class="sxs-lookup"><span data-stu-id="9d6a3-229">See also</span></span>


- [<span data-ttu-id="9d6a3-230">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-230">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="9d6a3-231">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-231">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="9d6a3-232">Получение встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d6a3-232">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

