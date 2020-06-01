---
title: Шаблоны повторения и EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Сведения о шаблонах повторения и повторяющихся рядах в Exchange.
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459330"
---
# <a name="recurrence-patterns-and-ews"></a><span data-ttu-id="d1243-103">Шаблоны повторения и EWS</span><span class="sxs-lookup"><span data-stu-id="d1243-103">Recurrence patterns and EWS</span></span>

<span data-ttu-id="d1243-104">Сведения о шаблонах повторения и повторяющихся рядах в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1243-104">Learn about recurrence patterns and recurring series in Exchange.</span></span>
  
<span data-ttu-id="d1243-105">Повторяющийся ряд — это встреча или собрание, повторяющиеся в соответствии с определенным шаблоном.</span><span class="sxs-lookup"><span data-stu-id="d1243-105">A recurring series is an appointment or meeting that repeats according to a defined pattern.</span></span> <span data-ttu-id="d1243-106">Повторяющиеся ряды могут иметь определенное количество повторений или может повторяться в течение неопределенного периода.</span><span class="sxs-lookup"><span data-stu-id="d1243-106">A recurring series can either have a specific number of occurrences or can repeat indefinitely.</span></span> <span data-ttu-id="d1243-107">Кроме того, повторяющиеся ряды могут содержать исключения, которые не следуют шаблону остальных вхождений, и могут иметь экземпляры, удаленные из шаблона.</span><span class="sxs-lookup"><span data-stu-id="d1243-107">Additionally, a recurring series can have exceptions that don't follow the pattern of the rest of the occurrences, and can have occurrences that have been deleted from the pattern.</span></span> <span data-ttu-id="d1243-108">Вы можете использовать управляемый API EWS и EWS для работы с повторяющимися сериями и связанными с ними элементами календаря.</span><span class="sxs-lookup"><span data-stu-id="d1243-108">You can use the EWS Managed API and EWS to work with recurring series and their associated calendar items.</span></span>
  
## <a name="recurring-calendar-items"></a><span data-ttu-id="d1243-109">Повторяющиеся элементы календаря</span><span class="sxs-lookup"><span data-stu-id="d1243-109">Recurring calendar items</span></span>

<span data-ttu-id="d1243-110">Все элементы календаря делятся на одну из следующих четырех категорий:</span><span class="sxs-lookup"><span data-stu-id="d1243-110">All calendar items fall into one of the following four categories:</span></span>
  
- <span data-ttu-id="d1243-111">Неповторяющиеся элементы календаря</span><span class="sxs-lookup"><span data-stu-id="d1243-111">Non-recurring calendar items</span></span>
    
- <span data-ttu-id="d1243-112">Повторяющиеся шаблоны</span><span class="sxs-lookup"><span data-stu-id="d1243-112">Recurring masters</span></span>
    
- <span data-ttu-id="d1243-113">Вхождения в серии</span><span class="sxs-lookup"><span data-stu-id="d1243-113">Occurrences in a series</span></span>
    
- <span data-ttu-id="d1243-114">Измененные экземпляры в серии, называемые исключениями</span><span class="sxs-lookup"><span data-stu-id="d1243-114">Modified occurrences in a series, known as exceptions</span></span>
    
<span data-ttu-id="d1243-115">В этой статье мы рассмотрим три типа элементов календаря, которые входят в повторяющиеся ряды.</span><span class="sxs-lookup"><span data-stu-id="d1243-115">In this article, we'll look at the three types of calendar items that are part of a recurring series.</span></span>
  
