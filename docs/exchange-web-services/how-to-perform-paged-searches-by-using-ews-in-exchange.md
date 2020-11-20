---
title: Выполнение страничного поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Узнайте, как выполнять страничный поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.
localization_priority: Priority
ms.openlocfilehash: fa36a2ce77150f29e5a62876138c9693a3b4ab1f
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348824"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="38400-103">Выполнение страничного поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="38400-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="38400-104">Узнайте, как выполнять страничный поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.</span><span class="sxs-lookup"><span data-stu-id="38400-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="38400-105">Разбиение на страницы — это функция в EWS, которая позволяет управлять размером результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="38400-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="38400-106">Вместо получения всех результатов в одном ответе EWS можно получить меньше результатов в нескольких ответах EWS. </span><span class="sxs-lookup"><span data-stu-id="38400-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="38400-107">Например, представьте, что в папке "Входящие" пользователя находится 10 000 сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="38400-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="38400-108">Гипотетически можно получать все 10 000 сообщений электронной почты в одном огромном ответе, но можно разбить его на более доступные для управления блоки по соображениям пропускной способности или производительности.</span><span class="sxs-lookup"><span data-stu-id="38400-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="38400-109">Разбиение на страницы дает вам инструменты для этого.</span><span class="sxs-lookup"><span data-stu-id="38400-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="38400-110">Хотя можно получить 10 000 элементов в одном запросе, в действительности это маловероятно из-за регулирования EWS.</span><span class="sxs-lookup"><span data-stu-id="38400-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="38400-111">Дополнительные сведения см. в разделе [регулирование EWS в Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="38400-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="38400-112">**Таблица 1. Параметры разбиения на страницы в управляемом API EWS и EWS**</span><span class="sxs-lookup"><span data-stu-id="38400-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="38400-113">**Чтобы настроить или получить...**</span><span class="sxs-lookup"><span data-stu-id="38400-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="38400-114">**В управляемом API EWS, используйте...**</span><span class="sxs-lookup"><span data-stu-id="38400-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="38400-115">**В EWS используйте...**</span><span class="sxs-lookup"><span data-stu-id="38400-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38400-116">Максимальное количество элементов или папок в ответе</span><span class="sxs-lookup"><span data-stu-id="38400-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="38400-117">Параметр **pageSize** [конструктора ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) или [конструктора FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="38400-118">Или</span><span class="sxs-lookup"><span data-stu-id="38400-118">Or</span></span>  <br/> <span data-ttu-id="38400-119">Свойство [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-120">Атрибут **MaxEntriesReturned** элемента [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="38400-121">Начальная точка в списке элементов или папок</span><span class="sxs-lookup"><span data-stu-id="38400-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="38400-122">Параметр **offsetBasePoint** конструктора **ItemView** или конструктора **FolderView**</span><span class="sxs-lookup"><span data-stu-id="38400-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="38400-123">Или</span><span class="sxs-lookup"><span data-stu-id="38400-123">Or</span></span>  <br/> <span data-ttu-id="38400-124">Свойство [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-125">Атрибут **BasePoint** элемента **IndexedPageItemView** или элемента **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="38400-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="38400-126">Смещение от начальной точки</span><span class="sxs-lookup"><span data-stu-id="38400-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="38400-127">Параметр **offset** конструктора **ItemView** или конструктора **FolderView**</span><span class="sxs-lookup"><span data-stu-id="38400-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="38400-128">Или</span><span class="sxs-lookup"><span data-stu-id="38400-128">Or</span></span>  <br/> <span data-ttu-id="38400-129">Свойство [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-130">Атрибут **Offset** элемента **IndexedPageItemView** элемента **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="38400-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="38400-131">Общее число результатов на сервере</span><span class="sxs-lookup"><span data-stu-id="38400-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="38400-132">Свойство [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-133">Атрибут **TotalItemsInView** элемента [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="38400-134">Смещение первого элемента или папки, не включенных в текущий ответ</span><span class="sxs-lookup"><span data-stu-id="38400-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="38400-135">Свойство [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-136">Атрибут **IndexedPagingOffset** элемента **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="38400-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="38400-137">Индикатор того, что ответ включает последний элемент или папку в списке</span><span class="sxs-lookup"><span data-stu-id="38400-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="38400-138">Свойство [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38400-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="38400-139">Атрибут **IncludesLastItemInRange** элемента **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="38400-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="38400-140">Как работает разбиение на страницы</span><span class="sxs-lookup"><span data-stu-id="38400-140">How paging works</span></span>
<span data-ttu-id="38400-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="38400-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="38400-142">Чтобы понять, как работает разбиение на страницы, можно визуализировать сообщения в папке, чтобы они отображались в виде рекламных щитов, выстроенных бок о бок в поле за вашим домом.</span><span class="sxs-lookup"><span data-stu-id="38400-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="38400-143">Некоторые из этих рекламных щитов можно увидеть через волшебное окно.</span><span class="sxs-lookup"><span data-stu-id="38400-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="38400-144">У вас есть возможность изменять размер окна (чтобы видеть больше или меньше рекламных щитов одновременно) и перемещать окно (чтобы управлять тем, какие рекламные щиты вы видите).</span><span class="sxs-lookup"><span data-stu-id="38400-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="38400-145">Эта манипуляция с окном и есть разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="38400-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="38400-146">При отправке запроса на сервер Exchange Server необходимо определить размер окна с точки зрения количества элементов, которые необходимо вернуть.</span><span class="sxs-lookup"><span data-stu-id="38400-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="38400-147">Установить положение окна можно задав начальную точку (начало строки или конец строки) и смещение от этой начальной точки, выраженное в количестве элементов.</span><span class="sxs-lookup"><span data-stu-id="38400-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="38400-148">Начало окна — это количество элементов, заданное смещением от начальной точки.</span><span class="sxs-lookup"><span data-stu-id="38400-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="38400-149">Разбиение на страницы более интереснее в ответе сервера и в том, как ваше приложение может использовать этот ответ для формирования следующего запроса.</span><span class="sxs-lookup"><span data-stu-id="38400-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="38400-150">Сервер предоставляет три фрагмента сведений, которые можно использовать, чтобы определить, как настроить ваше «окно» для вашего следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="38400-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="38400-151">Включают ли результаты в ответ последний элемент в общие результаты на сервере.</span><span class="sxs-lookup"><span data-stu-id="38400-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="38400-152">Общее количество элементов в результатах на сервере.</span><span class="sxs-lookup"><span data-stu-id="38400-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="38400-153">Каким должно быть следующее значение смещения, если вы хотите переместить ваше окно к следующему элементу в результатах, который не включен в текущий ответ.</span><span class="sxs-lookup"><span data-stu-id="38400-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="38400-154">Рассмотрим простой пример.</span><span class="sxs-lookup"><span data-stu-id="38400-154">Let's look at a simple example.</span></span> <span data-ttu-id="38400-155">Представьте папку "Входящие" с 15 сообщениями.</span><span class="sxs-lookup"><span data-stu-id="38400-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="38400-156">Приложение отправляет начальный запрос на получение не более 10 элементов, начиная с начала списка сообщений (поэтому смещение равно нулю).</span><span class="sxs-lookup"><span data-stu-id="38400-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="38400-157">Сервер отвечает первыми 10 сообщениями и указывает, что ответ не включает последний элемент, что всего присутствует 15 элементов и что следующее смещение должно быть равно 10.</span><span class="sxs-lookup"><span data-stu-id="38400-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="38400-158">**Рисунок 1. Запрос 10 элементов с нулевым смещением от начала списка, состоящего из 15 элементов**</span><span class="sxs-lookup"><span data-stu-id="38400-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов с нулевым смещением от начала списка, состоящего из 15 элементов.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="38400-160">Приложение повторно отправляет тот же запрос на сервер с единственным изменением, заключающимся в том, что теперь смещение равно 10.</span><span class="sxs-lookup"><span data-stu-id="38400-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="38400-161">Сервер возвращает последние пять элементов и указывает, что в ответе содержится последний элемент, что всего присутствует 15 элементов, а следующее смещение должно быть равно 15 (хотя конец достигнут, поэтому следующего смещения не будет.)</span><span class="sxs-lookup"><span data-stu-id="38400-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="38400-162">**Рисунок 2. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов**</span><span class="sxs-lookup"><span data-stu-id="38400-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="38400-164">Анализ дизайна для разбиения на страницы</span><span class="sxs-lookup"><span data-stu-id="38400-164">Design considerations for paging</span></span>
<span data-ttu-id="38400-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="38400-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="38400-166">Чтобы максимально эффективно использовать разбиение на страницы в приложении, необходимо учитывать некоторые вопросы.</span><span class="sxs-lookup"><span data-stu-id="38400-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="38400-167">Например, насколько большим можно сделать "окно"?</span><span class="sxs-lookup"><span data-stu-id="38400-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="38400-168">Что делать, если результаты на сервере меняются при перемещении «окна»?</span><span class="sxs-lookup"><span data-stu-id="38400-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="38400-169">Определение размера окна</span><span class="sxs-lookup"><span data-stu-id="38400-169">Determine the size of your window</span></span>

<span data-ttu-id="38400-170">Не существует универсального максимального количества записей, которое должны использовать все приложения.</span><span class="sxs-lookup"><span data-stu-id="38400-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="38400-171">Выбор числа, подходящего для вашего приложения, зависит от нескольких факторов.</span><span class="sxs-lookup"><span data-stu-id="38400-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="38400-172">Тем не менее, рекомендуется учитывать следующие моменты:</span><span class="sxs-lookup"><span data-stu-id="38400-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="38400-173">По умолчанию Exchange ограничивает максимальное количество элементов, которые могут быть возвращены в одном запросе, до 1000.</span><span class="sxs-lookup"><span data-stu-id="38400-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="38400-174">Установка максимального числа записей на большее количество элементов приводит к необходимости отправлять меньше запросов для получения всех элементов за счет более длительного ожидания ответов.</span><span class="sxs-lookup"><span data-stu-id="38400-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="38400-175">Установка максимального количества записей на меньшее количество элементов приводит к более быстрому времени отклика за счет необходимости отправлять больше запросов для получения всех элементов.</span><span class="sxs-lookup"><span data-stu-id="38400-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="38400-176">Обработка изменений в результирующем наборе</span><span class="sxs-lookup"><span data-stu-id="38400-176">Handling changes to the result set</span></span>

<span data-ttu-id="38400-177">В простом примере, приведенном ранее в этой статье, количество элементов в папке «Входящие» пользователя оставалось постоянным.</span><span class="sxs-lookup"><span data-stu-id="38400-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="38400-178">Однако в действительности количество элементов в папке «Входящие» может часто меняться.</span><span class="sxs-lookup"><span data-stu-id="38400-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="38400-179">Новые сообщения могут приходить, а элементы могут быть удалены или перемещены в любое время.</span><span class="sxs-lookup"><span data-stu-id="38400-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="38400-180">Но как это повлияет на разбиение на страницы?</span><span class="sxs-lookup"><span data-stu-id="38400-180">But how does this impact paging?</span></span> <span data-ttu-id="38400-181">Давайте изменим предыдущий примерный сценарий, чтобы выяснить это.</span><span class="sxs-lookup"><span data-stu-id="38400-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="38400-182">Начнем снова с 15 элементов в папке «Входящие» пользователя и отправим тот же начальный запрос.</span><span class="sxs-lookup"><span data-stu-id="38400-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="38400-183">Как и раньше, сервер отвечает первыми 10 сообщениями и указывает, что ответ не включает последний элемент, что всего присутствует 15 элементов и что следующее смещение должно быть равно 10, как показано на рисунке 1.</span><span class="sxs-lookup"><span data-stu-id="38400-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="38400-184">Пока приложение обрабатывает эти 10 элементов, новое сообщение поступает в папку «Входящие» и добавляется в результирующий набор на сервере.</span><span class="sxs-lookup"><span data-stu-id="38400-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="38400-185">Приложение повторно отправляет тот же запрос на сервер (только с установленным смещением 10).</span><span class="sxs-lookup"><span data-stu-id="38400-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="38400-186">На этот раз сервер возвращает шесть элементов и указывает, что всего в результирующем наборе 16 элементов.</span><span class="sxs-lookup"><span data-stu-id="38400-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="38400-187">На этом этапе вам может быть интересно, действительно ли это проблема.</span><span class="sxs-lookup"><span data-stu-id="38400-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="38400-188">В конце концов, вы получили 16 элементов по двум ответам, так в чем проблема?</span><span class="sxs-lookup"><span data-stu-id="38400-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="38400-189">Ответ зависит от того, где в списке размещен новый элемент.</span><span class="sxs-lookup"><span data-stu-id="38400-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="38400-190">Если список отсортирован так, что самые старые элементы (по дате и времени получения) идут первыми, то с этим сценарием все в порядке.</span><span class="sxs-lookup"><span data-stu-id="38400-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="38400-191">Новый элемент будет помещен в конец списка и будет включен во второй ответ.</span><span class="sxs-lookup"><span data-stu-id="38400-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="38400-192">**Рисунок 3. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, при этом 16-й элемент в списке является новым**</span><span class="sxs-lookup"><span data-stu-id="38400-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="38400-194">Другое дело, если список отсортирован так, что на первом месте находятся самые новые элементы.</span><span class="sxs-lookup"><span data-stu-id="38400-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="38400-195">В этом случае первый элемент во втором запросе будет последним элементом из предыдущего запроса плюс оставшиеся пять элементов из исходных 15.</span><span class="sxs-lookup"><span data-stu-id="38400-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="38400-196">Выражаясь в терминах нашего воображаемого волшебного окна, вы сместили положение своего окна на 10, но сами рекламные щиты также сдвинулись на 1.</span><span class="sxs-lookup"><span data-stu-id="38400-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="38400-197">**Рисунок 4. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, при этом первый элемент в списке является новым**</span><span class="sxs-lookup"><span data-stu-id="38400-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="38400-199">Один из способов выявления изменения результатов на сервере является использование концепции элемента привязки.</span><span class="sxs-lookup"><span data-stu-id="38400-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="38400-200">Элемент привязки — это дополнительный элемент в ответе, который не обрабатывается вместе с остальными результатами, но используется для сравнения со следующей результатами, чтобы проверить, сместились ли сами элементы.</span><span class="sxs-lookup"><span data-stu-id="38400-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="38400-201">Опять же, основываясь на нашем простом примере, если приложение использует размер «окна» равный 10, вы фактически устанавливаете максимальное количество возвращаемых элементов равным 11.</span><span class="sxs-lookup"><span data-stu-id="38400-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="38400-202">Приложение обрабатывает первые 10 элементов ответа обычным способом.</span><span class="sxs-lookup"><span data-stu-id="38400-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="38400-203">Для последнего элемента вы сохраняете идентификатор элемента в качестве элемента привязки, а затем отправляете следующий запрос со смещением 10.</span><span class="sxs-lookup"><span data-stu-id="38400-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="38400-204">Если данные не изменились, первый элемент во втором ответе должен иметь идентификатор элемента, соответствующий привязке.</span><span class="sxs-lookup"><span data-stu-id="38400-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="38400-205">Если идентификаторы элементов не совпадают, вы знаете, что данные были удалены или вставлены в те части списка, которые вы уже «перелистали».</span><span class="sxs-lookup"><span data-stu-id="38400-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="38400-206">Даже если вы знаете, что данные изменились, вам все равно нужно решить, как реагировать.</span><span class="sxs-lookup"><span data-stu-id="38400-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="38400-207">На этот вопрос также не существует универсального ответа.</span><span class="sxs-lookup"><span data-stu-id="38400-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="38400-208">Ваши действия будут зависеть от характера вашего приложения и от того, насколько важно захватить все элементы.</span><span class="sxs-lookup"><span data-stu-id="38400-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="38400-209">Можно проигнорировать это, перезапустить процесс с самого начала или вернуться назад и попытаться определить, где произошло изменение.</span><span class="sxs-lookup"><span data-stu-id="38400-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="38400-210">Пример: Выполнение страничного поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="38400-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="38400-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="38400-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="38400-212">Разбиение на страницы поддерживается следующими методами управляемого API EWS:</span><span class="sxs-lookup"><span data-stu-id="38400-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="38400-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="38400-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="38400-217">При использовании управляемого API EWS приложение настраивает разбиение на страницы с помощью класса [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) или [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) и получает с сервера сведения о разбиении на страницы из класса [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) или [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="38400-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="38400-218">В следующем примере все элементы в папке извлекаются с помощью страничного поиска, который возвращает пять элементов в каждом ответе.</span><span class="sxs-lookup"><span data-stu-id="38400-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="38400-219">Он также извлекает дополнительный элемент, который будет использоваться в качестве привязки для обнаружения изменений результатов на сервере.</span><span class="sxs-lookup"><span data-stu-id="38400-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="38400-220">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="38400-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems && anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
                
            anchorId = results.Items.Last<Item>().Id;
            
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = 0;
            if ((results.MoreAvailable == false && results.Items.Count > pageSize) || (results.Items.Count < pageSize))
            {
                displayCount = results.Items.Count;
            }
            else
            {
                displayCount = pageSize;
            }
            
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="38400-221">Пример: Выполнение страничного поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="38400-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="38400-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="38400-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="38400-223">Разбиение на страницы поддерживается следующими операциями EWS:</span><span class="sxs-lookup"><span data-stu-id="38400-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="38400-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="38400-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="38400-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="38400-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="38400-226">При использовании EWS приложение настраивает разбиение на страницы с помощью элемента [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) и получает с сервера сведения о разбиении на страницы из элемента [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="38400-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="38400-227">В этом примере запроса запрос **FindItem** отправляется максимум для шести элементов, начиная с нулевого смещения от начала списка элементов в папке «Входящие» пользователя.</span><span class="sxs-lookup"><span data-stu-id="38400-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38400-228">Сервер возвращает следующий ответ, содержащий шесть элементов.</span><span class="sxs-lookup"><span data-stu-id="38400-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="38400-229">Ответ также указывает, что в результатах на сервере содержится всего восемь элементов, а в этом ответе не присутствует последний элемент в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="38400-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="38400-230">В этом примере отправляется тот же запрос, но на этот раз атрибут **Offset** изменен на 5, что указывает на то, что сервер должен вернуть не более шести элементов, начиная со смещения, равного пяти от начала.</span><span class="sxs-lookup"><span data-stu-id="38400-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38400-231">Сервер отправляет следующий ответ, содержащий три элемента.</span><span class="sxs-lookup"><span data-stu-id="38400-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="38400-232">Ответ также указывает, что общее количество элементов в результатах на сервере по-прежнему равно восьми, и что последний элемент в списке результатов включен в этот ответ.</span><span class="sxs-lookup"><span data-stu-id="38400-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="38400-233">См. также</span><span class="sxs-lookup"><span data-stu-id="38400-233">See also</span></span>


- [<span data-ttu-id="38400-234">Поиск и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="38400-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="38400-235">Метод ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-236">Метод ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="38400-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-237">Метод Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-238">Метод Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="38400-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="38400-239">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="38400-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="38400-240">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="38400-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="38400-241">EWS регулирование в Exchange</span><span class="sxs-lookup"><span data-stu-id="38400-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