<span data-ttu-id="d1243-116">Полезно знать, как повторяющиеся ряды реализуются на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1243-116">It's helpful to understand how recurring series are implemented on the Exchange server.</span></span> <span data-ttu-id="d1243-117">Вместо того чтобы создавать отдельный отдельный элемент для каждого вхождения в повторяющейся серии, сервер создает в календаре только один фактический элемент, называемый повторяющимся образцом.</span><span class="sxs-lookup"><span data-stu-id="d1243-117">Instead of creating a separate distinct item for each occurrence in a recurring series, the server creates only one actual item in the calendar, known as the recurring master.</span></span> <span data-ttu-id="d1243-118">Формат повторяющейся основной схемы очень похож на неповторяющуюся встречу с добавлением сведений о расписании повторения.</span><span class="sxs-lookup"><span data-stu-id="d1243-118">The format of a recurring master is very similar to a non-recurring appointment, with the addition of recurrence pattern information.</span></span> <span data-ttu-id="d1243-119">Затем сервер создает экземпляры на основе шаблона повторения в ответ на клиентские запросы для сведений о встрече, используя процесс, называемый расширением.</span><span class="sxs-lookup"><span data-stu-id="d1243-119">The server then generates occurrences based on the recurrence pattern in response to client requests for appointment information, using a process called expansion.</span></span> <span data-ttu-id="d1243-120">Эти созданные экземпляры не будут безвозвратно храниться на сервере.</span><span class="sxs-lookup"><span data-stu-id="d1243-120">These generated occurrences are not permanently stored on the server.</span></span> <span data-ttu-id="d1243-121">Это важно понимать, так как поиск элементов календаря определяет, какие сведения вы получаете и как происходит расширение.</span><span class="sxs-lookup"><span data-stu-id="d1243-121">This is important to understand because the way that you search for calendar items determines what information you receive and whether expansion occurs.</span></span>
  
## <a name="recurrence-patterns"></a><span data-ttu-id="d1243-122">Расписания повторения</span><span class="sxs-lookup"><span data-stu-id="d1243-122">Recurrence patterns</span></span>

<span data-ttu-id="d1243-123">Основной частью ряда повторяющихся данных является периодичность расширения.</span><span class="sxs-lookup"><span data-stu-id="d1243-123">The key piece to a recurring series that makes expansion possible is the recurrence pattern.</span></span> <span data-ttu-id="d1243-124">Шаблон повторения находится на повторяющейся основной странице, а также описывает набор критериев для расчета вхождений на основе даты и времени повторяющегося образца.</span><span class="sxs-lookup"><span data-stu-id="d1243-124">The recurrence pattern is found on the recurring master, and describes a set of criteria for calculating occurrences based on the date and time of the recurring master.</span></span>
  
<span data-ttu-id="d1243-125">**Таблица 1. Доступные шаблоны повторения**</span><span class="sxs-lookup"><span data-stu-id="d1243-125">**Table 1. Available recurrence patterns**</span></span>

|<span data-ttu-id="d1243-126">**Класс управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-126">**EWS Managed API class**</span></span>|<span data-ttu-id="d1243-127">**Элемент EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-127">**EWS element**</span></span>|<span data-ttu-id="d1243-128">**Примеры**</span><span class="sxs-lookup"><span data-stu-id="d1243-128">**Examples**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="d1243-129">Повторение. Даилипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-129">Recurrence.DailyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-130">даилирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-130">DailyRecurrence</span></span>](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-131">Повторять каждый день.</span><span class="sxs-lookup"><span data-stu-id="d1243-131">Repeat every day.</span></span>  <br/> <span data-ttu-id="d1243-132">Повторять каждый день.</span><span class="sxs-lookup"><span data-stu-id="d1243-132">Repeat every other day.</span></span>  <br/> |
|[<span data-ttu-id="d1243-133">Повторение. Монслипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-133">Recurrence.MonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-134">абсолутемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-134">AbsoluteMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-135">Повторять каждый месяц на десятый день месяца.</span><span class="sxs-lookup"><span data-stu-id="d1243-135">Repeat every month on the tenth day of the month.</span></span>  <br/> <span data-ttu-id="d1243-136">Повторять каждый второй месяц в двадцать первый день месяца.</span><span class="sxs-lookup"><span data-stu-id="d1243-136">Repeat every other month on the twenty-first day of the month.</span></span>  <br/> |
|[<span data-ttu-id="d1243-137">Повторение. Релативемонслипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-137">Recurrence.RelativeMonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-138">релативемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-138">RelativeMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-139">Повторяйте во второй вторник каждого месяца.</span><span class="sxs-lookup"><span data-stu-id="d1243-139">Repeat on the second Tuesday of every month.</span></span>  <br/> <span data-ttu-id="d1243-140">Повторяйте в третий четверг месяца каждые три месяца.</span><span class="sxs-lookup"><span data-stu-id="d1243-140">Repeat on the third Thursday of the month every three months.</span></span>  <br/> |
|[<span data-ttu-id="d1243-141">Повторение. Релативэйеарлипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-141">Recurrence.RelativeYearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-142">релативэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-142">RelativeYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-143">Повторяйте на первом понедельник августа каждый год.</span><span class="sxs-lookup"><span data-stu-id="d1243-143">Repeat on the first Monday of August every year.</span></span>  <br/> |
|[<span data-ttu-id="d1243-144">Повторение. Виклипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-144">Recurrence.WeeklyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-145">виклирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-145">WeeklyRecurrence</span></span>](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-146">Повторяйте каждый понедельник.</span><span class="sxs-lookup"><span data-stu-id="d1243-146">Repeat every Monday.</span></span>  <br/> <span data-ttu-id="d1243-147">Повторяйте каждый вторник и четверг каждую вторую неделю.</span><span class="sxs-lookup"><span data-stu-id="d1243-147">Repeat every Tuesday and Thursday every other week.</span></span>  <br/> |
|[<span data-ttu-id="d1243-148">Повторение. Еарлипаттерн</span><span class="sxs-lookup"><span data-stu-id="d1243-148">Recurrence.YearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-149">абсолутэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-149">AbsoluteYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-150">Повторяйте каждый год 1 сентября.</span><span class="sxs-lookup"><span data-stu-id="d1243-150">Repeat on September 1st every year.</span></span>  <br/> |
   
<span data-ttu-id="d1243-151">Другой важный фрагмент данных для шаблона повторения — по окончании повторения.</span><span class="sxs-lookup"><span data-stu-id="d1243-151">The other important piece of information for a recurrence pattern is when the recurrence ends.</span></span> <span data-ttu-id="d1243-152">Может быть выражено как заданное число повторений, как Дата окончания, так и без окончания.</span><span class="sxs-lookup"><span data-stu-id="d1243-152">This can be expressed as either a set number of occurrences, as an end date, or as having no end.</span></span>
  
<span data-ttu-id="d1243-153">**Таблица 2. Варианты для конца повторяющейся серии**</span><span class="sxs-lookup"><span data-stu-id="d1243-153">**Table 2. Options for the end of a recurring series**</span></span>

|<span data-ttu-id="d1243-154">**Метод или свойство управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-154">**EWS Managed API method/property**</span></span>|<span data-ttu-id="d1243-155">**Элемент EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-155">**EWS element**</span></span>|<span data-ttu-id="d1243-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d1243-156">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="d1243-157">Повторение. Нумберофоккурренцес</span><span class="sxs-lookup"><span data-stu-id="d1243-157">Recurrence.NumberOfOccurrences</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-158">нумбередрекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-158">NumberedRecurrence</span></span>](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-159">Значение этого свойства или элемента указывает количество повторений.</span><span class="sxs-lookup"><span data-stu-id="d1243-159">The value of this property or element specifies the number of occurrences.</span></span>  <br/> |
|[<span data-ttu-id="d1243-160">Повторение. EndDate</span><span class="sxs-lookup"><span data-stu-id="d1243-160">Recurrence.EndDate</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-161">енддатерекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-161">EndDateRecurrence</span></span>](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-162">Последнее вхождение в ряду приходится на или предшествует дате, указанной этим свойством или элементом.</span><span class="sxs-lookup"><span data-stu-id="d1243-162">The last occurrence in the series falls on or before the date specified by this property or element.</span></span>  <br/> |
|[<span data-ttu-id="d1243-163">Повторение. Хасенд</span><span class="sxs-lookup"><span data-stu-id="d1243-163">Recurrence.HasEnd</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d1243-164">Повторение. Неверендс</span><span class="sxs-lookup"><span data-stu-id="d1243-164">Recurrence.NeverEnds</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d1243-165">ноендрекурренце</span><span class="sxs-lookup"><span data-stu-id="d1243-165">NoEndRecurrence</span></span>](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |<span data-ttu-id="d1243-166">У ряда нет конца.</span><span class="sxs-lookup"><span data-stu-id="d1243-166">The series has no end.</span></span>  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a><span data-ttu-id="d1243-167">Расширенные и нерасширенные представления</span><span class="sxs-lookup"><span data-stu-id="d1243-167">Expanded vs. non-expanded views</span></span>

<span data-ttu-id="d1243-168">Вызов процесса расширения с помощью метода **FindAppointments** в УПРАВЛЯЕМОМ API EWS (или операции **FindItem** с элементом **CalendarView** в EWS).</span><span class="sxs-lookup"><span data-stu-id="d1243-168">Using the **FindAppointments** method in the EWS Managed API (or the **FindItem** operation with a **CalendarView** element in EWS) invokes the expansion process.</span></span> <span data-ttu-id="d1243-169">Это скрывает повторяющиеся основные встречи из набора результатов, а вместо этого предоставляет расширенное представление этой серии.</span><span class="sxs-lookup"><span data-stu-id="d1243-169">This hides recurring master appointments from the result set, and instead presents an expanded view of that recurring series.</span></span> <span data-ttu-id="d1243-170">Экземпляры и исключения из повторяющейся основной реплики, которые попадают в параметры представления календаря, включаются в результирующий набор.</span><span class="sxs-lookup"><span data-stu-id="d1243-170">Occurrences of and exceptions to the recurring master that fall within the parameters of the calendar view are included in the result set.</span></span> <span data-ttu-id="d1243-171">С другой стороны, с помощью метода **FindItems** в УПРАВЛЯЕМОМ API EWS (или операции **FindItem** с элементом **индекседпажеитемвиев** или **фрактионалпажеитемвиев** в EWS) не вызывается процесс расширения, а экземпляры и исключения не включаются.</span><span class="sxs-lookup"><span data-stu-id="d1243-171">Conversely, using the **FindItems** method in the EWS Managed API (or the **FindItem** operation with a **IndexedPageItemView** or **FractionalPageItemView** element in EWS), does not invoke the expansion process, and occurrences and exceptions are not included.</span></span> <span data-ttu-id="d1243-172">Рассмотрим пример сравнения двух методов.</span><span class="sxs-lookup"><span data-stu-id="d1243-172">Let's look at an example comparing the two methods.</span></span> 
  
<span data-ttu-id="d1243-173">**Таблица 3. Методы и операции для поиска встреч**</span><span class="sxs-lookup"><span data-stu-id="d1243-173">**Table 3. Methods and operations for finding appointments**</span></span>

|<span data-ttu-id="d1243-174">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-174">**EWS Managed API method**</span></span>|<span data-ttu-id="d1243-175">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="d1243-175">**EWS operation**</span></span>|<span data-ttu-id="d1243-176">**Разворачивает ряды?**</span><span class="sxs-lookup"><span data-stu-id="d1243-176">**Expands series?**</span></span>|<span data-ttu-id="d1243-177">**Элементы, включенные в результаты**</span><span class="sxs-lookup"><span data-stu-id="d1243-177">**Items included in results**</span></span>|
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d1243-178">ExchangeService. FindAppointments</span><span class="sxs-lookup"><span data-stu-id="d1243-178">ExchangeService.FindAppointments</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="d1243-179">[Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d1243-179">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="d1243-180">Да</span><span class="sxs-lookup"><span data-stu-id="d1243-180">Yes</span></span>  <br/> |<span data-ttu-id="d1243-181">Неповторяющиеся встречи, отдельные экземпляры повторяющихся рядов и исключения из повторяющихся рядов</span><span class="sxs-lookup"><span data-stu-id="d1243-181">Non-recurring appointments, single occurrences of recurring series, and exceptions to recurring series</span></span>  <br/> |
|[<span data-ttu-id="d1243-182">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="d1243-182">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="d1243-183">[Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [Индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элементом [фрактионалпажеитемвиев](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d1243-183">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="d1243-184">Нет</span><span class="sxs-lookup"><span data-stu-id="d1243-184">No</span></span>  <br/> |<span data-ttu-id="d1243-185">Неповторяющиеся встречи и повторяющиеся запланированные встречи</span><span class="sxs-lookup"><span data-stu-id="d1243-185">Non-recurring appointments and recurring master appointments</span></span>  <br/> |
   
<span data-ttu-id="d1243-186">Ольга только что подписался на себя для группы свим.</span><span class="sxs-lookup"><span data-stu-id="d1243-186">Sadie has just signed her son up for swim team.</span></span> <span data-ttu-id="d1243-187">У группы есть упражнения каждую среду утром в 8:30 AM, начиная с 2 июля, с последней практикой из 6 августа.</span><span class="sxs-lookup"><span data-stu-id="d1243-187">The team has practice every Wednesday morning at 8:30 AM, starting July 2, with the last practice being on August 6.</span></span> <span data-ttu-id="d1243-188">Не нужно забывать о практике, Ольга добавляет повторяющуюся встречу в свой календарь для напоминания.</span><span class="sxs-lookup"><span data-stu-id="d1243-188">Not wanting to forget about practice, Sadie adds a recurring appointment to her calendar to remind her.</span></span>
  
<span data-ttu-id="d1243-189">**Таблица 4. Повторяющаяся встреча Ольга**</span><span class="sxs-lookup"><span data-stu-id="d1243-189">**Table 4. Sadie's recurring appointment**</span></span>

|<span data-ttu-id="d1243-190">**Поле "Встреча"**</span><span class="sxs-lookup"><span data-stu-id="d1243-190">**Appointment field**</span></span>|<span data-ttu-id="d1243-191">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d1243-191">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1243-192">Subject</span><span class="sxs-lookup"><span data-stu-id="d1243-192">Subject</span></span>  <br/> |<span data-ttu-id="d1243-193">Практика группы свим</span><span class="sxs-lookup"><span data-stu-id="d1243-193">Swim Team Practice</span></span>  <br/> |
|<span data-ttu-id="d1243-194">Начало</span><span class="sxs-lookup"><span data-stu-id="d1243-194">Start</span></span>  <br/> |<span data-ttu-id="d1243-195">2 июля 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="d1243-195">July 2, 2014 8:30 AM</span></span>  <br/> |
|<span data-ttu-id="d1243-196">Конец</span><span class="sxs-lookup"><span data-stu-id="d1243-196">End</span></span>  <br/> |<span data-ttu-id="d1243-197">2 июля 2014 10:00 AM</span><span class="sxs-lookup"><span data-stu-id="d1243-197">July 2, 2014 10:00 AM</span></span>  <br/> |
|<span data-ttu-id="d1243-198">Повторяется</span><span class="sxs-lookup"><span data-stu-id="d1243-198">Recurs</span></span>  <br/> |<span data-ttu-id="d1243-199">Каждую среду</span><span class="sxs-lookup"><span data-stu-id="d1243-199">Every Wednesday</span></span>  <br/> |
|<span data-ttu-id="d1243-200">Последнее событие</span><span class="sxs-lookup"><span data-stu-id="d1243-200">Last occurrence</span></span>  <br/> |<span data-ttu-id="d1243-201">6 августа 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="d1243-201">August 6, 2014 8:30 AM</span></span>  <br/> |
   
<span data-ttu-id="d1243-202">Краткий обзор календаря показывает, что у команды будет всего шесть практических рекомендаций.</span><span class="sxs-lookup"><span data-stu-id="d1243-202">A quick look at a calendar shows that the team will have a total of six practices.</span></span> <span data-ttu-id="d1243-203">Однако в календаре не существует шести отдельных элементов встречи.</span><span class="sxs-lookup"><span data-stu-id="d1243-203">However, there aren't six distinct appointment items in the calendar.</span></span> <span data-ttu-id="d1243-204">Вместо этого существует только одна повторяющаяся Главная встреча, представляющая ряд.</span><span class="sxs-lookup"><span data-stu-id="d1243-204">Instead, there is just one recurring master appointment representing the series.</span></span>
  
<span data-ttu-id="d1243-205">Теперь рассмотрим Поиск встреч в календаре Ольга, который встречается в июле.</span><span class="sxs-lookup"><span data-stu-id="d1243-205">Now let's look at finding appointments on Sadie's calendar that occur within the month of July.</span></span> <span data-ttu-id="d1243-206">В следующем примере кода используется метод **FindItems** в управляемом API Exchange для создания нерасширенного представления календаря Ольга.</span><span class="sxs-lookup"><span data-stu-id="d1243-206">The following code example uses the **FindItems** method in the Exchange Managed API to produce a non-expanded view of Sadie's calendar.</span></span> 
  
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

<span data-ttu-id="d1243-207">Этот код приводит к следующему запросу [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d1243-207">That code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="d1243-208">Ответ сервера включает в себя только один элемент — шаблон повторения, указанный значением элемента [календаритемтипе](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) в **рекуррингмастер**.</span><span class="sxs-lookup"><span data-stu-id="d1243-208">The server's response includes only a single item, the recurring master, indicated by the [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element value of **RecurringMaster**.</span></span> <span data-ttu-id="d1243-209">Значение элемента [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1243-209">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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

<span data-ttu-id="d1243-210">Теперь выполним сравнение с расширенным представлением.</span><span class="sxs-lookup"><span data-stu-id="d1243-210">Now let's compare with an expanded view.</span></span> <span data-ttu-id="d1243-211">В следующем примере кода используется метод **FindAppointments** в УПРАВЛЯЕМОМ API EWS для создания расширенного представления календаря Ольга.</span><span class="sxs-lookup"><span data-stu-id="d1243-211">The following code example uses the **FindAppointments** method in the EWS Managed API to create an expanded view of Sadie's calendar.</span></span> 
  
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

<span data-ttu-id="d1243-212">Этот код приводит к следующему запросу [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d1243-212">This code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="d1243-213">В этот раз ответ сервера включает пять повторений, по одному для каждой среды в июле.</span><span class="sxs-lookup"><span data-stu-id="d1243-213">This time, the server response includes five occurrences, one for each Wednesday in July.</span></span> <span data-ttu-id="d1243-214">Элементы [календаритемтипе](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) для этих элементов имеют значение " **экземпляр**".</span><span class="sxs-lookup"><span data-stu-id="d1243-214">The [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) elements on these items all have a value of **Occurrence**.</span></span> <span data-ttu-id="d1243-215">Обратите внимание, что в отклике отсутствует шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="d1243-215">Note that the recurring master is not present in the response.</span></span> <span data-ttu-id="d1243-216">Значения элементов [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1243-216">The values of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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

<span data-ttu-id="d1243-217">После создания повторяющегося образца, вхождения или исключения всегда можно [получить другие связанные элементы](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d1243-217">After you have a recurring master, an occurrence, or an exception, you can always [retrieve the other related items](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="d1243-218">Получив исключение, вы можете извлечь шаблон повторения и наоборот.</span><span class="sxs-lookup"><span data-stu-id="d1243-218">Given an occurrence or exception, you can retrieve the recurring master, and vice versa.</span></span>
  
## <a name="working-with-recurring-calendar-items"></a><span data-ttu-id="d1243-219">Работа с повторяющимися элементами календаря</span><span class="sxs-lookup"><span data-stu-id="d1243-219">Working with recurring calendar items</span></span>

<span data-ttu-id="d1243-220">Для работы с повторяющимися элементами календаря используются те же методы и операции, что и при работе с неповторяющимися элементами календаря.</span><span class="sxs-lookup"><span data-stu-id="d1243-220">You use all the same methods and operations to work with recurring series as you use to work with non-recurring calendar items.</span></span> <span data-ttu-id="d1243-221">Разница заключается в том, что в зависимости от элемента, используемого для вызова этих методов или операций, выполняемые действия можно применить ко всей серии или только к одному экземпляру.</span><span class="sxs-lookup"><span data-stu-id="d1243-221">The difference is that, depending on the item you use to invoke those methods or operations, the actions you take can apply to the entire series, or just a single occurrence.</span></span> <span data-ttu-id="d1243-222">[Действия, выполняемые на повторяющейся основной реплике](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) , будут применяться ко всем вхождениям в ряду, в то время как [действия, выполненные с одним экземпляром или исключением](how-to-update-a-recurring-series-by-using-ews.md) , будут применяться только к этому экземпляру или исключению.</span><span class="sxs-lookup"><span data-stu-id="d1243-222">[Actions taken on the recurring master](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) will apply to all occurrences in the series, while [actions taken to a single occurrence or exception](how-to-update-a-recurring-series-by-using-ews.md) will only apply to that occurrence or exception.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="d1243-223">Содержание</span><span class="sxs-lookup"><span data-stu-id="d1243-223">In this section</span></span>

- [<span data-ttu-id="d1243-224">Доступ к повторяющимся сериям с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-224">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d1243-225">Создание серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-225">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d1243-226">Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-226">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d1243-227">Обновление серии повторяющихся данных с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="d1243-227">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="d1243-228">Обновление серии повторяющихся данных с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-228">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="d1243-229">См. также</span><span class="sxs-lookup"><span data-stu-id="d1243-229">See also</span></span>


- [<span data-ttu-id="d1243-230">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-230">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d1243-231">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-231">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="d1243-232">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1243-232">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

